# Piedra-Papel-o-Tijera
package piedrapapeltijera;

import java.util.Scanner;
import java.math.*;

public class PiedraPapelTijera {

    
    public static void main(String[] args) {
        int op_ju, op_pc;
        Scanner Lec=new Scanner(System.in);
       do{ 
        System.out.println("Elige una Opción: ");
        System.out.println("1) Piedra ");
        System.out.println("2) Papel ");
        System.out.println("3) Tijera ");
        op_ju=Lec.nextInt();
        op_pc= (int) (Math.random()*3)+1;
        
        System.out.println("El usuario a escogido: "+op_ju+" la pc ha escogido: " +op_pc);
        
        if(op_ju==1){
         if(op_pc==1)   
            System.out.println("Han empatado!");
         if(op_pc==2)
            System.out.println("Jugador Eligio: Piedra, Pc escogio: Papel--- jugador pierde, pc gana");
        if(op_pc==3)
                System.out.println("Jugador Eligio: Piedra, Pc escogio: Tijera--- jugador gana, pc pierde");
           }else 
            
              if(op_ju==2){
         if(op_pc==2)   
            System.out.println("Han empatado!" );
            if(op_pc==2)
            System.out.println("Jugador Eligio: Papel, Pc escogio: Piedra--- jugador gana, pc pierde");
            if(op_pc==3)
                System.out.println("Jugador Eligio: Papel, Pc escogio: Tijera--- jugador pierde, pc gana");
             }else
                  
             if(op_ju==3){
         if(op_pc==1)   
            System.out.println("Jugador Eligio: Tijera, Pc escogio: Piedra--- jugador pierde, pc gana");
         if(op_pc==2)
            System.out.println("Jugador Eligio: Tijera, Pc escogio: Papel--- jugador gana--- pc pierde");
         if(op_pc==3)
                System.out.println("Han empatado!");
         }                    
                
             
                 } while(op_ju==op_pc);
        
    }
    
}
