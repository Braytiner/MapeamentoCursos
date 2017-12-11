# 1940 A - Parte 1 - Backend

### Aula 1
Explicação sobre as camadas nas quais a aplicação está dividida

### Aula 2
Utilização do Postman  
10:00 Montando as classes (a partir da mais básica Categoria)  
15:10 Abordagem inicial do projeto de testes  
27:57 Trabalhando com listas em classes  
  28:25 Sempre instanciar/inicializar listas em classes mestre-detalhe  
32:27 Diferenças entre Ilist e Icollection  
34:20 Inicio Bloqueando adição avulsa de itens  
  41:06 Direto ao ponto  
	42:30 Trabalhando externamente com Ienumerable e internamente com  Ilist  
44:27 Total do pedido dinâmico (através de método)  
	Existe uma outra forma em outro curso usando linq  
  Curso 1969 - Aula 8 (Subtotal - 07:30, Total - 08:25)  
46:00 Status do pedido usando enumeradores  

### Aula 3
00:40 - Por que não usar exceptions  
03:25 Domain Notifications/Domain Events  
06:38 Injeção de dependências  
	O Icontainer será semelhante a classe gerada pelo Unity para gerenciar as dependencias  
08:04 Domain Events  
	Podemos usar esse recursos como listeners para realizar algumas operações quando algo ocorrer no domínio  
13:46 Implementando Domain Notifications manualmente (sem a utilização do FluentValidator)  
15:20 Helpers  
29:25 Update  
30:50 Scopes  

### Aula 4
07:15 Dica de reuso de objetos em Testes  
11:33 Resumo de fluxo sobre como trabalhar com escopos  
Parei em 13:13  

### Aula 5
Commands  
	02:59 Não precisar ser um command específico para cada unidade  
10:40 Specs  
	20:29 Vantagens  

### Aula 6
Repositórios  
07:40 Montagem da abstração da camada de serviços (application services)  

### Aula 7
Montagem da camada de infraestrutura  
17:30 Unit of Work  
32:40 EF Profiler  
	Analisador de queries geradas pelo EF  
	
### Aula 8
Implementação da camada de Serviços (Application Services)  
	Não terminei de assistir devido a complexidade desnecessária das implementações  
	
### Aula 9
CrossCutting (Pulei)  
10:32 Desenvolvimento da API  
	Instale o `Owin`  
	Instale `Microsoft.Owin.Host.SystemWeb`  
	Para segurança baseada em tokens, instale: `Microsoft.Owin.Security.Oauth`  
	`Microsoft.Owin.Cors`  
	EntityFramework  
