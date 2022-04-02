# Write-a-program-that-allows-the-user-to-enter-5-codes-store-these-5-codes-in-an-array.
Write a program that allows the user to enter 5 codes, store these 5 codes in an array.
import java.util.Scanner;
public class BaiTapJavaCoBan15
{
    public static void main(String[] args)
    {
       String[] code = new String[5];
       Scanner sc = new Scanner(System.in);

       for (int i = 0; i < 5; i++)
       {
          System.out.println("Enter th code " + (i+1));
          code[i] = sc.nextLine();
          if(!code[i].matches("00[2-5]L\\d{4}"))
          {
             System.out.println("Wrong!");
             return;
          }
       }
       System.out.println("That's right!");
    }
}
