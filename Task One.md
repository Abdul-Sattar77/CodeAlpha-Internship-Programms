Task by CodeAlpha a program that allows a teacher to enter
students' grades and compute their average,
highest, and lowest scores.

import java.util.Scanner;

public class CodeAlphaTaskOne {
    int eng,math,it,java;

    void Average(){
        System.out.println("Average : "+(eng+math+it+java)/4);
    }
    void highestScore(){
        if(eng>math && eng>it && eng >java){
            System.out.println("Highest marks are in English : "+eng);
        }else if(math >eng && math>it && math>java){
            System.out.println("Highest marks are in Maths : "+math);
        }else if(it>eng && it>math && it>java){
            System.out.println("Highest marks are in IT : "+it);
        }else {
            System.out.println("Highest marks are in Java : "+java);
        }
    }
    void LowestScore(){
        if(eng<math && eng<it && eng <java){
            System.out.println("Lowest marks are in English : "+eng);
        }else if(math <eng && math<it && math<java){
            System.out.println("Lowest marks are in Maths : "+math);
        }else if(it<eng && it<math && it<java){
            System.out.println("Lowest marks are in IT : "+it);
        }else {
            System.out.println("Lowest marks are in Java : "+java);
        }
    }
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);


        CodeAlphaTaskOne student1 = new CodeAlphaTaskOne();
        System.out.print("Enter English Marks : ");
        student1.eng = input.nextInt();
        System.out.print("Enter Maths Marks : ");
        student1.math = input.nextInt();
        System.out.print("Enter IT Marks : ");
        student1.it = input.nextInt();
        System.out.print("Enter Java Marks : ");
        student1.java = input.nextInt();

        student1.Average();
        student1.highestScore();
        student1.LowestScore();
    }
}
