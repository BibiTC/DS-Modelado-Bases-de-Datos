

# Diagrama ER para gestionar cuentas bancarias y pagos de servicios. 

**Entidades:**

*  _Cliente:_ Con atributos como cod_cliente, nombre, etc.
*  _Cuenta Bancaria:_ Con atributos como ID_Cuenta, Número de Cuenta, Tipo de Cuenta, Saldo, etc.
*  _Servicio:_ Con atributos como ID_Servicio, Nombre del Servicio, Descripción, Precio, etc.
*  _Transacción:_ Con atributos como ID_Transacción, Fecha, Importe, Tipo de Transacción (Crédito/Débito), ID_Cuenta_Bancaria, ID_Servicio, etc.


**Relaciones:**
* Cliente posee Cuenta Bancaria: Un cliente puede tener una o más cuentas bancarias. (Relación uno a muchos)
* Cuenta Bancaria realiza Transacciones: Una cuenta bancaria puede realizar varias transacciones. (Relación uno a muchos)
* Transacción paga Servicio: Una transacción está asociada a un servicio que se paga.
(Relación uno a uno, un servicio puede ser pagado por una transaccion)

**Ejemplo aplicable en el dia a dia:**
Imaginemos que Juan (Cliente) tiene una cuenta de ahorros (Cuenta Bancaria) y realiza una transacción para pagar la luz (Servicio).
En el diagrama, Juan estaría conectado a la cuenta de ahorros, y la cuenta de ahorros estaría conectada a la transacción de pago de la luz.
La transacción de pago de la luz también estaría conectada al servicio "Luz".

**Cardinalidades:**
* Un Cliente puede tener 0 a muchos Cuentas Bancarias.
* Una Cuenta Bancaria puede realizar 0 a muchas Transacciones.
* Una Transacción paga a 1 Servicio.

## :white_check_mark:Estado del proyecto

Finalizado 

---

## 📁 Acceso al proyecto
El proyecto se puede descargar o acceder desde este link de GitHub, son diagramas que se pueden visualizar en https://app.diagrams.net/ (Modelo Concpetual y Logico) y para ver el Modelo fisico debe instalarse SQL Power Architect https://bestofbi.com/architect-download/ .

[GitHub - Challenge Data Science - Modelado Datos Python](https://github.com/BibiTC/DS-Modelado-Bases-de-Datos.git)


## :white_check_mark:Tecnologías utilizadas
- diagrams.net
- SQL Power Architect
  
## Contribución
Este proyecto existe gracias al curso de ONE Oracle Next Education y Alura Latam, Grupo 8.

[<img src="https://avatars.githubusercontent.com/alura-es-cursos" width=115><br><sub>Alura Latam</sub>](https://github.com/alura-es-cursos)


## Autor

[<img src="https://avatars.githubusercontent.com/BibiTC" width=115><br><sub>Bibiana Trujillo</sub>](https://github.com/BibiTC)

## Licencia

Data Science - Modelado de Base de Datos [MIT licensed].
