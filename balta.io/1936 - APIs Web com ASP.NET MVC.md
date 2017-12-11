# 1936 A - Introdução

### Aula 1 - Introdução ao WebAPI

### Aula2 - Criando o alicerce
Criando aplicação com Repository Pattern e sem injeção de dependencias tanto no ASP.Net MVC quanto no Web API

### Aula 3 - CRUD

#1936 B - Padronização

### Aula 1 - Padronizando os retornos com HTTP Message
09:00 Montando um http message

### Aula 2 - Padronizando as propriedades dos objetos de retorno

### Aula 3 - Padronizando Rotas e Url
03:53 RoutePrefix e Route  
06:36 Padrao de nomenclatura  
08:55 Rotas com parametros  
10:40 Rota com skip e take  
13:29 Versionamento  

# 1936 C - Performance

### Aula 1 -  Melhorando o alicerce. ORM vs ADO
Recomendação para assitir o treinamento Acesso a dados com Entity Framework (treinamento anterior ao 1936)  
10:30 AppInsights e Fiddler para medir o tempo de cada chamada  
14:10 Pequena abordagem sobre utilização de OnPremise e Cloud  
18:10 Camada de serviços  
	Explicacão de por que usar  
	O repositório trabalha manipulando o objeto completo com todas as suas propriedades, em alguns casos não iremos precisar de todas as propriedades, somente de algumas (um exemplo claro, é quando iremos gravar um produto, onde não precisamos do id, pois o mesmo será gerado pelo banco de dados [isso pode parecer pouco, mas se tratando em vários usuarios pendurados em um mesmo banco dá uma diferença no custo de cloud computing]), por isso junto com este exemplo ele utiliza o recurso de ViewModels  

### Aula 2 - Limitando o retorno de dados
03:45 Expondo somente o necessário para a interface  
04:30 Limite o numero de registros com Skip e Take  
	Limite no repositório e não apenas na API  
	Utilização de Odata para filtrar (filtrar via url)  
11:45 Como o banco interpreta o skip e take  

### Aula 3 - Utilizando outros serializadores
Existe um tempo para a conversão do objeto List<Entidade> para o Json que será retornado para o frontend  
03:00 Quadro comparativo de tempo entre serializadores  

### Aula 4 - Implementando compressão
Fiddler

### Aula 5 - Implementando caching

### Aula 6 - Utilizando Async
Utilizacao de tasks para liberacao do processador do IIS  

### Aula 7 - Retornando múltiplos resultados
02:47 Toda vez que você cai na declaração do DataContext dentro da Controller você iniciou uma requisição  
04:00 Criação de uma viewmodel para Dashboard  
08:20 Para trazer registros de diferentes tabelas em apenas uma requisição, trabalhe com objetos aninhados  

# 1936 D - Parte 4: Segurança

### Aula 1 - Autenticação básica
08:04 Para fazer uma autorização customizada, basta criar uma classe que herda de AuthorizationFilterAttribute e sobrescrever o método OnAuthorization  
09:15 Montando o cabeçalho com a autenticação no postman  
10:58  Obtendo no nome de usuario e senha do cabeçalho  
18:00 Quando usar  

### Aula 2 - Autenticação via token
05:20 Owin  
06:45 Pacotes a instalar  
https://weblogs.asp.net/andrebaltieri  

### Aula 3 - Limitando o acesso a API
Limite o acesso por Ips de um determinado país  
Limite o acessco por um determinado dominio  

# 1936 E - Outros

### Aula 1 - CORS
Cross Origin Resource Sharing

### Aula 2 - Deploy para Azure Website
Existem três modelos de entrega para subir as aplicações: WebSite, Cloud Service e VM

# 1936 F - vNext
