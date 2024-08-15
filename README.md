# Saludos en Go

Este paquete proporciona una forma simple de obtener saludos personalizados en Go.

## Instalación
Ejecuta el siguiente comando para instalar el paquete:

```bash
go get -u github.com/jceduardo/greetings
```

## Uso
Aquí tienes un ejemplo de cómo utilizar el paquete en tu código:

```go
package main

import (
	"fmt"
	"log"

	"github.com/jceduardo/greetings"
)

func main() {
	log.SetPrefix("greetings: ")
	//log.SetFlags(0)

	names := []string{"Juan", "Vivi", "Alex"}
	messages, err := greetings.Hellos(names)
	if err != nil {
		log.Fatal(err)
	}

	fmt.Println(messages)
}
```

