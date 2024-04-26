# Ice-Task-4
import java.util.*;
import java.util.Random;
import javax.swing.JOptionPane;
import javax.swing.JFrame;

/**
 *
 * @author ST10177832
 */
public class Task2 {
    int option;
    String task;
    String aa;
    String bb;
    int cc;
    String dd;
    String ee;
    String ff;
    
    public void setaa(String aa){
        this.aa = aa;
    }
    public String getaa(){
        return aa;
    }
    public void setbb(String bb){
        this.bb = bb;
    }
    public String getbb(){
        return bb;
    }
    public void setaa(int cc){
        this.cc = cc;
    }
    public int getcc(){
        return cc;
    }
    public void setdd(String dd){
        this.dd = dd;
    }
    public String getdd(){
        return dd;
    }
    public void setee(String ee){
        this.ee = ee;
    }
    public String getee(){
        return ee;
    }
    public void setff(String ff){
        this.ff = ff;
    }
    public String getff(){
        return ff;
    }
            
    
    
    
    

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner check = new Scanner(System.in);
        Task2 aaa = new Task2();
        
            JFrame show = new JFrame();
            String found = "W";
            Random get = new Random();
            int x = get.nextInt(99)+10;
            
    do{
        int option = Integer.parseInt(JOptionPane.showInputDialog(show, "Welcome to EasyKanBan" + "\n" + "Choose one of the following features from the menu given below" + "\n" + "Option 1 - Add task" + "\n" + "Option 2 - Show report" + "\n" + "Option 3 - Quit"));
        
        
        if(option == 1){
            System.out.println("Hello, enter the number of tasks you want to do");
            String task = check.next();
            System.out.println("Please enter task name");
            
            String aa = check.next();
            aaa.setaa(aa);
            aaa.getaa();
            System.out.println("Please enter task number");
            int cc = check.nextInt();
            
            System.out.println("Please enter task description");
            String bb = check.next();
            aaa.setbb(bb);
            aaa.getbb();
            
            System.out.println("Please enter developer details");
            String dd = check.next();
            aaa.setdd(dd);
            aaa.getdd();
            
            System.out.println("Please enter task duration: ");
            String ee = check.next();
            aaa.setee(ee);
            aaa.getee();
            
            System.out.println("Please enter task ID: " + get.nextInt(99)+10 + "\n");
            
             System.out.println("Please enter task status: ");
            String ff = check.next();
            aaa.setff(ff);
            aaa.getff();
        }else if(option == 2){
            System.out.println("Coming soon");
            
        }else if(option == 3){
            System.exit(option);
        }
        JOptionPane.showMessageDialog(show, ' ' + "Task Name: " + aaa.aa + "\n" + "Task Number: " + aaa.cc + "\n" + "Task Description: " + aaa.bb + "\n" + "Developer Details: " + aaa.dd + "\n" + "Task Duration: " + aaa.ee + "\n" + "Task ID: " + get.nextInt(99)+10 + "\n" + "Task Status: " + aaa.ff);
        
        found = JOptionPane.showInputDialog(show,"do you wish to exit application? Enter(W) continue" );
    }while(found.equals("W"));
    }
    
}
