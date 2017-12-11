# 1969 A - Parte 1: Backend

**Neste treinamento é desenvolvido uma aplicação de delivery, refaça o treinamento montando a aplicação**

### Aulas 1 e 2 
Introdução e agenda  

### Aula 3 - Ferramentas
Instalação e verificação de versão do nodejs  
Yeoman - Gerando estrutura básica para aplicações .NET sem Visual Studio  

### Aula 4 - Frameworks
Diferenças entre .NET Core e .NET Full Framework  
Verificar versão do .NET  

### Aula 5 - Startup do projeto
Arquivo .sln é somente um arquivo de agrupamento de projetos  
Compilando aplicações fora da IDE  
Global.json  
Configurações do VisualStudio.Code  

### Aula 6 - OOP de Verdade
Modelo Entidade Relacionamento é mais pobre que OOP, pois OOP tem propriedades, métodos e eventos sendo muito mais rico que o banco de dados  
CodeFirst = codificar primeiro e pensar no banco depois  
Dinamica de fazer a aplicação funcionar sem banco de dados só exibindo e inputando dados na tela  
Conceito de Entidade  
Classe abstrata é aquela que não pode ser instanciada  
Virtual serve para explicitar que um método pode ser sobrescrito  
String Interpolation  
Classes fechadas para  modificações  
Arrow Functions ou Bareless Function  
FluentValidator (dá para substituir com a solução sem estar em um pacote citada pelo próprio Baltieri em outro video)  
Utilização de notificações puras para tratar exceções (Notification Pattern)  
Code Contracts - Design By Contracts  
	Você desenvolve especificando coisas (menos ifs)  
01:09:00 - Explanação sobre a utilização de Validation Contract da Fluent Validator  

### Aula 7 - Testando o domínio
Testando validações simples de campos (Nome preenchido, tamanho de nome, etc...)  
04:00 - Regras para composição de nomes de teste  
Agrupamento de testes com TestCategory  

### Aula 8 - Revistando o domínio
Organização de Enums  
Criação de mestre detalhe (Pedidos X Items)  
06:06 - Por que usar IReadOnlyCollection para Lista de itens de um pedido  
07:30 - Obter subtotal do produto através de cálculo em um método  
	Não guardar campo total no banco  
08:25 - Obter total do pedido através de cálculo em um método que utiliza for each  
11:03 - Como fazer se for guardar o campo total e subtotal no banco  
11:50 - Criar método para adicionar itens detalhe  
42:00 - Por que utilizar testes (Exemplo do estoque = 18)  

### Aula 9 - Value Objects
Validação de CPF  
Com a utilização de value objects posso concentrar minhas validações específicas de campos em um só lugar  

### Aula 10 - CQRS Parte 1
CQRS = Divisão da aplicação entre leitura e escrita (Salva uma coisa no banco e mostra outra na tela)  
Fake Repository  
Site Gerador de CPF (http://geradordecpf.org/)  
Descobrir diferenças entre `ICollection`, `IEnumerable`, `IDictionary` e `IList`  
Estudar estrutura `pedido.Data:dd/MM/yyyy`  
Repository Pattern = uma unidade de acesso a dados para cada entidade, útil para mudar de banco no futuro, pois só ira mudar no repositório  
	Não fazemos a implementação do repositório no domínio, nele só fazemos a abstração através do uso de interfaces  
Utilização de interfaces para agrupar classes  
47:30 - Conceito de injecao de dependencias  
	Injecao de dependencia sempre trabalha com interfaces e um metodo construtor  
	
### Aula 17 - Segurança
Oauth = Open Authentication  
Não assisti tudo
