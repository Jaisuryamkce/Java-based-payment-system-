# Java-based-payment-system-
Basic payment system in java

import java.util.*; 
class Main{ 
static void Sign() { 
 Scanner obj=new Scanner(System.in); 
 System.out.println(" Welcome to International Bank "); 
 System.out.println(" sign up "); 
 System.out.println("Username: "); 
 String user_name=obj.nextLine(); 
 System.out.println("Password:"); 
 String pass_word=obj.nextLine(); 
 System.out.println(user_name); 
 System.out.println(pass_word); 
 System.out.println("😍Your account is Created Successfully😍"); 
 
 } 
 static void DTH_Recharge(){ 
 System.out.println("New recharge......"); 
 System.out.println(" Dish_TV d2h Tata_Play Airtel_Digital_TV Sun_Direct"); 
 System.out.println("Enter Your Favorite ! "); 
 Scanner objecc=new Scanner(System.in); 
 String dth=objecc.nextLine(); 
 System.out.println(" Your Favorite*"); 
 System.out.println(dth); 
 System.out.println(" Subscriber Id: "); 
 int sub_id=objecc.nextInt(); 
 System.out.println(" Payable amount :"); 
 int sub_amt=objecc.nextInt(); 
 
System.out.println("__________________________________________________________________________
__________________________"); 
 System.out.println(" Subscriber Id: "+sub_id); 
 System.out.println(" Payable amount :"+sub_amt); 
 
System.out.println("__________________________________________________________________________
__________________________"); 
 System.out.println(" Enter UPI pin :---- "); 
 int upi=objecc.nextInt(); 
 int upi_pin=2021; 
 double ban_amt=5025.00; 
 
 
 System.out.println(" "); 
 if(upi_pin==upi) 
 { 
 System.out.println("Wait for Payment Status**"); 
 System.out.println("Payment Successfully"); 
 System.out.println("Do you want to CheckbankBalance_if_Enter-1"); 
 int e1=objecc.nextInt(); 
 if(e1==1){ 
 System.out.println("Current Balance:₨.₹"+(ban_amt-sub_amt)); 
 } 
 
 } 
 else{ 
 System.out.println("Enter Valid UPI pin"); 
 System.out.println(" Forget UPI "); 
 } 
 } 
 
 static void Moblie_Recharge(){ 
 System.out.println("New recharge......"); 
 System.out.println(" Jio VI Airtel BSNL_India"); 
 System.out.println("Enter Your Favorite NEtwork ! "); 
 Scanner objee=new Scanner(System.in); 
 String m_re=objee.nextLine(); 
 System.out.println(" Your Favorite*"); 
 System.out.println(m_re); 
 System.out.println(" Moblie: "); 
 String m_num=objee.nextLine(); 
 System.out.println(" Payable amount :"); 
 int m_amt=objee.nextInt(); 
 
System.out.println("__________________________________________________________________________
__________________________"); 
 System.out.println(" Subscriber Id: "+m_num); 
 System.out.println(" Payable amount :"+m_amt); 
 
System.out.println("__________________________________________________________________________
__________________________"); 
 System.out.println(" Enter UPI pin :---- "); 
 
 int upi=objee.nextInt(); 
 int upi_pin=2021; 
 double ban_amt=5025.00; 
 
 
 System.out.println(" "); 
 if(upi_pin==upi) 
 { 
 System.out.println("Wait for Payment Status**"); 
 System.out.println("Payment Successfully"); 
 System.out.println("Do you want to CheckbankBalance_if_Enter-1"); 
 int e2=objee.nextInt(); 
 if(e2==1) 
 { 
 System.out.println("Current Balance:₨.₹"+(ban_amt-m_amt)); 
 } 
 
 } 
 else{ 
 System.out.println("Enter Valid UPI pin");System.out.println(" Forget UPI "); 
 } 
 
 } 
 
 static void Payment(){ 
 
 System.out.println(" Payment "); 
 
 System.out.println(" DTH_Recharge-1 ** Moblie_Recharge-2 ** "); 
 Scanner obj=new Scanner(System.in); 
 System.out.println(" Select your Paymentway"); 
 int paych=obj.nextInt(); 
 switch(paych) 
 { 
 case 1: 
 DTH_Recharge(); 
 break; 
 case 2: 
 Moblie_Recharge(); 
 break; 
 
 default: 
 System.out.println("Sorry Something went wrong"); 
 System.out.println(" Try later "); 
 break; 
 } 
 } 
 static void CheckbankBalance(){ 
 
 System.out.println(" CheckbankBalance "); 
 System.out.println(" Enter UPI pin :---- "); 
 Scanner objec=new Scanner(System.in); 
 int upi=objec.nextInt(); 
 int upi_pin=2021; 
 double bank_amt=5025.00; 
 System.out.println("Loading....."); 
 System.out.println("Fetched...✨"); 
 
 System.out.println(" "); 
 if(upi_pin==upi) 
 { 
 System.out.println("Your bank balance is:₨.₹"+bank_amt); 
 
 } 
 else{ 
 System.out.println("Enter Valid UPI pin"); 
 System.out.println(" Forget UPI "); 
 } 
 } 
 static void login_sucess(){ 
 int wh=1; 
 while(wh==1){System.out.println(" CheckbankBalance-1 ** Payment-2 "); 
 Scanner obj=new Scanner(System.in); 
 int in=obj.nextInt(); 
 switch(in) 
 { 
 case 1: 
 CheckbankBalance(); 
 break; 
 case 2: 
 Payment(); 
 break; 
 
 default: 
 System.out.println("Sorry Something went wrong"); 
 System.out.println(" Try later "); 
 break; 
 } 
 } 
 } 
 public static void Login() 
 { 
 Scanner obj=new Scanner(System.in); 
 String user_na="admin"; 
 String pass_w="adminpass"; 
 System.out.println(" Welcome to International Bank "); 
 System.out.println(" Login "); 
 System.out.println("Username: "); 
 String user=obj.nextLine(); 
 System.out.println("Password:"); 
 String pass=obj.nextLine(); 
 if(user_na.compareTo(user)==0&&pass_w.compareTo(pass)==0){ 
 System.out.println(" "+"Profile 🙂"); 
 System.out.println(" "+" Id :"+user); 
 System.out.println(" "+" Settings "); 
 login_sucess(); 
 } 
 else 
 { 
 System.out.println("wrong username &password"); 
 } 
 } 
 
 public static void main(String[] args) { 
 System.out.println(" *IB* "); 
 System.out.println(" Welcome to International Bank "); 
 System.out.print(" Login || "); 
 System.out.print(" sign up "); 
 System.out.println(" "); 
 System.out.println(" Login-1 ***** signup-2 "); 
 System.out.println(" "); 
 Scanner ob=new Scanner(System.in); 
 int ch=ob.nextInt();switch(ch) 
 { 
 case 1: 
 Login(); 
 break; 
 case 2: 
 Sign(); 
 break; 
 default: 
 System.out.println("Sorry Something went wrong"); 
 System.out.println(" Try later "); 
 break; 
 
 } 
 
 } 
}
