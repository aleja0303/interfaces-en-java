Swing: Swing es un conjunto de componentes GUI para Java. Aquí hay un ejemplo básico de una ventana Swing:
java

import javax.swing.*;

public class VentanaSwing {
    public static void main(String[] args) {
        JFrame frame = new JFrame("Ejemplo de Ventana Swing");
        JButton button = new JButton("Haz clic aquí");
        
        button.setBounds(50, 50, 200, 30);
        frame.add(button);
        
        frame.setSize(300, 200);
        frame.setLayout(null);
        frame.setVisible(true);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
JavaFX: JavaFX es un framework moderno para la creación de aplicaciones de escritorio y aplicaciones web ricas en contenido. Aquí tienes un ejemplo de una ventana JavaFX:
java

import javafx.application.Application;
import javafx.scene.Scene;
import javafx.scene.control.Button;
import javafx.scene.layout.StackPane;
import javafx.stage.Stage;

public class VentanaJavaFX extends Application {
    public static void main(String[] args) {
        launch(args);
    }
    
    @Override
    public void start(Stage primaryStage) {
        primaryStage.setTitle("Ejemplo de Ventana JavaFX");
        Button button = new Button("Haz clic aquí");
        StackPane root = new StackPane();
        root.getChildren().add(button);
        primaryStage.setScene(new Scene(root, 300, 250));
        primaryStage.show();
    }
}
Java AWT: AWT (Abstract Window Toolkit) es la biblioteca original de GUI de Java. Aquí hay un ejemplo básico de una ventana AWT:
java

import java.awt.*;
import java.awt.event.*;

public class VentanaAWT {
    public static void main(String[] args) {
        Frame frame = new Frame("Ejemplo de Ventana AWT");
        Button button = new Button("Haz clic aquí");
        
        button.setBounds(50, 100, 80, 30);
        frame.add(button);
        
        frame.setSize(300, 200);
        frame.setLayout(null);
        frame.setVisible(true);
        
        frame.addWindowListener(new WindowAdapter() {
            public void windowClosing(WindowEvent e) {
                frame.dispose();
            }
        });
    }
}
