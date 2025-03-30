1. Challenge 1:
  - Answer: "abc;
  
  - Explanation: foo se declara fuera de la función con let, por lo que es una variable global. Dentro de bar(), se reasigna su valor a "xyz", y luego se imprime. Como no hay una nueva variable foo dentro del scope de bar(), se modifica la original. Por eso ambos console.log imprimen "xyz".


2. Challenge 2:
  - Answer: 10 and 1
  - Explanation: Cuando se llama a example(a), el argumento se copia por valor (porque es un número primitivo). Dentro de la función, a = 10 afecta solo a la copia local. El console.log(a) fuera de la función sigue mostrando 1.


3. Challenge 3:
  - Answer:  "Hi there!"
  - Explanation: Las declaraciones de función en JavaScript son hoisted, es decir, se elevan al inicio del scope, por lo que puedes llamar la función antes de su definición en el código.


4. Challenge 4:
  - Answer: { num: 90 }
  - Explanation: Aunque a es una constante, su contenido sí puede cambiar (los objetos son mutables). b apunta al mismo objeto que a, así que al cambiar b.num, también cambia a.num.


5. Bonus - Challenge 5:
  - Answer: { name: "Bob", age: 10 } and { name: "Ada", age: 20 }
  - Explanation: obj.age = 10 modifica el objeto original (rabbit1).

Luego, obj apunta a un nuevo objeto { name: "Ada", age: 20 }, pero eso no afecta a rabbit1.

rabbit1 sigue apuntando al objeto original modificado.

rabbit2 apunta al nuevo objeto retornado.


