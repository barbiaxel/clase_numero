# clase_numero
/*Realiza una clase numero, que almacene un número entero y tenga las siguientes características: • Constructor por defecto que inicializa a 0 el número interno. • Constructor que inicializa el número interno. • Método anyade que permite sumarle un número al valor interno. • Método resta que resta un número al valor interno. • Método getValor que devuelve el valor interno. • Método getDoble que devuelve el doble del valor interno. • Método getTriple que devuelve el triple del valor interno. • Método setNumero que inicializa de nuevo el valor interno.*/

public class numero
{
      private int dato;
      public void aniade(int num){dato=dato+num;}
      public void resta(int num){dato=dato-num;}
      public int getValor(){return dato;}
      public int getDoble(){return 2*dato;}
      public int getTriple(){return 3*dato;}
      public void setNumero(int num){dato=num;}
      public boolean esPrimo(){
      boolean primo=true;
        for(int i=2; i<dato/2; i++)
          if (dato%i==0) {
          primo=false;
          break;
          }
          return primo;
        }
      numero(){dato =0;}
      numero(int dato){this.dato=dato;}
      public static void main(String [] args)
    {
    numero m = new numero(2);
    m.setNumero(2);
    m.aniade(11);
    System.out.println(m.getDoble());
    System.out.println(m.getTriple());
    System.out.println(m.getValor());
    System.out.println("El numero: "+m.getValor()+" es primo?
    "+m.esPrimo());
    }
}
