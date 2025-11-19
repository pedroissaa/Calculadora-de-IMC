# Calculadora-de-IMC
Estudo feito para entender o funcionamento das variáveis em Java

import java.util.Scanner;
public class CALCULANDOIMC {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite o nome: ");
        String nome = sc.nextLine();

        System.out.print("Digite a idade: ");
        int idade = sc.nextInt();

        System.out.print("Digite o peso: ");
        float peso = sc.nextFloat();

        System.out.print("Digite a altura: ");
        float altura = sc.nextFloat();

        pessoa pes = new pessoa(nome, idade, peso, altura);
        float imc = pes.getPeso() / (pes.getAltura() * pes.getAltura());
        System.out.println("O IMC de " + pes.getNome() + " é: " + imc);
   
    }
}
