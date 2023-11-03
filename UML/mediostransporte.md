@startuml

scale 3

abstract class MediosTransporte{
    -tipo: String
    -numPasajeros: int
    -costo: float
    +avanzar(): void
    +frenar(): void
    +calcularDistacia(float tiempo, float velocidad): void
}

class TransporteAcuatico{
    -tripulante: int
    -capacidad: int
    -tipoAc: String
    +navegar(String destino): void
    +calcularCarga(): float
}


class TransporteTerrestre{
    -ventanas: int
    -combustible: int
    -puertas: int
    +avanzar(): void
    +retroceder(): void
    +cambiarVelocidad(): void
}

class TransporteAereo{
    -alturaVuelo: int
    -velocidadAscenso: float
    -velocidadDescenso: float
    +despegar(): void
    +aterrizar(): void
    +recorrerRuta(): void
}

class Barco{
    -puertoOrigen: String
    -puertoDestino: String
    +abordarPasajeros():void
}

class Trajinera{
    -guia: String
    +inicarRecorrido(): void
    +parar(): void
    +tomarFoto(): void
}

class Supraterraneo{
    -llantas: int
    -motor: int
    -color: String
    +manejar(): void
    +estacionar(): void
    arrancar(): void
}

class Subterraneo{
    -vagones: int
    -linea: String
    -capacidad: int
    +frenar(): void
    +abrirPuerta():void
    +avanzar():void
}

class Avion{
    -alturaMax: int
    -modelo: String
    +volar(String destino): void
    +subirAltura(): void
    +bajarAltura(): void

}

class Helicoptero{
    -numHelices: int
    -numMotores: int
    +acelerar(float velocidad): void
    +girar(String lado): void
}

class Taxi{
    -modelo: String
    -taximetro: int
    +manejar(): void
    +abrir(): void
    +cobrar(): void
}

class Combi{
    -capacidad: int
    -ruta: int
    +seguirRuta(): void
    +cobrar(): void
    +frenar(): void

}

class Metro{
    -capacidad: int
    +viajar(String destino): void
    +fallar(): void
    +ingresar(int personas): void
}

class Suburbano{
    -ruta: String
    +cambiarRuta(String destino): void
    +destino(): void
}


MediosTransporte <|-- TransporteAcuatico
MediosTransporte <|-- TransporteTerrestre
MediosTransporte <|-- TransporteAereo

TransporteAcuatico <|-- Barco: interfaz 
TransporteAcuatico <|-- Trajinera: interfaz
TransporteTerrestre <|-- Supraterraneo: interfaz
TransporteTerrestre <|-- Subterraneo: interfaz
TransporteAereo <|-- Avion: interfaz
TransporteAereo <|-- Helicoptero: interfaz

Supraterraneo <|-- Taxi: interfaz
Supraterraneo <|-- Combi: interfaz

Subterraneo <|-- Metro: interfaz
Subterraneo <|-- Suburbano: interfaz



@enduml