# Co
// Clase Persona
class Persona {
  constructor(edad, nombre, telefono) {
    this.edad = edad;
    this.nombre = nombre;
    this.telefono = telefono;
  }
}

// Clase Cliente que hereda de Persona
class Cliente extends Persona {
  constructor(edad, nombre, telefono, credito) {
    super(edad, nombre, telefono);
    this.credito = credito;
  }
}

// Clase Trabajador que hereda de Persona
class Trabajador extends Persona {
  constructor(edad, nombre, telefono, salario) {
    super(edad, nombre, telefono);
    this.salario = salario;
  }
}

// Crear un objeto Cliente
const cliente = new Cliente(30, "Juan", "123456789", 1000);

// Mostrar las propiedades del Cliente por consola
console.log("Edad del cliente:", cliente.edad);
console.log("Nombre del cliente:", cliente.nombre);
console.log("Teléfono del cliente:", cliente.telefono);
console.log("Crédito del cliente:", cliente.credito);

// Crear un objeto Trabajador
const trabajador = new Trabajador(40, "Pedro", "987654321", 2000);

// Mostrar las propiedades del Trabajador por consola
console.log("Edad del trabajador:", trabajador.edad);
console.log("Nombre del trabajador:", trabajador.nombre);
console.log("Teléfono del trabajador:", trabajador.telefono);
console.log("Salario del trabajador:", trabajador.salario);
