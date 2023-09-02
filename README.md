import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class LibraryManagementGUI extends JFrame {
    private JTextField idField;
    private JTextField titleField;
    private JTextArea outputArea;
    private Book[] books;

    public LibraryManagementGUI() {
        setTitle("Library Management System");
        setSize(400, 300);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLayout(new BorderLayout());

        JPanel inputPanel = new JPanel();
        inputPanel.setLayout(new GridLayout(4, 2));

        JLabel idLabel = new JLabel("Book ID:");
        idField = new JTextField();
        JLabel titleLabel = new JLabel("Book Title:");
        titleField = new JTextField();

        JButton setDetailsButton = new JButton("Set Details");
        setDetailsButton.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                int id = Integer.parseInt(idField.getText());
                String title = titleField.getText();
                int index = findEmptyBookSlot();
                if (index != -1) {
                    books[index] = new Book(id, title);
                    outputArea.setText("Details set successfully.");
                } else {
                    outputArea.setText("No available slots for a new book.");
                }
            }
        });

        JButton getDetailsButton = new JButton("Get Details");
        getDetailsButton.addActionListener(new ActionListener() {
            public void actionPerformed(ActionEvent e) {
                int id = Integer.parseInt(idField.getText());
                int index = findBookIndexById(id);
                if (index != -1) {
                    String bookDetails = books[index].getDetails();
                    outputArea.setText(bookDetails);
                } else {
                    outputArea.setText("Book not found.");
                }
            }
        });

        inputPanel.add(idLabel);
        inputPanel.add(idField);
        inputPanel.add(titleLabel);
        inputPanel.add(titleField);
        inputPanel.add(setDetailsButton);
        inputPanel.add(getDetailsButton);

        outputArea = new JTextArea();
        outputArea.setEditable(false);

        add(inputPanel, BorderLayout.NORTH);
        add(outputArea, BorderLayout.CENTER);

        books = new Book[10]; // You can adjust the size as needed
    }

    private int findEmptyBookSlot() {
        for (int i = 0; i < books.length; i++) {
            if (books[i] == null) {
                return i;
            }
        }
        return -1; // No empty slots found
    }

    private int findBookIndexById(int id) {
        for (int i = 0; i < books.length; i++) {
            if (books[i] != null && books[i].getBookId() == id) {
                return i;
            }
        }
        return -1; // Book not found
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(new Runnable() {
            public void run() {
                LibraryManagementGUI gui = new LibraryManagementGUI();
                gui.setVisible(true);
            }
        });
    }
}

class Book {
    private int bookId;
    private String bookTitle;

    public Book(int bookId, String bookTitle) {
        this.bookId = bookId;
        this.bookTitle = bookTitle;
    }

    public int getBookId() {
        return bookId;
    }

    public String getDetails() {
        return "Book ID: " + bookId + "\nBook Title: " + bookTitle;
    }
}

