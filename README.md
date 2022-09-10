# Herencia
Es uno de los conceptos fundamentales de la programacion orientada a objetos ya que permite la reusabilidad de variables y funcionalidades que se han definido en otras clases.

```c++
//Crea una clase
class Animal
{
    //Se crea las funciones
  public:
    void comer()
    {
      Serial.println("Puedo comer");
    }

    void dormir()
    {
      Serial.println("Puedo dormir");
    }
};

//Se crea la clase hija
class Dog : public Animal {

    //Crea funciones en la clase hija
  public:
    void ladrar() {
      Serial.println("Puedo ladrar");
    }
};

void setup()
{
  Serial.begin(9600); //Inicia el puerto serial
}

void loop()
{
  Dog perro; //Crea el objeto de la clase

  //Llama funciones de la clase principal
  perro.comer();
  perro.dormir();

  //Llama una funcion de la clase hija
  perro.ladrar();

  delay(5000); //Retardo de 5 segundos
}
```
