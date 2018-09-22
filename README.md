import java.util.Scanner;

/**
 *
 * @author Javier Octavio
 */
public class Principal {


    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner input = new Scanner(System.in);
        System.out.println("¿Qué calificación obtuviste?");
        double rCalifa;
        rCalifa = input.nextDouble();
        
        while (rCalifa >= 100) {
            System.out.println("Syntax ERROR");
            rCalifa = input.nextDouble();
        }
        if (rCalifa >= 70) {
            System.out.print("Tu calificación es: ");
            System.out.println(rCalifa);
            System.out.println("PASASTE");
        } else {
            System.out.println("Tu calificación es 0");
            System.out.println("Lo Bueno es que hay Salud");
        }
    }
}
