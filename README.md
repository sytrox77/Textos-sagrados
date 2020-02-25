# Textos-sagrados
//PARTES

VEHICULO

import Componentes.Chasis;
import Componentes.Llanta;
import Componentes.Motor;

public class Vehiculo {
    private String marca;
    private String color;
    private String modelo;
    private Chasis estructura;
    private Llanta movimiento;
    private Motor potencia;

    public Vehiculo(String marca, String color, String modelo, Chasis estructura, Llanta movimiento, Motor potencia) {
        this.marca = marca;
        this.color = color;
        this.modelo = modelo;
        this.estructura = estructura;
        this.movimiento = movimiento;
        this.potencia = potencia;
    }

    public Vehiculo() {
        
    }

    public String getMarca() {
        return marca;
    }

    public void setMarca(String marca) {
        this.marca = marca;
    }

    public String getColor() {
        return color;
    }

    public void setColor(String color) {
        this.color = color;
    }

    public String getModelo() {
        return modelo;
    }

    public void setModelo(String modelo) {
        this.modelo = modelo;
    }

    public Chasis getEstructura() {
        return estructura;
    }

    public void setEstructura(Chasis estructura) {
        this.estructura = estructura;
    }

    public Llanta getMovimiento() {
        return movimiento;
    }

    public void setMovimiento(Llanta movimiento) {
        this.movimiento = movimiento;
    }

    public Motor getPotencia() {
        return potencia;
    }

    public void setPotencia(Motor potencia) {
        this.potencia = potencia;
    }
    public void encender(){
        System.out.println("Encendiendo vehiculo de marca:"+ this.marca);
    }
    public void apagar(){
        System.out.println("Apagando vehiculo de marca."+ this.marca);
    }
}


MOTOR

public class Motor {
    private int potencia;
    private int tamanio;
    private String combustion;

    public Motor(int potencia, int tamanio, String combustion) {
        this.potencia = potencia;
        this.tamanio = tamanio;
        this.combustion = combustion;
    }

    public int getPotencia() {
        return potencia;
    }

    public void setPotencia(int potencia) {
        this.potencia = potencia;
    }

    public int getTamanio() {
        return tamanio;
    }

    public void setTamanio(int tamanio) {
        this.tamanio = tamanio;
    }

    public String getCombustion() {
        return combustion;
    }

    public void setCombustion(String combustion) {
        this.combustion = combustion;
    }
    public void encender(){
        System.out.println("Encendiendo....");
    }
         
}

LLANTA

public class Llanta {
    private String marca;
    private int diametro;
    private int presionDelAire;

    public Llanta(String marca, int diametro, int presionDelAire) {
        this.marca = marca;
        this.diametro = diametro;
        this.presionDelAire = presionDelAire;
    }

    public String getMarca() {
        return marca;
    }

    public void setMarca(String marca) {
        this.marca = marca;
    }

    public int getDiametro() {
        return diametro;
    }

    public void setDiametro(int diametro) {
        this.diametro = diametro;
    }

    public int getPresionDelAire() {
        return presionDelAire;
    }

    public void setPresionDelAire(int presionDelAire) {
        this.presionDelAire = presionDelAire;
    }
    public void frenar(){
        System.out.println("Frenando...");
    }
    public void amortiguar(){
        System.out.println("Amortiguando...");
    }
    
}

CHASIS

public class Chasis {
    private String rigidez;
    private int piezaQueLoCompone;
    private int bastidores;

    public Chasis(String rigidez, int piezaQueLoCompone, int bastidores) {
        this.rigidez = rigidez;
        this.piezaQueLoCompone = piezaQueLoCompone;
        this.bastidores = bastidores;
    }

    public String getRigidez() {
        return rigidez;
    }

    public void setRigidez(String rigidez) {
        this.rigidez = rigidez;
    }

    public int getPiezaQueLoCompone() {
        return piezaQueLoCompone;
    }

    public void setPiezaQueLoCompone(int piezaQueLoCompone) {
        this.piezaQueLoCompone = piezaQueLoCompone;
    }

    public int getBastidores() {
        return bastidores;
    }

    public void setBastidores(int bastidores) {
        this.bastidores = bastidores;
    }
    public void sostener(){
        System.out.println("Sosteniendo Peso...");
    }
            
}




