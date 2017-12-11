# 1935 A - Parte 1 - Introdução

### Aula 1 - O que é um ORM?

### Aula 3 - Imersão
O data context representa o banco de dados em memória  
	Isso não quer dizer que todo o banco (todas as tabelas, etc..) serão carregados na memória, existe uma otimização  
O Data Context nada mais é do que uma classe comum que herda a classe DbContext  
DbSet<Cliente> é uma coleção de cliente, semelhante a um List<Cliente>, só que no primeiro caso os items da coleção são obtidos do banco de dados  
18:20 Relacionamentos entre tabelas explicados nas classes  
Método Seed  
20:10  Comentário do Baltieri sobre ferramentas geradoras de código
Database Project Visual Studio  
	Permite que você versione um banco de dados pelo visual studio, quando você rodar o projeto ele gera um script com as diferenças entre o banco para você aplicar  
	
### Aula 4 - Mapeamento
01:00 Quadro com listagem de alguns data annotations  
08:20 Usando DbContext sem repositorio, de forma simples para exemplos rápidos  
Conceito de POCO, classes que dependam apenas de recursos da CLR  
Mapeamento de Stored Procedures  

# 1935 B - Parte 2 - Operações Básicas

### Aula 1 - CRUD
10:00 Objetos aninhados

### Aula 2 - Leitura de dados
Lazy Load  (https://msdn.microsoft.com/en-us/data/jj574232.aspx)  
20:10 - LINQ (Language Integrated Query)  
	Permite realizar consultas em objetos  
10:00 Carregamento de múltiplos níveis com Eagger Loading e include  
	Traz todo o conteudo com apenas uma requisição
	
Pequeno descritivo de comandos First, Single, Any, Contains, Where e Find  
Site 101 Linq Examples  
Exemplos de Where, Join e Group  

# 1935 C - Parte 3 - Otimização

### Aula 1 - Ferramentas
EF Profiler

### Aula 2 Performance
Quadro comparativo de Cold x Warm Queries  
Caching  
Queries  
Não terminei de assistir essa aula, parei aos 35 minutos  

### Aula 3 - Fine Tune
Não assisti essa aula

# 1935 D - Parte 4 - Repository Pattern

### Aula 1 - Repository Pattern
Por que separar o Domain em um outro assembler (aplicação)?  
	Se você tiver o Domain separado em pasta e precisar usar o domínio em outra aplicação, ele trará todo projeto (Controllers, Views, etc...) coisas que você não usará  
Definição de contrato para Interfaces: é o que pode e o que não pode ser feito  
	Por que utilizar interfaces na injeção de dependências  
	Como um contrato para o repositório a interface deve apenas abstrair métodos referentes ao acesso a dados, métodos de validação devem ficar no domínio  
15:32 Por que utilizar Ilist no lugar de Ienumerable no Listar  
25:00 Por que separar a Interface e a classe dos repositórios em diferentes camadas (projetos)  
41:00 ValidationMessage  
UnityOfWork  
	É uma abstração do Save do DbContext do seu repositório a fim de trabalhar com transações  
Aos 55 minutos tem um exemplo de como compartilhar um dbcontext sem usar injecao de dependencias
