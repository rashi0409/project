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
