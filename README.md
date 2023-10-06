#incluir<bits/stdc++.h>

class Circulo {
private:
    double radio;
    double diametro;

public:
    // Constructor para inicializar los atributos
    Circulo(double r) {
        radio = r;
        diametro = 2.0 * r;
    }

    // Métodos para obtener el valor de los atributos (getters)
    double getRadio() {
        return radio;
    }

    double getDiametro() {
        return diametro;
    }

    // Métodos para establecer el valor de los atributos (setters)
    void setRadio(double r) {
        radio = r;
        diametro = 2.0 * r;
    }

    void setDiametro(double d) {
        diametro = d;
        radio = d / 2.0;
    }
};

int main() {
    // Crear una instancia de la clase Circulo con radio inicial
    Circulo miCirculo(5.0);

    // Imprimir los atributos utilizando los métodos get
    std::cout << "Radio: " << miCirculo.getRadio() << std::endl;
    std::cout << "Diámetro: " << miCirculo.getDiametro() << std::endl;

    // Modificar el radio utilizando el método set
    miCirculo.setRadio(3.0);

    // Imprimir los atributos actualizados
    std::cout << "Radio: " << miCirculo.getRadio() << std::endl;
    std::cout << "Diámetro: " << miCirculo.getDiametro() << std::endl;

    return 0;
}
