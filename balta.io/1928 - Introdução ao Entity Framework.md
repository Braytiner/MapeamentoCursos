### Aula 1 - Introdução
A ideia principal do EF é ter o mapeamento das tabelas da fonte de dados  
	A ideia é ter um espelho da fonte de dados no sistema  
		A regra de negocio deve ficar na aplicação,  
			É mais fácil e prático  
			C# tem mais recurso que T-SQL  
			Visual Studio tem mais recursos que Management Studio  
			Dá para realizar testes unitários  
	Por isso existe a abordagem Code First, focada em gerar o banco baseado nos seus domínios  
	
A utilização de ORMs é semelhante a geração do banco que havia na época do GAS DOS  
	O DataContext é o mesmo arquivo de código que continha a definição de tabelas e campos no clipper  
	Migrations seria o arquivo que gerava o Adap  
Utilizamos Guid no lugar de int por questão de segurança, uma vez que um integer sequencial é sugestivo para que alguma operação ilegal externa seja executada: como é sequencial (1, 2, 3, etc...) um hacker pode executar um delete passando o id com um valor 4, enquanto que o guid gera um conjunto randomico, o que inviabiliza essa pratica  
ReportService no lugar de ORM para relatórios  
ORMs encontram lentidão em joins  
Inicializadores  
Fluent Mapping  

### Aula 2 - Imersão
Entity Frameworks PowerTolls

### Aula 3 - Tópicos Avançados
30:00 - Lazy Loading  
Migrations
