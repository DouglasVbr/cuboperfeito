# cuboperfeito


package cuboperfeito;

import java.util.Scanner;

public class CuboPerfeito {

   
    public static void main(String[] args) {
     
    Scanner Scanner = new Scanner (System.in);
//Solicita ao usuario que insira um número
System.out.println("Digite um número inteiro positivo.");
int numero = Scanner.nextInt();
//verifica se o número é um cubo perfeito
boolean ehcuboperfeito=false;
if(numero>=0){
    int raizcubica= (int) Math.cbrt(numero);
  ehcuboperfeito = raizcubica*raizcubica*raizcubica==numero;
  }

// exibe o resultado

if(ehcuboperfeito){
    System.out.println(numero + " é um cubo perfeito.");
}else{
    System.out.println(numero + "não é um cubo perfeito.");
    
}
    //fecha o Scanner
Scanner.close();
    }
    
}
