/*      Take Integer N as input and print the following pattern :-

 "Sample Input"                      "Sample Output"
  5                                         *
                                           * *
                                          * * *
                                         * * * *
                                        * * * * *
                                         * * * *
                                          * * *
                                           * *
                                            *
*/



import java.util.*;
import java.io.*;

public class Main {
    public static void main(String[] args) {
Scanner asd= new Scanner(System.in);
            int n = asd.nextInt();
            int nsp = n-1, nst = 1;
            int np = 1, nt = n-1;
            
            for (int row = 1; row <= n; row++){
                    for (int sp = 1; sp <= nsp; sp++){
                            System.out.print(" ");
                    }
                    for (int st = 1; st <= nst; st++){
                            System.out.print("* ");
                    }
                    nsp--; nst++;
                    System.out.println();
            }
            
            for (int row = n-1; row >= 1; row--){
                for (int sp = 1; sp <= np; sp++){
                            System.out.print(" ");
                    }
                    for (int st = nt; st >= 1; st--){
                            System.out.print("* ");
                    }
                    np++;  nt--;
                    System.out.println();
            }
    }
}
