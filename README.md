# inf450_2023-1

[Rascunho no Excalidraw](https://excalidraw.com/#json=15KXt5mk6sa4Shr7iu0Vb,483hu3vDrCqqQeKGN7ufXQ)

## Memória Cache (leitura e escrita)

### Parâmetros

* [5:0] : Tamanho da RAM (em B) -> R
* [5:0] : Tamanho da Cache (em B) -> C
* [4:0] : Tamanho do Bloco (em B) -> B

### Entrada:

* [0:0] : Operação (leitura ou escrita) -> Op
    * leitura = 0 / escrita = 1
* [5:0] : Endereço (= R) -> Addr
* [7:0] : Dado -> Data

### Saída:
* [7:0] : Dado da RAM -> RAMData (válido para Op == 0)

## Módulos

* Memória RAM
* Memória Cache
* Memória TAG
* Memória Valid
* Memória Dirty
* FSM Controle
* FSM Contador
* Mux
* Comparator
