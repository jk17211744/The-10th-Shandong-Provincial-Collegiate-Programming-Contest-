```
import java.util.*;
import java.math.*;
public class Main {
		static int a = 10;
        public static void main(String[] args) {
             Scanner cin = new Scanner(System.in);
             int T = cin.nextInt();
             for(int i = 0;i < T;i++)
             {
            	 int a,b,c,d = 0;
            	 String s;
            	 a = cin.nextInt();
            	 b = cin.nextInt();
            	 c = cin.nextInt();
            	 s = cin.next();
            	 switch(s)
            	 {
            	 	case  "Monday": d = 1;break;
            	 	case  "Tuesday": d = 2;break;
            	 	case  "Wednesday": d = 3;break;
            	 	case  "Thursday": d = 4;break;
            	 	case  "Friday": d = 5;break;
            	 }
            	 int x,y,z;
            	 x = cin.nextInt();
            	 y = cin.nextInt();
            	 z = cin.nextInt();
            	 int ans = b * 30 % 5 - c % 5 + y * 30 % 5 + z % 5;
            	 if(ans < 0)
            		 ans += 5;
            	 ans += d;
            	 ans %= 5;
            	 switch(ans)
            	 {
            	 	case  1:System.out.println("Monday");break;
            	 	case  2:System.out.println("Tuesday");break;
            	 	case  3:System.out.println("Wednesday");break;
            	 	case  4:System.out.println("Thursday");break;
            	 	case  0:System.out.println("Friday");break;
            	 }
             } 
         }  
}
```