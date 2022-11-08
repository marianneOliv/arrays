# arrays

package mes;
import java.util.Arrays;

public class mes {
    private static String [] mes = {"Janeiro","Fevereiro", "Março", "Abril", "Maio", 
    "Junho", "Julho","Agosto", "Setembro", "Outubro", "Novembro", "Dezembro"};
    
    public mes() {
    }
    public void mostraMes (int mes){
        if (mes < 0 || mes > 11)
            System.out.println("Mês inválido");
        else 
            System.out.println(this.mes[mes]);
    } 
}


EXECUTA MES 

package mes;

public class ExecMes {
    public static void main(String[] args) {
        mes lista= new mes();
        int valor;
        valor =(int) (Math.random()*12);
        lista. mostraMes(valor);
    }
}
