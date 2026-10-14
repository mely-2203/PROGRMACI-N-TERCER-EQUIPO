package poo;

import javax.swing.JOptionPane;
import javax.swing.ImageIcon;
import java.util.ArrayList;

public class CASETADECOBRO {

    public static void main(String[] args) {

       
        ArrayList<String> vehiculos = new ArrayList<String>();

        ImageIcon Logo = new ImageIcon("C:\\Users\\USUARIO\\Pictures\\vehiculos\\images.png");
        ImageIcon moto = new ImageIcon("C:\\Users\\USUARIO\\Pictures\\vehiculos\\moto.png");
        ImageIcon carro = new ImageIcon("C:\\Users\\USUARIO\\Downloads\\carro.png");
        ImageIcon auto = new ImageIcon("C:\\Users\\USUARIO\\Pictures\\vehiculos\\camion de carga.png");
        ImageIcon lata = new ImageIcon("C:\\Users\\USUARIO\\Pictures\\vehiculos\\autobus 2,3 y 4.png");
        ImageIcon mely = new ImageIcon("C:\\Users\\USUARIO\\Pictures\\vehiculos\\camion.png");
        ImageIcon said = new ImageIcon("C:\\Users\\USUARIO\\Pictures\\vehiculos\\camion 5 y 6.png");
        ImageIcon migu = new ImageIcon("C:\\Users\\USUARIO\\Pictures\\vehiculos\\camion 7 y 8.png");
        ImageIcon chayo = new ImageIcon("C:\\Users\\USUARIO\\Pictures\\vehiculos\\camion ligero.png");

        JOptionPane.showMessageDialog(
            null,
            "MENU DE OPCIONES CASETA DE COBRO",
            null,
            JOptionPane.PLAIN_MESSAGE,
            Logo
        );

        JOptionPane.showMessageDialog(null,
            "\n1._MOTOCICLETA"
            + "\n2._AUTOMÓVIL"
            + "\n3._CAMIÓN DE CARGA"
            + "\n4._AUTOBUS DE 2, 3 Y 4 EJES"
            + "\n5._CAMIÓN DE 2, 3 Y 4 EJES"
            + "\n6._CAMIÓN DE 5 Y 6 EJES"
            + "\n7._CAMIÓN DE 7, 8 Y 9 EJES"
            + "\n8._CAMIÓN LIGERO",
            null,
            JOptionPane.PLAIN_MESSAGE
        );

        int opcion = Integer.parseInt(
            JOptionPane.showInputDialog("Selecciona una opción, del 1 al 8.")
        );

        switch (opcion) {

            case 1:
                vehiculos.add("Motocicleta - $117");
                JOptionPane.showMessageDialog(null, "Ha escogido la opción de motocicleta.", null, JOptionPane.PLAIN_MESSAGE, moto);
                JOptionPane.showMessageDialog(null, "Se le cobrará la siguiente cantidad: $117.", null, JOptionPane.PLAIN_MESSAGE, moto);
                JOptionPane.showMessageDialog(null, "Vuelva pronto.", null, JOptionPane.PLAIN_MESSAGE, moto);
                break;

            case 2:
                vehiculos.add("Automóvil - $234");
                JOptionPane.showMessageDialog(null, "Ha escogido la opción de automóviles.", null, JOptionPane.PLAIN_MESSAGE, carro);
                JOptionPane.showMessageDialog(null, "Se le cobrará la siguiente cantidad: $234.", null, JOptionPane.PLAIN_MESSAGE, carro);
                JOptionPane.showMessageDialog(null, "Vuelva pronto.", null, JOptionPane.PLAIN_MESSAGE, carro);
                break;

            case 3:
                vehiculos.add("Camión de carga - $270");
                JOptionPane.showMessageDialog(null, "Ha escogido la opción de camión de carga.", null, JOptionPane.PLAIN_MESSAGE, auto);
                JOptionPane.showMessageDialog(null, "Se le cobrará la siguiente cantidad: $270.", null, JOptionPane.PLAIN_MESSAGE, auto);
                JOptionPane.showMessageDialog(null, "Vuelva pronto.", null, JOptionPane.PLAIN_MESSAGE, auto);
                break;

            case 4:
                vehiculos.add("Autobús de 2, 3 y 4 ejes - $468");
                JOptionPane.showMessageDialog(null, "Ha escogido la opción de autobús de 2, 3 y 4 ejes.", null, JOptionPane.PLAIN_MESSAGE, lata);
                JOptionPane.showMessageDialog(null, "Se le cobrará la siguiente cantidad: $468.", null, JOptionPane.PLAIN_MESSAGE, lata);
                JOptionPane.showMessageDialog(null, "Vuelva pronto.", null, JOptionPane.PLAIN_MESSAGE, lata);
                break;

            case 5:
                vehiculos.add("Camión de 2, 3 y 4 ejes - $468");
                JOptionPane.showMessageDialog(null, "Ha escogido la opción de camión de 2, 3 y 4 ejes.", null, JOptionPane.PLAIN_MESSAGE, mely);
                JOptionPane.showMessageDialog(null, "Se le cobrará la siguiente cantidad: $468.", null, JOptionPane.PLAIN_MESSAGE, mely);
                JOptionPane.showMessageDialog(null, "Vuelva pronto.", null, JOptionPane.PLAIN_MESSAGE, mely);
                break;

            case 6:
                vehiculos.add("Camión de 5 y 6 ejes - $702");
                JOptionPane.showMessageDialog(null, "Ha escogido la opción de camión de 5 y 6 ejes.", null, JOptionPane.PLAIN_MESSAGE, said);
                JOptionPane.showMessageDialog(null, "Se le cobrará la siguiente cantidad: $702.", null, JOptionPane.PLAIN_MESSAGE, said);
                JOptionPane.showMessageDialog(null, "Vuelva pronto.", null, JOptionPane.PLAIN_MESSAGE, said);
                break;

            case 7:
                vehiculos.add("Camión de 7, 8 y 9 ejes - $1053");
                JOptionPane.showMessageDialog(null, "Ha escogido la opción de camión de 7, 8 y 9 ejes.", null, JOptionPane.PLAIN_MESSAGE, migu);
                JOptionPane.showMessageDialog(null, "Se le cobrará la siguiente cantidad: $1053.", null, JOptionPane.PLAIN_MESSAGE, migu);
                JOptionPane.showMessageDialog(null, "Vuelva pronto.", null, JOptionPane.PLAIN_MESSAGE, migu);
                break;

            case 8:
                vehiculos.add("Camión ligero - $117");
                JOptionPane.showMessageDialog(null, "Ha escogido la opción de camión ligero.", null, JOptionPane.PLAIN_MESSAGE, chayo);
                JOptionPane.showMessageDialog(null, "Se le cobrará la siguiente cantidad: $117.", null, JOptionPane.PLAIN_MESSAGE, chayo);
                JOptionPane.showMessageDialog(null, "Vuelva pronto.", null, JOptionPane.PLAIN_MESSAGE, chayo);
                break;

            default:
                JOptionPane.showMessageDialog(null, "ERROR!!!");
                JOptionPane.showMessageDialog(null, "No es válida la opción, seleccione de la opción 1 a la 8.");
                break;
        }

      
        if (!vehiculos.isEmpty()) {
            JOptionPane.showMessageDialog(
                null,
                "VEHICULO REGISTRADO:\n" + vehiculos.get(0)
            );
        }
    }
}
