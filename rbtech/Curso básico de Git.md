# [Aula 1](https://www.youtube.com/watch?v=WVLhm1AMeYE&list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)

00:10 - Explicação do que é Git  
01:35 - Como funciona um controle de versão  
02:32 - Controle de versão centralizado e distribuído  
03:48 - Organização do fluxo de funcionamento do Git  
05:43 - Instalação e configuração do Git  

# [Aula 2](https://www.youtube.com/watch?v=-GhA2JPImgU&index=2&list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)
02:35 - Alterando a pasta inicial do terminal do Git  
04:54 - Criação do repositório local com o comando  `git init`  
05:50 - `gitstatus` para saber estado atual do repositório  
07:10 - Adicionando arquivos ao com `git add`  
09:55 - Commitando alterações com `git commit`  
12:18 - Ignorando arquivos com `git ignore`  
15:55 - Parâmetro `-a` do `git commit`  

# [Aula 3](https://www.youtube.com/watch?v=bDLEBDaS3ao&list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0&index=3)
00:55 - Visualizando alterações com `git diff`  
02:25 - Visualizando conteúdo da staged are com `git diff --stage`  
03:15 - `git log`  
  05:15 - Limitando quantidade de commits no log com parâmetro `-p`  
06:20 - Visualizando relatório de alterações com interface gráfica com `gitk`  


# [Aula 4](https://www.youtube.com/watch?v=dRV13jZqhU0&index=4&list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)
00:28 - Editando último commit feito com `git commit --ammend -m "Descricao"`  
03:47 - Removendo arquivo adicionado por engano com `git reset HEAD "nomedoarquivo"`  
04:30 - Revertendo alterações com `git checkout -- nome do arquivo`  
08:20 - Apagando arquivos do repositorio com `git rm nomedoarquivo`  

# [Aula 5](https://youtu.be/Fhd8OKIDQ5M?list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)

00:15 Tags
  `git tag -a -m`  
  A tag sempre é criada no commit atual  
  02:20 Criando tags em  outros commits  
  04:15 Revertendo para tags anteriores  
  05:25 Apagando tags  

06:00 Branches
  06:53 Utilizando branches para criar diferentes ambientes (produção, teste e desenvolvimento)  
  08:28 `git checkout`para fazer transição entre as branches, `git checkout -b nomedabranch` cria e faz o checkout de uma vez só  
  09:30 Mesclando alterações entre branches com `git merge` (é necessário estar na branch que será o destino das alterações)  
  13:45 Corrigindo conflitos de merge entre branches  
 
# [Aula 6](https://youtu.be/fRQrnWqDLn0?list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)
00:10 Configurando o controle de versão em uma rede local  
04:10 `git --bare` cria um repositório que será compartilhado com outras máquinas  
05:10 `git clone file:////nomedoservidor/pasta nomedorepositoriolocal`  
09:20 Enviando alterações para o servidor com `git push nomedoremoto nomedabranchlocal`  
13:28 Trazendo alterações do servidor com `git pull nomeremoto nomedabranchremota`  
      O `git pull` faz o merge automaticamente, para não realizar o merge automaticamente utilize o `git fetch nomeremoto branchlocal`  

# [Aula 7](https://youtu.be/1IfAFYQD8u0?list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)
00:10 Utilizando o Git em conjunto com Github  
02:00 Dando acesso a uma maquina local a conta do Github  
04:12 Criando um repositório  
06:15 Clonando o repositório  
09:00 Enviando alterações para o repositório remoto  

# [Aula 8](https://youtu.be/mGeIFe-pDow?list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)
00:35 Colaborando com outros projetos no Github  
00:53 `Fork` clona um determinado repositório para sua conta no Github  
01:02 `Pull request` abre uma requisição para que as alterações realizadas sejam analisadas e integradas ao projeto principal  
07:50 Apagando um repositório do Github

