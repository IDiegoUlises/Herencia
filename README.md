# Herencia editar
La Herencia es uno de los conceptos fundamentales de la programación orientada a objetos ya que permite la reusabilidad de variables y funcionalidades que se han definido en otras clases.

```c++
//Crea la clase
class Animal
{
  public:
    void comer() {
      Serial.println("Puedo comer");
    }

    void dormir() {
      Serial.println("Puedo dormir");
    }
};

//Crea la clase hija
class Dog : public Animal {

  public:
    void ladrar() {
      Serial.println("Puedo ladrar");
    }
};

void setup()
{
  Serial.begin(9600);
}

void loop()
{
  Dog perro;

  perro.comer();
  perro.dormir();

  //Llama a la clase hija
  perro.ladrar();

  delay(1000);
}
```
