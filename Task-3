import java.io.*;
import java.util.*;
public class Atm_Machine
{
   private static int PIN=2005;
   static int balance,choice;
    public static void main(String args[])
    {
        int attempt=3;
        Scanner scanner=new Scanner(System.in);
        for(attempt=0;attempt<3; attempt++)
        {
            System.out.print("Enter your Pin(attempt"+(attempt+1)+"):");
            PIN=scanner.nextInt();
            if(PIN==2005)
            {
                attempt=3;
                System.out.println("Hello! Welcome to use Atm Machine");
        boolean Exit=false;
        while(!Exit)
        {
            System.out.println("***ATM Interface***");
        System.out.println("1.Check Balance\n2.Deposit\n3.Withdraw\n4.Exit");
        Scanner s=new Scanner(System.in);
        System.out.print("Enter your choice:");
        choice=s.nextInt();
          switch(choice)
        {
            case 1:
                Checkbalance();
                break;
            case 2:
                Deposit();
                break;
            case 3:
                Withdraw();
                break;
            case 4:
                Exit=true;
                System.out.println("Thanks for using Atm Machine");
                break;
            default:
            System.out.println("Invalid option!Try again.");
        }
        }
            }
            else
            {
                System.out.println("Incorrect Pin!Please try again.");
            }
            if(attempt==2)
            {
                System.out.println("You reached maximun attempts!Try after sometime.");
            }
        }
    }
    private static void Checkbalance()
        {
            System.out.println("Current Balance:Rs."+balance);
        }
    private static void Deposit()
    {
        Scanner s=new Scanner(System.in);
        System.out.print("Enter the amount to be deposited:Rs.");
        int amount=s.nextInt();
        balance=balance+amount;
        System.out.println("Amount Deposited Successfully...");
    }
    private static void Withdraw()
    {
        Scanner s=new Scanner(System.in);
        System.out.print("Enter the Amount to be withdraw:");
        int amount=s.nextInt();
        if(amount<balance)
        {
            balance=balance-amount;
            System.out.println("Withdrawal of Rs."+(amount)+" is done Successfully....");
        }
        else
        {
            System.out.println("Insufficient balance!Please check your balance");
        }
    }
}
