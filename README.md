import java.util.*;
public class book
{
    int bookId;
    String bookTitle;
    int yearOfPublication;
String authorName;
String publisherName;
int availableCopies;
int totalCopies;
public void setDetails(){
this.bookId=0;
 this.bookTitle="";
 this.yearOfPublication=0;
this.authorName=null;
this.publisherName="";
this.availableCopies =0;
this.totalCopies=0;
}
public void getDetails(int id){
System.out.println("Bookid is "+this.bookId);
System.out.println("Book title is "+this.bookTitle);
System.out.println("Publisher name is "+this.yearOfPublication);
System.out.println("Author name is "+this.authorName);
System.out.println("Publisher name is "+this.publisherName);
System.out.println("Number of available copies are "+this.availableCopies);
System.out.println("Number of total copies are "+this.totalCopies);
}
public void setDetails(int id,String title,int year, String author,String publisher,int count){
this.bookId=id;
 this.bookTitle=title;
 this.yearOfPublication=year;
this.authorName=author;
this.publisherName=publisher;
this.availableCopies =count;
}
void issue(int id){
if(availableCopies>0)
{
    this.availableCopies-=1;
     System.out.println("Book is issued");}
     else
     System.out.println("Book is not issued yet");
}

void returnbook (int id){


if(availableCopies<totalCopies){
    this.availableCopies+=1;
    System.out.println("Book is returned successfully");}
 this.availableCopies+=1;
    System.out.println("Book is returned successfully");}
    else
    System.out.println("Book is not returned yet");
}
book(){
 bookId=0;
 bookTitle="";
    yearOfPublication=0;
authorName=null;
publisherName="";
availableCopies =0;
totalCopies=0;
}
book(int totalCopies)
{
this.totalCopies=totalCopies;
}
public static void main(String []args)
{
    Scanner sc=new Scanner (System.in);
int i=1;
int n;
System.out.println("Enter the number of books");
n=sc.nextInt();
book a[]=new book[n];
for(int j=0;j<n;j++)

{System.out.println("Enter total number of copies");
    int x=sc.nextInt();
    a[i]=new book(x);
}
int ch;
while(i!=0){
System.out.println("To set the details press 1");
System.out.println("To get the details press 2");
System.out.println("To issue press 3");
System.out.println("To return press 4");
System.out.println("To exit press 5");
System.out.println("Please enter your choice");
 this.availableCopies+=1;
    System.out.println("Book is returned successfully");}
    else
    System.out.println("Book is not returned yet");
}
book(){
 bookId=0;
 bookTitle="";
    yearOfPublication=0;
authorName=null;
publisherName="";
availableCopies =0;
totalCopies=0;
}
book(int totalCopies)
{
this.totalCopies=totalCopies;
}
public static void main(String []args)
{
    Scanner sc=new Scanner (System.in);
int i=1;
int n;
System.out.println("Enter the number of books");
n=sc.nextInt();
book a[]=new book[n];
for(int j=0;j<n;j++)

{System.out.println("Enter total number of copies");
    int x=sc.nextInt();
    a[i]=new book(x);
}
int ch;
while(i!=0){
System.out.println("To set the details press 1");
System.out.println("To get the details press 2");
System.out.println("To issue press 3");
System.out.println("To return press 4");
System.out.println("To exit press 5");
System.out.println("Please enter your choice");
 this.availableCopies+=1;
    System.out.println("Book is returned successfully");}
    else
    System.out.println("Book is not returned yet");
}
book(){
 bookId=0;
 bookTitle="";
    yearOfPublication=0;
authorName=null;
publisherName="";
availableCopies =0;
totalCopies=0;
}
book(int totalCopies)
{
this.totalCopies=totalCopies;
}
public static void main(String []args)
{
    Scanner sc=new Scanner (System.in);
int i=1;
int n;
System.out.println("Enter the number of books");
n=sc.nextInt();
book a[]=new book[n];
for(int j=0;j<n;j++)

{System.out.println("Enter total number of copies");
    int x=sc.nextInt();
    a[i]=new book(x);
}
int ch;
while(i!=0){
System.out.println("To set the details press 1");
System.out.println("To get the details press 2");
System.out.println("To issue press 3");
System.out.println("To return press 4");
System.out.println("To exit press 5");
System.out.println("Please enter your choice");
 this.availableCopies+=1;
    System.out.println("Book is returned successfully");}
    else
    System.out.println("Book is not returned yet");
}
book(){
 bookId=0;
 bookTitle="";
    yearOfPublication=0;
authorName=null;
publisherName="";
availableCopies =0;
totalCopies=0;
}
book(int totalCopies)
{
this.totalCopies=totalCopies;
}
public static void main(String []args)
{
    Scanner sc=new Scanner (System.in);
int i=1;
int n;
System.out.println("Enter the number of books");
n=sc.nextInt();
book a[]=new book[n];
for(int j=0;j<n;j++)

{System.out.println("Enter total number of copies");
    int x=sc.nextInt();
    a[i]=new book(x);
}
int ch;
while(i!=0){
System.out.println("To set the details press 1");
System.out.println("To get the details press 2");
System.out.println("To issue press 3");
System.out.println("To return press 4");
System.out.println("To exit press 5");
System.out.println("Please enter your choice");
v this.availableCopies+=1;
    System.out.println("Book is returned successfully");}
    else
    System.out.println("Book is not returned yet");
}
book(){
 bookId=0;
 bookTitle="";
    yearOfPublication=0;
authorName=null;
publisherName="";
availableCopies =0;
totalCopies=0;
}
book(int totalCopies)
{
this.totalCopies=totalCopies;
}
public static void main(String []args)
{
    Scanner sc=new Scanner (System.in);
int i=1;
int n;
System.out.println("Enter the number of books");
n=sc.nextInt();
book a[]=new book[n];
for(int j=0;j<n;j++)

{System.out.println("Enter total number of copies");
    int x=sc.nextInt();
    a[i]=new book(x);
}
int ch;
while(i!=0){
System.out.println("To set the details press 1");
System.out.println("To get the details press 2");
System.out.println("To issue press 3");
System.out.println("To return press 4");
System.out.println("To exit press 5");
System.out.println("Please enter your choice");
ch=sc.nextInt();
switch (ch)
{
case 1:
{System.out.println("Enter id, title of book, year of publication, author name, publisher name, number of available copies and book number");
int id1=sc.nextInt();
String title=sc.next();
int year=sc.nextInt();
String author=sc.next();
String publisher=sc.next();
int count=sc.nextInt();
int k1=sc.nextInt();
a[k1].setDetails(id1,title,year,author,publisher,count);
System.out.println("Object of book number "+k1+" has been created");
break;}
case 2:
{int id2=sc.nextInt();
    int k2=sc.nextInt();
a[k2].getDetails(id2);
break;}
case 3:
{
    System.out.println("Enter the id and book number ");
int id3=sc.nextInt();
int k3=sc.nextInt();
a[k3].issue(id3);
break;
}
case 4:
{System.out.println("Enter the id and book number ");
int id4=sc.nextInt();
int k4=sc.nextInt();
a[k4].returnbook(id4);
break;}
case 5:
i=0;
break;
default:
System.out.println("Wrong choice");
}
}
}}
