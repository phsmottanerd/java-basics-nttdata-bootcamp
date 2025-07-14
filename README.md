import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        var value1 = -12;
        var binary1 = Integer.toBinaryString(value1);
        System.out.printf("Primeiro número da operação %s (representação binária %s)\n", value1, binary1);

        var value2 = 2;
        var binary2 = Integer.toBinaryString(value2);
        System.out.printf("Segundo número da operação %s (representação binária %s)\n", value2, binary2);
        var result = value1 >>> value2;
        var binaryResult = Integer.toBinaryString(result);
        result = ~value1;
        System.out.printf(" ~%s | %s  = %s (representação binária %s)\n", value1, value2, result, binaryResult);
        System.out.println(Integer.toBinaryString((Integer.MAX_VALUE)));
    }

    /*
     0 = false
     1 = true
    */

}

// Exercícios
/*
 1.Escreva um código  que recaba o nome e o ano de nascimento e impreima na tela aseguinte menssagem:"oláFulano 'você tem 'X' anos"

2. escreva um código que receba o tamanho   do lado de um quadrado ,e calacule sua áreae exiba na tela.
Fórmula:área =lado=lado X lado

3.Escreva um còdigo que receba a base e a alturade um retângulo ,calcule sua área eexiba na tela.
fórmula:área=base X altura

4. Escreva um código que receba o nome ea idade de 2 pessoas e imprima a diferença de idade de entre elas
*/


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        var baseYear = 2024;
        var scanner = new Scanner(System.in);
        System.out.println("Informe o seu nome:");
        var name = scanner.next();
        System.out.println("Informe o seu ano de nascimento:");
        var year = scanner.nextInt();
        var age = baseYear - year;
        System.out.printf("Olá %s você tem %d anos\n", name, age);
    }
}




import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        var scanner = new Scanner(System.in);

        System.out.print("Digite otamanho do lado do quadrado:");
        var lado = scanner.nextDouble();

        var area = lado * lado;
        System.out.printf("A área do quadrado é %,.2f\n", area);

    }
}




import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        var scanner = new Scanner(System.in);

        System.out.print("Digite o valor da base do retângulo:");
        var base = scanner.nextDouble();

        System.out.print("Digite o valor da altura do retângulo: ");
        var altura = scanner.nextDouble();

        var area = base * altura;

        System.out.printf("A área do retângulo é :%.2f\n", area);

    }
}




import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        var scanner = new Scanner(System.in);

        System.out.print("Digite o nome da primeira pessoa: ");
        var nome1 = scanner.nextLine();

        System.out.print("Digite a idade da primeira pessoa: ");
        var idade1 = scanner.nextInt();
        scanner.nextLine();

        System.out.print("Digite o nome da segunda pessoa: ");
        var nome2 = scanner.nextLine();

        System.out.print("Digite a idade da segunda pessoa: ");
        var idade2 = scanner.nextInt();

        var diferenca = Math.abs(idade1 - idade2);

        System.out.printf("A diferença de idade entre %s e %s é de %d anos.\n", nome1, nome2, diferenca);
    }
}
