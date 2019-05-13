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
            	 int n = cin.nextInt();
            	 int m = cin.nextInt();
            	 for(int j = 0;j < m;j++)
            		 if(n <= 1)
            			 break;
            		 else
            			 n -= n / 2;
            	 System.out.println(n);
             }
         }  
}
```