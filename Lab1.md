# melekabdullaieva1lab
package lab1;

import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;
public class lab
{
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String[] arr=new String[5];
        int lenthSum=0;
        for(int i=0;i<arr.length;i++) {
            arr[i]=sc.nextLine();
            lenthSum+=arr[i].length();
        }
        int average=lenthSum/arr.length;
        List<String> bigger=new ArrayList();
        List<String> smoller=new ArrayList();
        for(int i=0;i<arr.length;i++) {
            if(arr[i].length()>average) {
                bigger.add(arr[i]);
            }else {
                smoller.add(arr[i]);
            }
        }
        System.out.print("Smaller\n");
        smoller.forEach(System.out::println);
        System.out.print("Bigger\n");
        bigger.forEach(System.out::println);
    }
}




