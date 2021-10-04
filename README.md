# Herencia
La Herencia es uno de los conceptos fundamentales de la programación orientada a objetos ya que permite la reusabilidad de variables y funcionalidades que se han definido en otras clases.

## Codigo no probado

```c++

#include<iostream>
using namespace std;

class ClaseBase
{
    protected:
    int unaVar = 0;
    public:
    void unMetodo(void)
    {
        unaVar++;
        cout<<"unaVar = "<<unaVar<<endl;
    }
};

class ClaseDerivada : public ClaseBase  /* Sintaxis para indicar que ClaseDerivada hereda de ClaseBase */
{
    /* Esta clase implementa los miembros de clase que hereda de ClaseBase */
};

int main()
{
    ClaseDerivada obj1;
    obj1.unMetodo(); /* Acceso a los miembros heredados de ClaseBase */
    obj1.unMetodo();
    return 0;
}
  '''
