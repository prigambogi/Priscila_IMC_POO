# Priscila_IMC_POO
package com.mycompany.imc;

import javax.swing.JOptionPane;

/**
 *
 * @author Alex
 */
public class IMC {

    public static void main(String[] args) {
       
        float peso;
        float altura;
        String resp;
        String situacao;
        
        
        resp = JOptionPane.showInputDialog(" Digite seu Peso em kg:");
        peso = Float.parseFloat(resp);
        
        JOptionPane.showMessageDialog(null, " O seu peso em Kg é : " +  peso);
        
        resp = JOptionPane.showInputDialog(" Digite sua Altura em m:");
        altura = Float.parseFloat(resp);
        
        JOptionPane.showMessageDialog(null, " A sua altura em m é : " +  altura);
        
        float imc = peso / (altura * altura);
        
        if (imc < 17) {
           situacao = "Muito abaixo do peso";
        } else 
            if (imc >= 17 && imc <= 18.49) {
            situacao = "Abaixo do peso";
        } else 
                if (imc >= 18.5 && imc <= 24.99) {
            situacao = "Peso normal";
        } else 
                if (imc >= 25 && imc <= 29.99) {
            situacao = "Acima do peso";
        } else 
                if (imc >= 30 && imc <= 34.99) {
            situacao = "Obesidade I";
        } else 
                if (imc >= 35 && imc <= 39.99) {
            situacao = "Obesidade II (severa)";
        } else {
            situacao = "Obesidade III (mórbida)";
        }
        JOptionPane.showMessageDialog(null, "Seu IMC é: " + imc );
        JOptionPane.showMessageDialog(null,"Situação: " + situacao);
        

        
    }
        
        
        
    }
