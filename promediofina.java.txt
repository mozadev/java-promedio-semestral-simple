package com.mycompany.mavenproject1;

import javax.swing.JOptionPane;

public class ejercicios {

    public static void main(String[] args) {

        //declaracion de variable

        String nombreAlumno;
        int notaExamenParcial;
        int notaExamenFinal;
        int promedioDePracticasCalificadas;
        int promedioDeTrabajosPracticos;
        double pesoExamenParcial=0.3;
        double pesoExamenFinal=0.4;
        double PesopromedioDePracticasCalificadas=0.15;
        double PesopromedioDeTrabajosPracticos=0.15;
        double promediFinal;

        // ingreso de datos del usuario

        nombreAlumno = JOptionPane.showInputDialog("Digite el nombre del alumno: ");
        notaExamenParcial = Integer.parseInt(JOptionPane.showInputDialog("Digite la nota del examen parcial:"));
        notaExamenFinal = Integer.parseInt(JOptionPane.showInputDialog("Digite la nota del examen final:"));
        promedioDePracticasCalificadas =Integer.parseInt(JOptionPane.showInputDialog("Digite la nota del promedio de practicas:"));
        promedioDeTrabajosPracticos =Integer.parseInt(JOptionPane.showInputDialog("Digite la nora del promedio de trabajos practicos:"));

        // procesamiento de datos
        
        promediFinal=(notaExamenParcial*pesoExamenParcial+notaExamenFinal*pesoExamenFinal+
                promedioDePracticasCalificadas*PesopromedioDePracticasCalificadas+
                promedioDeTrabajosPracticos*PesopromedioDeTrabajosPracticos);

        // impresion de informacion
        
        System.out.println("Nombre del alumno:  " + nombreAlumno);
        System.out.println("promedio Final: " + promediFinal);
        
    }
}
