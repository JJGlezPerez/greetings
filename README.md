# Saludos en Go

Este paquete proporciona una forma simple de obtener saludos personalizados en Go.

## Instalacion
Ejecuta el siguiente comand para instala el paquete: 
```bash
go get -u github.com/JJGlezPerez/greetings
```

## Uso 
Aqui tienes un ejemplo de como utilizar el paquete en tu codigo:

```go
package main

import (
    "fmt"
    "github.com/JJGlezPerez/greetings"
)

func main() {
    message, err := greetings.Hello("Alex")

    if err != nil {
        fmt.Println("Ocurrio un error: ",err)
        return
    }

    fmt.Println(message)
}
