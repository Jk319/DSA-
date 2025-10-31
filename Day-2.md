brute

import java.util.*;
 class Main {
    public static void main(String[] args){
        int n = 5;
        int[] a = {1,2,3,4,5};
        int[] result = getSecondOrderElements(n,a);
        System.out.println(result[0]);
         System.out.println(result[1]);
    }
    public static int[] getSecondOrderElements(int n, int []a) {
        Arrays.sort(a);
        int s = a[1];
       int l = a[n-2];
       return new int[]{l,s};
    }
}
