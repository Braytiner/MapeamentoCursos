### Aula 4 - Organizando a solução
Caminho seguro = sem espacos, na unidade padrão, sem caracteres especiais, etc...

### Aula 7 - Separação em contextos delimitados
Basicamente trata da organização de áreas do projeto, a fim de dividir um projeto em partes menores o que pode facilitar a reescrita de um projeto. Por exemplo, em um ERP: Contexto financeiro, contexto de relatórios, etc... A divisão pode ser feita por pastas, projetos ou até mesmo solutions.

### Aula 8 - OOP
A classe não é um objeto, ela é um molde do qual os objetos irão se formar  
Explicação da importancia da divisão logica de namespaces  
	Existe a divisão física com a qual estruturamos nosso projeto   
	
### Aula 10
05:00 - Modificador Sealed impede que uma classe seja herdada  
06:00 - Abstract impede que a classe seja instanciada  

### Aula 11 - OOP: Interfaces e sobrescrita  
Interface permite herança multipla (lado pratico dessa herança)  
Todo objeto no .NET tem um metodo `ToString()`  

### Aula 12 - Definindo as entidades
Método para mapeamento de entidades  
17:20 - Não precisa colocar o id do pedido na classe item de pedido

### Aula 15 - Value Objects
Uma boa dica para discernir VO é que estes não serão armazenados em tabelas separadas no banco  
08:40 - Quando trabalhar com Endereco como VO e como Classe  

### Aula 16 - Collections
Por convenção, o nome todo objeto private a ser utilizado na classe deve começar com _  
02:00 - Retornando conteudo de uma propriedade armazenada em uma lista private através do método get  

### Aula 17 - Modelando o pedido
Usando o ForEach como método de uma lista para percorrer esta lista  

### Aula 19 - Exceptions e validações
Exceptions são exceções (algo que você não espera) então se você usa o if para tratar um erro, é por que está esperando algo, então não é certo utilizar exceções nesse caso, até mesmo por que consomem muitos recursos do servidor, pois vai no processador e no event viewer do windows.  
Utilizaçao pura de notificações em o FluentValidator  

### Aula 20 - Implementando notificações
08:00 - Melhor explicação para ValidationContract  

### Aula 21 - Compartilhando informações em contextos delimitados
05:20 - Shared Context

### Aula 23 - Testando VOs
Estudar Testes  
Melhor explicação e assimilação de testes do que o curso 1969  
Uma unidade de teste nada mais é que uma classe comum decorada com [TestClass] que possui os seus métodos decorados com [TestMethod]  
Padrão de testes RedGreenRefactor  
Assert em inglês significa assegure

### Aula 24 - Testando Domains
Ótima abordagem para identificar quais testes serão realizados  
	Comece olhando o domínio e identificando os principais métodos e ações mais complexas (dentro destes métodos) que necessitam ter comprovação/corroboração de que estão funcionando
	
### Aula 25 - CQRS
Banco separado para relatórios para não onerar produção  
Event Sourcing

### Aula 26 - Commands
Commands são bem parecidos com Value Objects, porém são objetos somente de entrada de dados, onde serão consolidados todos os parâmetros necessários para realizar uma determinada ação dentro de um objeto

### Aula 27 - Criando o primeiro command
05:00 - Basicamente, o command irá refletir a estrutura do banco de dados em uma classe  
	Por exemplo o Value Object Name que contém as propriedades FirstName e LastName seria mapeado na classe do command como string FirsrName e string LastName  
05:17 - Explicação sobre como trabalhar com listas de detalhe e commands

### Aula 28 - Criando os demais commands
06:00 - Explicação sobre como trabalhar com listas de detalhe e commands

### Aula 29 - Fail Fast Validations
Quando o usuario inputar os dados na aplicacão, estes serão convertidos em Json e logo após se tornará em um command  
FastFailValidations são as validações mais simples realizadas no Command  
O método Valid da classe Notifiable retorna se o objeto é válido (ótimo para realizar as validações)  
  05:28 Fluxo da Fail Fast Validations do frontend até o backend

### Aula 30 - Aplicando validações
Fazendo validações no command

### Aula 31 - Testando Commands

### Aula 32 - Handlers
O handler é um objeto que irá realizar todos os passos necessários ao receber um Json de um determinado objeto

### Aula 33 - Criando um handler

### Aula 34 - Repositorios
02:47 - Para o dominio sempre irá chegar um Ilist, o repositório que é responsavel por passar essa lista já "mastigada" para o dominio

### Aula 35 - Serviços
São abstraidos na camada de dominio atraves de suas interfaces por que fazem parte da regra de negocio, mas são implementados na camada Infra
