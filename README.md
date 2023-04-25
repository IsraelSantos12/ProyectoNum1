import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        double monto;
        double montoReal = 0;
        String nombre, membrecia;
        Scanner sc = new Scanner(System.in);

        System.out.print(" Ingresa Tu Nombre Completo :  \t ");
        nombre = sc.nextLine();

        System.out.print(" Ingresa Tu Membrecia :  \t ");
        membrecia = sc.nextLine();

        System.out.print(" Ingresa El Monto De tu Compra :  \t ");
        monto = sc.nextDouble();




        if (membrecia.equals("Clasica")) {
            montoReal = monto - (monto * .10);
        }
        if (membrecia.equals("Oro")) {
            montoReal = monto - (monto * .20);
        }
        if (membrecia.equals("Platino")) {
            montoReal = monto - (monto * .30);
        }
        if (membrecia.equals("otro")) {
            montoReal = monto ;
        }
        System.out.println( nombre + " El valor de tu compra Total es de  $" + montoReal + " Tu membrecia  Fue La " +  membrecia );
    }
}
