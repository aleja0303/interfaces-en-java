import javax.swing.*;

public class SimpleGUI {
    public static void main(String[] args) {
        // Crear una nueva ventana
        JFrame frame = new JFrame("Ejemplo de GUI Simple");
        
        // Configurar el tamaño de la ventana
        frame.setSize(300, 200);
        
        // Crear un botón
        JButton button = new JButton("Haz clic aquí");
        
        // Añadir el botón a la ventana
        frame.add(button);
        
        // Configurar la operación por defecto al cerrar la ventana
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        
        // Hacer visible la ventana
        frame.setVisible(true);
    }
}
