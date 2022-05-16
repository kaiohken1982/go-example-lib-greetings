## Greetings lib with test

Esempio di libreria GO con test

Per lanciare i test usare 

```
go test
```

Per utilizzare questa lib da ambiente locale,  
inserirla in import

```
import (
  [...]
  "example.com/greetings"
)
```

quindi lanciare 

```
go mod tidy
```

Modificare quindi il file go.mod 
per far puntare alla dir locale

```
[...]
require example.com/greetings v0.0.0-00010101000000-000000000000

replace example.com/greetings => ../greetings
```

# Agomenti trattati

- Libreria GO esterna locale
- Inizializzazione ed uso random
- Gestione errori
- Inizializzazione ed assegnazione con :=
