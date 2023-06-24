- Memória RAM não precisa de input para permissão de leitura?
```
always @ (posedge reset)
  begin
  	if (rd)
  		dout <= memory[addr];
  	end
```
  	
- Parâmetros dentros do arquivos .v são sobrescritos no main?
```
%%writefile datacache.v
module datacache ( clk, line, blk, din, wr, dout );
parameter bitsBlock = 3;
```

- Adicionar reset no datacache.v?
