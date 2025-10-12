# Práctica programada 1

Mayquelin

package com.mycompany.inverso.java;

import java.util.Scanner;


public class InversoJava {
    int numInvertido(int num, int invert){
        if (num>0){
        return numInvertido (num/10, num%10+invert*10);
        }
        else{
        return invert;
        
        }
    }
    public static void main(String[] args) {
        InversoJava numInver = new InversoJava();
        Scanner sc= new Scanner(System.in);
        int num, inver = 0;
        System.out.print("Ingresar numero: ");
        num = sc.nextInt();
        System.out.print("Número invertido: " + numInver.numInvertido(num,inver));
      
    }
   
}
