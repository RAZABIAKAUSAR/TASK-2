# TASK-2
import java.util.*;
public class Guessinggame {
    public static int playgame(){
        Scanner sc=new Scanner(System.in);
        int guessed;
        int rand=(int)Math.random();
        int rd= (rand*10)+1;
        int attempt=0;boolean win=false;
        while(win==false){
            System.out.println("Enter your guess value ");
            guessed=sc.nextInt();
            attempt++;
        if(guessed==rd){
            win=true;
        }
        else if(guessed<rd){
            System.out.println("enterd value is greater than the exact");
         }
        else if(guessed>rd){
         
            System.out.println("enterd value is less than the exact "+rd);
         }
        }
        System.out.println("Cong! you have won totalattempt"+" "+ attempt +" "+"correct value is"+" "+rd);
        return attempt;
    }
    public static void main(String[] args) {
        playgame();
    }
}
