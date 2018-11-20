# CC2-projects
1H , FARRO FREDERICK ANTHONY A.

TITLE: "AREAS"
  
   
package userinput;



import java.util.*;


public class Calculator {
    public static void main (String [] args) {
     
        Scanner sc = new Scanner(System.in);
        System.out.println ("Enter the first number: ");
        int a = sc.nextInt();
        System.out.println ("Enter the second number: ");
        int b = sc.nextInt();
        
        System.out.println ("What arithmetic operation to be used(add, subtract, multiply, divide, modulo): ");
        String c = sc.next();                
        
        int sum, diff, prod, quo, mod;
        sum = a + b;
        diff = a - b;
        prod = a * b;
        quo = a / b;
        mod = a % b;
        
        if (c.equals("add")){
            System.out.println ( "Sum is: "+ sum);
        } else if (c.equals("subtract")){
            System.out.println ( "Difference is: "+ diff);
        }else if (c.equals("multiply")){
            System.out.println ( "Product is: "+ prod);
        } else if (c.equals("divide")){
             System.out.println ( "Quotient is: "+ quo);
        } else if (c.equals("modulo")){
             System.out.println ( "Modulo is: "+ mod);
        }
    }
}





CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "CALCULATOR (GUESSING GAME)"



package repetitivestructures;

import java.util.*;


public class GuessingNumber {
    public static void main (String [] args){
        Scanner sc = new Scanner (System.in);
        
        System.out.println("Enter a number from 0 - 1000:");
        int a = sc.nextInt(); 
        
        if (a>1000){
            System.out.println("Invalid.");
        }else if (a<0){
            System.out.println("Invalid");
        }else{
        
        
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();
        System.out.println();                                                                              
        System.out.println();
        System.out.println();  
        System.out.println();                                                                              
        System.out.println();
        System.out.println(); 
        System.out.println();
        System.out.println();    
        
        System.out.println("Guess a number from 0 - 1000:");
        int guess = sc.nextInt();
        
        if (guess>1000){
            System.out.println("Invalid.");
        }else if (guess<0){
            System.out.println("Invalid");
        }else{
            do{
                if (a%2==0){
                System.out.println("Hint:The number is an even number.");
                guess = sc.nextInt();
                }else{
                System.out.println("Hint:The number is an odd number.");
                guess = sc.nextInt();
                }if (guess < a){
                    System.out.println("Hint:The number is higher.");
                    guess = sc.nextInt();
                }else if (guess > a){
                    System.out.println("Hint:The number is lower");
                    guess = sc.nextInt();
                }
            }while (guess!=a);
                System.out.println("You have guessed the correct number.");
               System.out.println("Congratulations!");
            }
        }
    }
}



CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "COURSE" 


package multiarray;
             
 package nestedif;

import java.util.Scanner;


public class NestedIf {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        
         Scanner sc = new Scanner (System.in);
        String course   = sc.nextLine ();
        
        if (course.equals (" BSIT OR BSCS ")){
            String major = sc.nextLine ();
            System.out.println("Enter your course: BSIT or BSCS ");
            String x= sc.nextLine ();
            
            
            if (course.equals ("BSIT")){
                major = sc.nextLine ();
            }
            if (x.equals ("NETSEC")){
                System.out.println("BSIT- NETSEC");
            }
            else if (x.equals ("WebDeveloper")){
                System.out.println(" BSIT- WEBDEVELOPER");
            }
            else if (x.equals ("Erp")){
                System.out.println("BSIT-ERP");
            }
        }
           String major = sc.nextLine ();
            System.out.println("Enter your course: BSIT or BSCS ");
            course = sc.nextLine ();
       
            if (course.equals ("BSCS")){
                major = sc.nextLine ();
            }
            
            if (major.equals ("NETSEC")){
                System.out.println("BSCS- NETSEC");
            }
            else if (major.equals ("WebDeveloper")){
                System.out.println(" BSCS- WEBDEVELOPER");
            }
            else if (major.equals ("ERP")){
                System.out.println("BSCS-ERP");
            }
            
        }   
            
    }
    



CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "GUESSING GAME"
  

package frederick0000;
import java.util.*;

public class Frederick0000 {

    public static void main(String[] args) {
         System.out.println("Odd\t\t\tEven");
        
        
        ArrayList hehe = new ArrayList();
        ArrayList booo = new ArrayList();
        
        int i;
        int[] numbers ={3,9,15,20,65,23,18,4,2,14};
        for(i = 0; i< numbers.length; i++){
            
            if(numbers[i] % 2 == 0){
                hehe.add(numbers[i]);
            
            }else{
                booo.add(numbers[i]);
                
            }
        }
            for(i = 0; i< numbers.length; i++){
                if(i>=hehe.size() && i<booo.size()){
                    System.out.println("\t\t\t"+booo.get(i));
                  
                }
                else if(i>=booo.size() && i<hehe.size()){
                   System.out.println(hehe.get(i));
                   
                }
                else if(i<booo.size() && i<hehe.size()){
                    System.out.println(booo.get(i)+"\t\t\t"+ hehe.get(i));
                }
        } 
    }
    
}

CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "2D ROWS AND COLUMNS"
  
 
 package pkg2d;
import java.util.*;

public class Main {

    public static void main(String[] args) {
    Scanner sc = new Scanner (System.in);
    
        System.out.println("Enter number of rows: ");
        int r = sc.nextInt();
        
        System.out.println("Enter number of columns: ");
        int c = sc.nextInt();
        
        int [][] a = new int [c][r]; 
        
        for(int i=0; i<a.length; i++){
            for(int b=0; b<a[i].length; b++){
                System.out.println("Enter number of row " + (b+1) + " and column " + (i+1) + ":" );
                a [i][b]= sc.nextInt() ;
            }
        }
            for (int x=0; x<a.length; x++){
                
                for(int d=0; d<a[x].length; d++){
                    System.out.print(a[x][d] + "\t");
                }
                        System.out.println("");
            }
            
        }
    
    }
    


CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "1D ODD and EVEN TABLE"
  
  
package guessinggame;

import java.util.Scanner;
/**
 *
 * @author CC2_1H-9
 */
     public class GuessingGame {
           public static void main (String [] args) {
           Scanner kb = new Scanner (System.in);

           System.out.println("Guess a number between 0-1000: ");
           int a = kb.nextInt();

           System.out.println("Guess a number between 0-1000: ");
           int b = kb.nextInt();

           System.out.println("Hint:");

           
           if (a % 2==0){
           System.out.println("The number is even");
           }

           else {
           System.out.println("the number is odd");
          }

          do { 
          if (b<a){
          System.out.println("Enter a Higher Value: ");
          b = kb.nextInt();
          }
          else if (b>a){
          System.out.println("Enter a Lower value: ");
          b= kb.nextInt();

          }

         while(b!=a);
         System.out.println("You guessed the correct answer");

          }
             
             
            
CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "2D ODD and EVEN TABLE" 

  
package multiarray;

import java.util.*;

public class MultiArray {

   
    public static void main(String[] args) {
      Scanner sc= new Scanner (System.in);
      int rows;
      int columns;
        System.out.println("Enter number of rows: ");
        rows = sc.nextInt();
        System.out.println("Now enter the number of columns: ");
        columns= sc.nextInt();
       int[][]b = new int [rows][columns];
       for (int i=0; i<rows; i++){
           for (int j=0; j<columns; j++){
               System.out.println("Enter the number for Row " + (i+1) + " and Column " + (j+1) + " :  " );
               b[i][j]= sc.nextInt();
               
           
           }
           
       }
           
       for (int i=0;i<b.length;i++){
        System.out.println("\nRow:" + i + "\tColumn:");
        for (int j=0; j<b.length; j++){
            System.out.print(b[i][j]+ "\t");
            
        }
    }
       
     
        
        
        
    }
    
}
             
             
             
CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "FIBONACCI"
  
  

package fibonacci;

import java.io.*;
import java.util.*;
public class Fibonacci {
    
    public static int num = 0;
    public static int d1 = 0;
    public static int d2 = 1;
    public static int sum;
    
    
    public static void main(String[] args) {
        
       
        display();
        
           
    }
    public static int user(){
        Scanner sc = new Scanner(System.in);
  
        System.out.println("Please enter the desired ammount number: ");
        num = sc.nextInt();
        
        return num;
        
    }
    public static int display(){
        
        int y = algo(user());
        
        for(int i = 0; i<= y ; i++){
            System.out.print("f["+i+"]\t");    
        }
        
        System.out.println("");
        for(int j = 0; j <=y ; j++){
            for(int k=0;k<=j;k++){
                System.out.print(algo(k)+ "\t");
            }
                System.out.println(" ");
        }
        return y;

    }
    public static int algo(int n){
        if(n <=1){
            return n;
        }else 
            return algo(n-1)+algo(n-2);             
        
    }
    
    
}
             
CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "RECURSIVE SORTING"
  


import java.util.Arrays; 
  
public class JavaApplication  
{ 
    
    static void insertionSortRecursive(int arr[], int n) 
    { 
       
        if (n <= 1) 
            return; 
       
         
        insertionSortRecursive( arr, n-1 ); 
       
     
        int last = arr[n-1]; 
        int j = n-2; 
       
      
        while (j >= 0 && arr[j] > last) 
        { 
            arr[j+1] = arr[j]; 
            j--; 
        } 
        arr[j+1] = last; 
    } 
      
   
    public static void main(String[] args) 
    { 
        int arr[] = {12, 11, 13, 5, 6}; 
       
        insertionSortRecursive(arr, arr.length); 
          
        System.out.println(Arrays.toString(arr)); 
    } 
} 
             
             

CC2 Projects 

1H , FARRO FREDERICK ANTHONY A.

TITLE: "Fibonacci Factorial"
  
  
  
             
