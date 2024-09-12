import java.util.Scanner;

public class EvaluacionUsuario {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Capturar datos del usuario
        System.out.print("Ingrese su nombre: ");
        String nombre = scanner.nextLine();

        System.out.print("Ingrese su edad (en años): ");
        int edad = scanner.nextInt();

        System.out.print("Ingrese su altura (en metros): ");
        double altura = scanner.nextDouble();

        System.out.print("¿Es estudiante? (true/false): ");
        boolean esEstudiante = scanner.nextBoolean();

        // Evaluar datos
        boolean esMayorDeEdad = edad >= 18;
        boolean esAlto = altura >= 1.75;

        // Imprimir resultados
        System.out.println("\nResultados:");
        System.out.println("Eres " + (esMayorDeEdad ? "mayor" : "menor") + " de edad.");
        System.out.println("Eres " + (esAlto ? "alto" : "bajo") + ".");
        System.out.println("Eres " + (esEstudiante ? "" : "no ") + "estudiante.");

        // Imprimir resumen
        System.out.println("\nResumen:");
        System.out.println("Nombre: " + nombre);
        System.out.println("Edad: " + edad + " años");
        System.out.println("Altura: " + altura + " metros");
        System.out.println("Estudiante: " + esEstudiante);
    }
}
