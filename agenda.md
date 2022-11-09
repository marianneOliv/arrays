# arrays

EXECUTA AGENDA
import java.util.ArrayList;
import java.util.Collection;
import javax.swing.JOptionPane;


public class exemplo {
    public static void main(String[] args) {
        ArrayList< Contato> agenda = new ArrayList();
        
        Contato c = new Contato();
        c.setNome(JOptionPane.showInputDialog("Nome:"));
        c.setFone( Integer.valueOf(JOptionPane.showInputDialog("Telefone:")));
        c.setEndereço(JOptionPane.showInputDialog("Endereço:"));
        
        agenda.add(c);
        JOptionPane.showMessageDialog(null, c.toString());
    }
    
    
    
    }

AGENDA 

package array;
import java.util.Arrays;



public class Contato {
    private  String nome , endereço;
    private int fone;

    public Contato() {
    }

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public String getEndereço() {
        return endereço;
    }

    public void setEndereço(String endereço) {
        this.endereço = endereço;
    }

    public int getFone() {
        return fone;
    }

    public void setFone(int fone) {
        this.fone = fone;
    }

    @Override
    public String toString() {
        return  "nome:" + nome + ", \nendereço:" + endereço + ", \nfone:" + fone + '}';
    }
    
    

 
}

