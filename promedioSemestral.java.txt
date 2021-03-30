
package com.mycompany.mavenproject1;

import javax.swing.JOptionPane;

public class ejercicios {

    public static void main(String[] args) {

        //declaracion de variable

        int codigoAlumno;
        String nombreAlumno;
        float promedio1Unidad;
        float promedio2Unidad;
        int peso1Unidad = 1;
        int peso2Unidad = 2;
        float promedioSemetral;

        // ingreso de datos del usuario

        codigoAlumno = Integer.parseInt(JOptionPane.showInputDialog("Digite el codigo del alumno: "));
        nombreAlumno = JOptionPane.showInputDialog("Digite el nombre del alumno: ");

        promedio1Unidad = Float.parseFloat(JOptionPane.showInputDialog("Digite el promedio de la primera unidad: "));
        promedio2Unidad = Float.parseFloat(JOptionPane.showInputDialog("Digite el promedio de segunda unidad: "));

        // procesamiento de datos

        promedioSemetral = (promedio1Unidad * peso1Unidad + promedio2Unidad * peso2Unidad)/(peso1Unidad+peso2Unidad);

        // impresion de informacion
        
        System.out.println("Nombre: " + nombreAlumno);
        System.out.println("cogido de alumno"+codigoAlumno);
        System.out.println("promedio semestral: " + promedioSemetral);

    }
}
