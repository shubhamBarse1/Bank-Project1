import java.util.Scanner;
public class account {
	
	account(){
       System.out.println("Welcome to the SBI ATM");
       System.out.println("Please insert your ATM card");
       System.out.println("To witdraw press  = 1");
       System.out.println("To deposite press = 2"); 
       System.out.println("To check balance press = 3");
       }
	
	 private static int ass = 10000;
	 
	
		
	
      void main2() {
    	  for(;;) {
	  Scanner sc = new Scanner(System.in);
	    int SS= sc.nextInt();
	 
	    switch(SS) 
	   {
	   
	   case(1):
	   Scanner S1= new Scanner(System.in);
	   System.out.println("Enter your PIN");
	   Scanner V1= new Scanner(System.in);
	   int D1= V1.nextInt();
	   if(D1==1234)
	   {
	   System.out.println("enter withdraw amount");
	   int F1= S1.nextInt();
	   int withdraw =  ass - F1;
	   System.out.println("your are current balance is "+ withdraw);
	   break;
	   }
	    case(2):
	   System.out.println("Enter your PIN");
	   Scanner V2= new Scanner(System.in);
	   int D2= V2.nextInt();
	   if(D2==1234)
	   {
	     Scanner S2= new Scanner(System.in);
	   System.out.println("enter Deposite  amount");
	   int F2= S2.nextInt();
	   int Deposite =ass+F2;
	   System.out.println("your are current balance is "+ Deposite);
	   break;
	   }
	   
	   case(3):
		   System.out.println("Enter your PIN");
	   Scanner V3= new Scanner(System.in);
	   int D3= V3.nextInt();
	   if(D3==1234)
	   {
		System.out.println("CHECKING BALANCE");
	    System.out.println("your current  balance is"+ass);
	   break;
	   }
	    
	   default:
	   System.out.println("INVALID CRADENTIAL");
	   
	   }
	   
	    System.out.println("THANK YOU....");  
	    System.out.println("Welcome to the SBI ATM");
	       System.out.println("Please insert your ATM card");
	       System.out.println("To witdraw press  = 1");
	       System.out.println("To deposite press = 2"); 
	       System.out.println("To check balance press = 3");   
	   }
      }
	
	 public static void main(String[] args) {
		 account c = new account();
		 c.main2();
	 		
	}
		
	}

