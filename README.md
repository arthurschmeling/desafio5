package javaapplication77;


import java.text.DecimalFormat;
import java.util.Scanner;


public class JavaApplication77 {

   
    public static void main(String[] args) {
       Scanner ler= new Scanner(System.in);
       DecimalFormat decimal = new DecimalFormat("0.00");
       //variaveis//
       int contador, numero,par, impar, nulo;
       //processamento//
       contador=0;
       nulo=0;
       par=0;
       impar= 0;
       
       //saida//

        while (contador<30){
            System.out.println("Insira o número:");
            numero = ler.nextInt();
            if (numero ==0){
               nulo++;
               
                
            }else if (numero % 2 == 0){
                par++;
                
            }else{
                impar++;
            }
            contador++;
        }
        System.out.println("resultados:");
        System.out.println("pares: "+par);
        System.out.println("impar: "+impar);
        System.out.println("nulo:"+nulo);

    }
   
}
