# UN3T2
package cola;
public class Colaproceso {
   String cola[]=new String [5];
   int ultimo=-1; 
      public void insertar(String elemento){
        //Inserta un elemento en la Pila
        if(ultimo==5){
        System.out.println("cola llena, Ya no se puede insertar dat0s");
        }
        else{
        cola[++ultimo]=elemento;
        System.out.println("Se inserto el elemento");}
    }
      
     public void eliminar(){
       if(ultimo==-1){
        System.out.println("Cola vacia");
        }
        else{
        for(int i=0;i<ultimo;i++){
	cola[i]=cola[i+1];
	}
	cola[ultimo]="";
        ultimo--;
	}
	} 
     
     public void Mostrar(){
         if(ultimo==-1){
             System.out.println("Cola vacia");
         }
        else{
        for(int i=0;i<=ultimo;i++) {
            System.out.println(cola[i]);
        }

   
}
     }
}
