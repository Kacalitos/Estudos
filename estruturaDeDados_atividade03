import java.util.Scanner;

//import sun.net.www.content.text.plain;

public class App {
   public static Scanner ler = new Scanner(System.in);
    public static void main(String[] args) throws Exception {
        int auxl;
        int x = 5;
        int xx= 10;
        int i = 0;
        lista lista = new lista();
        lista.qtd = 0;
        pilha pilha = new pilha();
        fila fila = new fila();
        for(i =0; i<x;i++){ // Adiciona na lista 
            addObjeto(lista);
        }
        System.out.println("Adicionando na lista");
       
        // listar(lista);//debug
        for(i = 0; i<x; i++){//Remove na lista e inseri na pilha
           auxl = removeIni(lista);
          // System.out.println("Numero retorno:"+auxl);//debug
           //System.out.println("---------------------------");//debug
           pilha.push(auxl);
        }
        System.out.println("Removendo da lista e adicionando na pilha");
        for (i =0; i<x; i++){//Remove na pilha e inseri filha
             auxl= removePilha(pilha);
           // System.out.println("Numero retorno:"+auxl);//debug
           // System.out.println("---------------------------");//debug
            fila.inserir(auxl);   
        }
        System.out.println("Removendo da ilha e adicionando na fila");
        for(i =0; i<x;i++){ // Adiciona na lista 
            addObjeto(lista);
        }
        System.out.println("Adicionando na lista");
        // listar(lista);//debug
        for(i = 0; i<x; i++){//Remove na lista e inseri na pilha
           auxl = removeIni(lista);
          // System.out.println("Numero retorno:"+auxl);//debug
          // System.out.println("---------------------------");//debug
           pilha.push(auxl);
        }
        System.out.println("Removendo da lista e adicionando na pilha");
        for (i =0; i<x; i++){//Remove na pilha e inseri filha
             auxl= removePilha(pilha);
          //  System.out.println("Numero retorno:"+auxl);//debug
           // System.out.println("---------------------------");//debug
            fila.inserir(auxl);   
        }
        System.out.println("Removendo da lista e adicionando na fila");
        System.out.println("Números inseridos na Fila:\n");
        for (i =0; i<xx; i++){//lista fila
            removeFila(fila);      
        }
    }         
//----------------------------------------------------------------------------------------------------------------------------------------------//
    public static int removeIni(lista lista){
        elemento aux = lista.primeiro;
        int numero;
        if(lista.qtd == 0){
            System.out.print("Lista Vazia!");
        }else{
            //System.out.println("Lista sendo removida");//debug
          //  System.out.println("Numero:"+aux.num);//debug

            lista.primeiro = lista.primeiro.proximo;
            lista.qtd--;
        }
       
       // System.out.println("---------------------------");//debug
        numero = aux.num;
        return numero; 
    }
//----------------------------------------------------------------------------------------------------------------------------------------------//
    public static void listar(lista lista){
            elemento aux = lista.primeiro;
            //System.out.println("Numeros digitados:");
            if(aux == null ){
                System.out.println("Lista vazia");
            }else{
            while (aux!=null){
               // System.out.println(aux.num);
                aux =aux.proximo;
            }
        }
      //  System.out.println("---------------------------");
    }
//----------------------------------------------------------------------------------------------------------------------------------------------//
    public static void addObjeto(lista lista){
        elemento novoObj = new elemento();
        elemento objAux = new elemento();
        if(lista.qtd == 0 ){
           System.out.println("Numero:"); 
           novoObj.num =  ler.nextInt();
           novoObj.proximo = null;
        
           lista.primeiro = novoObj;
           lista.ultimo = novoObj;
           lista.qtd++;

        }else{
            objAux = lista.primeiro;
           while(objAux.proximo!=null){
               objAux = objAux.proximo;
           }     

           System.out.println("Numero:"); 
           novoObj.num =  ler.nextInt();
           novoObj.proximo = null;

           objAux.proximo =novoObj;
           lista.ultimo = novoObj;
           lista.qtd++;
        }
        

    }
//----------------------------------------------------------------------------------------------------------------------------------------------//
    public static int removePilha(pilha pilha){
            int elem = pilha.pop();
            //System.out.println("Desemplilhei:"+elem);//debug
            return elem;
        
    }
//----------------------------------------------------------------------------------------------------------------------------------------------//
    public static void removeFila(fila fila){
       int x = fila.retirar();
       System.out.println(x); 
    }
}
