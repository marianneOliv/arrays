# arrays


package notas;
import java.util.Arrays;
import javax.swing.JOptionPane;



public class Notas {
   private static final int TAM = 5;
   static float [] notas = new float [TAM];
   
    public static void main(String[] args) {
        float aux;
        for (int i=0;i<TAM;i++){
            notas [i]= Float.valueOf(JOptionPane.showInputDialog("Informe uma nota:"));
        }
        decrescente(notas);
        
        media(notas);
   }

    private static void decrescente(float[] notas) {
        float aux;
        for (int i =1 ;i<5;i++){
            for (int j=0; j<i;j++){
                if (notas[j]<notas[i] ){
                aux=notas [j];
                notas [j]= notas [i];
                notas [i]= aux;
                
            }
                
            }
        }
        for (int i=0; i<5;i++){
        System.out.println(notas[i]+ "");
    }
        
    }

    private static void media(float[] notas) {
        float media =0;
        for (int i=0; i<5;i++){
            media += notas[i];
        }
        media=media/5;
        System.out.println("Media:"+media);
    }
    
}
