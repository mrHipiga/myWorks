import javax.swing.JOptionPane;
public class HipigaMidterm {
        
    
    public HipigaMidterm() {
    }
  
    
    public static void main(String[] args) {
    	 String choice = "y" ;
   		 double income,tuition = 0,discount=0,a=0;
       int stud=0,stud1=0,stud2=0,stud3=0,stud4=0,stud5=0,stud6=0,nostud=0;
      
       while(choice.equals("y")){
       income = Double.parseDouble(JOptionPane.showInputDialog("Enter MONTHLY FAMILY income"));
       stud=stud+1;
       	
       			 if (income>20000){
       			 JOptionPane.showMessageDialog(null,"Sorry\n The student is not qualified for discount grant");
       			 nostud=nostud+1;
      			 choice = JOptionPane.showInputDialog("Enter another student?[y/n]");
      			 }
       			 
      			 else if ((income<=20000)&&(income>=18000)){
      			 stud1=stud1+1;
       			 tuition = Double.parseDouble(JOptionPane.showInputDialog("Enter Student Total Tuition Fee:"));
       			 discount=tuition*0.15;
       			 a=tuition-discount;
       			 JOptionPane.showMessageDialog(null,"Discount Grant: 15%\n Tuition Fee:"+tuition+"\nDiscount:"+discount+"\nDiscounted Tuition Fee:"+a);
       			 choice = JOptionPane.showInputDialog("Enter another student?[y/n]");
      			 }
      			  else if ((income<=17999)&&(income>=16000)){
      			 stud2=stud2+1;
       			 tuition = Double.parseDouble(JOptionPane.showInputDialog("Enter Student Total Tuition Fee:"));
       			 discount=tuition*0.20;
       			 a=tuition-discount;
       			 JOptionPane.showMessageDialog(null,"Discount Grant: 20%\n Tuition Fee:"+tuition+"\nDiscount:"+discount+"\nDiscounted Tuition Fee:"+a);
       			 choice = JOptionPane.showInputDialog("Enter another student?[y/n]");
      			 }
      			  else if ((income<=15999)&&(income>=14000)){
      			 stud3=stud3+1;
       			 tuition = Double.parseDouble(JOptionPane.showInputDialog("Enter Student Total Tuition Fee:"));
       			 discount=tuition*0.25;
       			 a=tuition-discount;
       			 JOptionPane.showMessageDialog(null,"Discount Grant: 25%\n Tuition Fee:"+tuition+"\nDiscount:"+discount+"\nDiscounted Tuition Fee:"+a);
       			 choice = JOptionPane.showInputDialog("Enter another student?[y/n]");
      			 }
      			  else if ((income<=13999)&&(income>=12000)){
      			 stud4=stud4+1;
       			 tuition = Double.parseDouble(JOptionPane.showInputDialog("Enter Student Total Tuition Fee:"));
       			 discount=tuition*0.30;
       			 a=tuition-discount;
       			 JOptionPane.showMessageDialog(null,"Discount Grant: 30%\n Tuition Fee:"+tuition+"\nDiscount:"+discount+"\nDiscounted Tuition Fee:"+a);
       			 choice = JOptionPane.showInputDialog("Enter another student?[y/n]");
      			 }
      			  else if ((income<=11900)&&(income>=10000)){
      			 stud5=stud5+1;
       			 tuition = Double.parseDouble(JOptionPane.showInputDialog("Enter Student Total Tuition Fee:"));
       			 discount=tuition*0.35;
       			 a=tuition-discount;
       			 JOptionPane.showMessageDialog(null,"Discount Grant: 35%\n Tuition Fee:"+tuition+"\nDiscount:"+discount+"\nDiscounted Tuition Fee:"+a);
       			 choice = JOptionPane.showInputDialog("Enter another student?[y/n]");
      			 }
      			  else if (income<10000){
      			 stud6=stud6+1;
       			 tuition = Double.parseDouble(JOptionPane.showInputDialog("Enter Student Total Tuition Fee:"));
       			 discount=tuition*0.40;
       			 a=tuition-discount;
       			 JOptionPane.showMessageDialog(null,"Discount Grant: 40%\n Tuition Fee:"+tuition+"\nDiscount:"+discount+"\nDiscounted Tuition Fee:"+a);
       			 choice = JOptionPane.showInputDialog("Enter another student?[y/n]");
      			 }
       			
       			
       			 
       }
      
      JOptionPane.showMessageDialog(null,"Discount tuition summary:\n No.of students:"+stud+"\nNo. of students not discounted:"+nostud+"\nNo.of students with Discount:\n40%= "+stud6+"\n35%= "+stud5+"\n30%= "+stud4+"\n25%= "+stud3+"\n20%= "+stud2+"\n15%= "+stud1); 
       
       
    }
}
