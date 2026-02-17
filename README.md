Este es un programa desarrollado en **JavaScript** diseñado para calcular el precio final de una cotizacion de la empresa TK-U, basándose en el perfil del asegurado, su estado civil y su carga familiar.

## 🚀 Funcionamiento

El programa solicita datos al usuario mediante ventanas emergentes (`prompt`) y realiza cálculos automáticos aplicando recargos porcentuales sobre un **precio base de Q. 2,000**.

### Requerimientos Implementados

1.  **Validación de Mayoría de Edad**: El sistema restringe el cálculo si el asegurado es menor de 18 años.
2.  **Recargos por Edad**: Se aplican rangos tanto para el asegurado como para el cónyuge:
    * **18 - 24 años**: 10% de recargo.
    * **25 - 49 años**: 20% de recargo.
    * **50 años o más**: 30% de recargo.
3.  **Cargo por Hijos**: Un recargo del 20% sobre el precio base por cada hijo, sin importar su edad.

## 🛠️ Detalles Técnicos y Cambios Realizados

Para asegurar la precisión del programa, se implementaron las siguientes mejoras:

* **Bloque de Validación**: Todo el proceso de cálculo está envuelto en una estructura condicional que verifica la edad inicial, cumpliendo con la restricción de no procesar a menores de edad.
* **Acumulación de Recargos**: Se utilizó el operador de asignación compuesta `+=` para sumar de forma incremental cada recargo al `recargo_total`. Esto permite que los recargos del asegurado, cónyuge e hijos se sumen correctamente sin sobrescribirse.
* **Lógica de Proporción por Hijos**: El recargo por hijos se calcula multiplicando el porcentaje fijo por la cantidad total de hijos ingresada por el usuario.
* **Estandarización de Entradas**: Se implementó el método `.toUpperCase()` en las respuestas de texto. Esto garantiza que el programa funcione correctamente aunque el usuario escriba "si", "Si" o "SI".

## 💻 Cómo ejecutarlo

1. Clona este repositorio o descarga el archivo `.js`.
2. Puedes ejecutarlo de dos formas:
   * **Consola del Navegador**: Copia el código y pégalo en la consola de desarrollador (F12) en cualquier navegador.
   * **Archivo HTML**: Vincula el script a un archivo HTML y ábrelo en tu navegador.

---
Desarrollado como parte del proyecto de lógica de programación.
