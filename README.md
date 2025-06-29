# CalculadoraBasica
//Importe de Classe Scanner para leitura de entrada de user
import java.util.Scanner;

import static java.util.Scanner.*;

//Classe principal, CalculadoraBasica
public class Main {
    //Método principal do código; "caixinha de recados" inicio da execução do programa
    public static void main(String[] args) {
        //criado objeto Scanner
        Scanner teclado = new Scanner(System.in);

        double numero1;
        double numero2;
        char operacao;
        double resultado = 0;

        System.out.println("Bem vindos a calculadora da putaria!");

        System.out.println("Digite o Primeiro numero seu puto:");
        numero1 = teclado.nextDouble();

        System.out.println("Escolha a Operação seu saco de merda(+,-,/,*): ");
        operacao = (char) teclado.next().charAt(0);

        System.out.println("Digite o Segundo numero seu merda:");
        numero2 = teclado.nextDouble();


        switch (operacao) {

            case '+':
                resultado = numero1 + numero2;
                System.out.println("Resultado da Operação do Corno do Usuário:");
                break;// Break serve para sair do switch(operação)

            case '-':
                resultado = numero1 - numero2;
                System.out.println("Resultado da Operação do Corno do Usuário:");
                break;

            case '*':
                resultado = numero1 * numero2;
                System.out.println("Resultado da Operação do Corno do Usuário:");
                break;

            case '/':
                resultado = numero1 / numero2;
                if (numero2 != 0) {
                    resultado = numero1 / numero2;
                } else {
                    System.out.println("A operação é invalida seu imbecil, Divisão por zero não é permitida seu puto!");
                    teclado.close();
                    return; //encerramento do metodo main
                }

            }

        System.out.println("O resultado da operação seu grande Filho da Puta é:" + resultado);

        teclado.close();
        }
}
