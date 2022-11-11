@startuml

class Empleado{
 +numEmp: int
+nombre: String
+Sueldo: int
+aumentoSueldo():int
}
class Gerente{
+presupuesto: int
+asignarPresupuesto():int
}
Empleado < | - - Gerente

class Animal{
+nombre: String
+origen: String
+color: String
}
-class Acuatico{
+numAletas: int
}
-class Terrestre{
+numPatas: int
}
-class Aereo{
+numAlas: int
}
Animal - - | > Acuatico
Animal - - | > Terrestre
Animal - - | > Aereo

+class Perro{
+numManchas: int
}
Terrestre - - | > Perro

+class Pajaro {
+tipoPico: String
}
Aereo- - | > Pajaro

+class Ballena{
+largo: int
}
Acuatico - - | > Ballena
@enduml