
#  pshicologicalgamegeneral


## 1. Fundamentos del sistema

Seria un juego con ambientación terror con campo abierto (mundo abierto ) 
trataria temas psicologicos como traumas depresion  y la separación familiar 
estaria ambientado en la epoca futurista pero con objetos antiguos y habria un o una protagonista al gusto de el usuario 
el juego trataria tambien de vencer algun jefe importante de la hsiroria para que cambie de etapa para asi en la siguinete pase algo nuevo en la hisrtorai 



## 2. Análisis y especificación de requisitiso
requisitos funcioanles : 

El jugador podrá crear o elegir al protagonista, seleccionando género, apariencia y nombre.

Se incluirá una  enemigo adaptativo, que cambia su comportamiento en función de las decisiones y el estado emocional del jugador.

El juego permitirá guardar partidas y retomar desde puntos de control.

Requisitos no funcionales

El entorno debe mantener una atmósfera inmersiva mediante iluminación tenue, efectos de sonido ambiental y música disonante

Los tiempos de carga entre áreas no deberán superar los 10 segundos.

Los archivos guardados y configuraciones del jugador estarán encriptados para proteger su información.

## 3. Diseño 
Habria una barra de vida que se regeneraria con objetos curativos que habria en el mapa repartidos y estarian limitados para que el jugador no abuse de ellos 
armas tambien empezaria con un palo o pistola o cuchillo
comofmre va avanzando conseguiria mejroes armas con munición limitada o desgaste y debera a usarlo de forma inteligente 
tambien habria plataformas para poder moverse por el mapa , y el diseño qeu estaria encargado por 5 dos de diseño dos D y dibujo y otros 3 de diseño 3 D 
el movimiento no solo seria por plataformas la gran mayoria seria andando o en unos railes electricos

## 4. Implementación

     // Esta clase sirve como calculadora 
   
        public class Calculadora  
        { 
             
    // Este método suma dos enteros x , y  
        public int sumar(int x, int y) 
        { 
     
        return x + y;} 
 
        // Este método resta x , y  
 
        public int restar(int x, int y) 
        { 
         
     return x - y;} 
 
         // Este método multiplica x  , y entre ellos 
 
        public int multiplicar(int x, int y){ 
     
     return x * y;} 
 
     // Este método divide x , y entre ellos 
 
        public int dividir( int x, int y ) 
    { 
     
        return x / y; 
         
    } 
 
        public static void main(String[] args){ 
     
    Calculadora c = new Calculadora();System.out.println( " resultado: " + c.sumar( 5 , 3 ) ); 
         
    } 
             
        } 
    
    public class alumno 
    { 
        private String NOMBRE; 
         
        private int edad;private double NotaFinal; 
         
        public alumno(String n, int e , double nf) 
        { 
            NOMBRE = n; 
            edad = e; 
            NotaFinal = nf; 
         
        } 
    public void Mostrardatos() 
        {    
            
        System.out.println(" Alumno: " + NOMBRE + ", Edad:" + edad + ", Nota Final:" + 
NotaFinal); 
        } 
    public boolean aprobado() 
    { 
        /**  
         * si la nota final es mayor de 5  
         */ 
        if(NotaFinal >= 5.0) 
        { 
            return true; 
        } 
        else 
        { 
            return false; 
        } 
         
    }       
    public void mensajeFinal()  
    { 
        /** 
         * si es mayor de 5 le sale apribaste y si no sale no aprobaste 
         */ 
         
    if(aprobado) 
            {  
        System.out.println( "felicidades " + NOMBRE + " aprobaste!" ); 
         
            } 
        else  
        { 
    System.out.println("Lo siento " + NOMBRE + " no aprobaste");  
     
        }  
     
    } 
        } 
       
        class curso 
        { 
            private String NOMBRE_CURSO; 
             
            private alumno[] lista; 
             
            public curso( String n , alumno [] l) 
            { 
                NOMBRE_CURSO = n; 
                lista = l; 
             
            } 
        
        public void mostrarTodo() 
        { 
            System.out.println("curso: " + NOMBRE_CURSO); for ( alumno a:lista ) 
            { 
                a.MostrarDatos(); 
                 
                a.mensajeFinal(); 
                 
            } 
 
        } 
    public static void main(String[] args) 
            { 
             alumno a1 = new alumno( "ana", 18 , 6 . 5 ); 
              
             alumno a2 = new alumno( "PEDRO" , 19 , 4 .3); 
              
             alumno a3 = new alumno( "Lucia" , 17 , 8 . 7); 
              
             alumno[] lista =   { a1 , a2 , a3 }; 
                      
                curso c1 = new curso( "programacion" , lista ); 
                 
                c1.mostrarTodo(); 
     
            } 
     
        } 
 
    } 

## 5. Plan de pruebas del sistema
Tipo de prueba 
Funcional : 

Entrada / acción 

Usuario crea una nueva partida 

El sistema recibe la orden y crea nuevos datos para que el usuario lo utilice 
(crea una nueva partida)





### 5.1. Pruebas de aceptación



El usuario ya entra en la partida creada 

El sistema lo recibe y acarga lo datos ya existentes desde donde lo habia dejado el usaurio

Usuario cambia los ajustes del juego

Sistema cambia el como el juego lo percibe el usuario cambiando datos ajustados a las preferencias del usuario.

## 7. Los diccionarios de datos








