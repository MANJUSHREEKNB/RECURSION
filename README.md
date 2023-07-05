# RECURSION
//Factorial of a NumbeR
//SOURCE CODE

import java.io.*;
import java.util.*;
public class Solution {
    public static void main(String[] args) {
        Scanner sc=new Scanner (System.in);
        int n=sc.nextInt();
        System.out.println("The factorial of "+n+" is "+fact(n));
    }
    public static int fact(int n) {
        if(n<1)
            return 1;
        return n*fact(n-1);
    }
}

//Number of digits
//SOURCE CODE

import java.io.*;
import java.util.*;
public class Solution {
    public static void main(String[] args) {
        Scanner sc=new Scanner (System.in);
        int n=sc.nextInt();
        int count=countdigit(n);
        System.out.println("The number of digits in "+n+" is "+count);
    }
    public static int countdigit(int n) {
        int temp=0;
        if(n<9)
            return 1;
        temp++;
        return temp+countdigit(n/10);
    }
}

//Sum of Array Elements
//SOURCE CODE

import java.util.Scanner;
public class Main {
public static int sum(int[] a, int n) {
    if (n <= 0) 
        return 0;
    return (sum(a, n - 1) + a[n - 1]);
    }
public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    int n = sc.nextInt();
    int[] a = new int[n];
    for (int i = 0; i < n; i++)
        a[i] = sc.nextInt();
    System.out.println(sum(a, n));    
    }
}
