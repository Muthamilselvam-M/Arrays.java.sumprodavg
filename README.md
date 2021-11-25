# Arrays.java.sumprodavg



import java.awt.*;
import java.util.Arrays;
import java.util.Scanner;
public class Main{
    public static void main(String[] args){
        Scanner a = new Scanner(System.in);
        System.out.print("Enter the array size:");
        int input = a.nextInt();
        int[] number = new int[input];
        System.out.println("Enter the array elements:");
        for(int i=0;i<input;i++){
        int number1 = a.nextInt();
        number[i]=number1;
            
        }
        System.out.println(Arrays.toString(number));
        sum(number);
        product(number);
        average(number);
        
    

    }
    public static void sum(int[] number){
        int sum=0;
        for(int i=0;i<number.length;i++){
            sum+=number[i];}
            System.out.println("The sum is: "+sum);
    }
    public static void product(int[] number){
        int product=1;
        for(int i=0;i<number.length;i++){
            product = product*number[i];
            
        }
        System.out.println("The product is: "+product);
    }
    public static void average(int[] number){
        int average=0;
        for(int i=0;i<number.length;i++){
            average +=number[i];
        }
        average= average/number.length;
        System.out.print("The average is: "+average);
    }
}
