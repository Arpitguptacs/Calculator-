import java.util.*;
public class Calculator{
    
       
     public static double divide(double num_1, double num_2){
          
            return num_1/num_2;
           
           
    }

    public static double multiply (double num_1, double num_2){

           return num_1*num_2;
    }

     public static double subtraction (int num_1, int num_2){
          
            return num_1-num_2;
         
    }



    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);

        int nums_1 = sc.nextInt();

        
        char symbol = sc.next().charAt(0);

        int nums_2 = sc.nextInt();

         if(nums_1==0 && symbol == '+'){
              System.out.println(nums_2);
         }else if(nums_2==0 && symbol=='+'){
              System.out.println(nums_1);
         }
        switch(symbol){

            case '+': System.out.println(nums_1 + nums_2);
            break;  
            case '-': System.out.println(subtraction(nums_1, nums_2));
            break;
            case 'x' : System.out.println(multiply(nums_1, nums_2));
            break;
            case '/' : System.out.println(divide(nums_1, nums_2));
            break;
            default : System.out.println("Opperation is not possible");

        }

      sc.close();
    } 
}
