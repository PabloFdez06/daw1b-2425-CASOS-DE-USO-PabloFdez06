# daw1b-2425-CASOS-DE-USO-PabloFdez06

(Entiendo lo que he realizado, en este ejercicio me he apoyado en algun momento de chatgpt, resolver duda en clase)

## CÓDIGO:

```
@startuml

actor Cliente
actor "Sistema Bancario" as SB

rectangle Cajero {
    usecase "Validar identidad" as R1
    usecase "Sacar dinero" as R2
    usecase "Verificar saldo disponible" as R2a
    usecase "Verificar límite diario" as R2b
    usecase "Realizar transferencia" as R4
    usecase "Realizar ingreso" as R5
}

Cliente --> R1
Cliente --> R2
Cliente --> R4
Cliente --> R5

R2 --> R2a : "Verifica saldo"
R2 --> R2b : "Verifica límite"
R2a --> SB
R2b --> SB

@enduml

```
## RESULTADO DEL CÓDIGO ANTERIOR:

![image](https://github.com/user-attachments/assets/ed6767a3-8328-45b5-a955-0313bae31a15)
