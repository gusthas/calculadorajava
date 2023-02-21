# calculadorajava
calculadora basica em java.
---------------------------------------------------------------------------------------------------------------------------------------------------------
package com.mycompany.mavenproject1;

import java.util.Scanner;

public class Mavenproject1 {

    public static void main(String[] args) {
       Scanner cal= new Scanner(System.in);
       System.out.println("digite o primeiro valor");
       float A= cal.nextFloat();
       System.out.println("Digite o segundo valor");
       float B=cal.nextFloat();
       System.out.println("Digite a operação:\n + \n - \n * \n /");
       String  C=cal.next();
       if(null == C){
           System.out.println("operação invalida");
       }else switch (C) {
            case "+":
                {
                    float D= A+B;
                    System.out.print("O resultado é:"+ D);
                    break;
                }
            case "-":
                {
                    float D= A-B;
                    System.out.print("O resultado é:"+D);
                    break;
                }
            case "*":
                {
                    float D= A*B;
                    System.out.println("O resultado é:"+ D);
                    break;
                }
            default:
                System.out.println("operação invalida");
                break;
        }

    }
}
