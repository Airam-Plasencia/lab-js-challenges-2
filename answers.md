1. Challenge 1:
  - Answer: b
  - Explanation: foo es una variable global y cualquier cambio dentro de la función bar afecta a la global foo.


2. Challenge 2:
  - Answer: c
  - Explanation: let a = 1 , es la variable global, cuando la pasas a un argumento en example(a) y la cambias por a = 10 , en el local es 10 dentro de la función pero el global sigue siendo 1.


3. Challenge 3:
  - Answer: c 
  - Explanation: la declaración de say Hi() esta arriba y JavaScript pone primero la declaración de la función, por lo tanto dentro function sayHi() el console.log va mostrar el texto espuesto.


4. Challenge 4:
  - Answer: c 
  - Explanation: 
  const a = { num: 42 }; crea un objeto con la propiedad num  a 42 y lo asigna a.
  const b = a; hace que b haga referencia al mismo objeto al que apunta a.
  b.num = 90; modifica la propiedad num del objeto y lo sustituye por 90. 

  Por lo tanto console.log(a); es { num: 90 } ya que b = a y b se ha modificado a 90.


5. Bonus - Challenge 5:
  - Answer: c
  - Explanation:
  function magicHat(obj) {
  obj.age = 10;
  obj = { name: "Ada", age: 20 };
  return obj;
}   tenemos una función con un objeto obj = { name: "Ada", age: 20 };

const rabbit1 = { name: "Bob", age: 30 }; una constante rabbit1 con nombre Bob , edad 30.
const rabbit2 = magicHat(rabbit1); al llamar esta constante rabbit1 pasa a la función de magicHat y
obj.age = 10; es el nueva constante que es rabbit1 por lo que la modifica a { name: "Bob", age: 10 } el obj.age seria ahora rabbit1.age.
el console.log(rabbit1) es el nuevo objeto { name: "Bob", age: 10 };
