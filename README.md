<h1>Git</h1>

> Status do projeto: Em desenvolvimento

```
App.java
```
<h4> 
Para se adicionar alguém a um projeto, dando a esta pessoa a capacidade de editar diretamente o código basta: Entrar no repositorio atraves do Github e entrar en Settings(configurações). Dentro dos Setings tem uma parte escrita Access aonde tera o botão Collaborators. Dentro deste menu é posivel ver quem ja esta la anteriormente. Um pouco abaixo tem o Manage access. Dentro tem o botão Add people, aonde você pode procurar pelo usuario e ao clicar nele(a) da para convidar a pessoa e dar a ela direito de edição.

git clone: Ele mais o link do repositorio permitem que o mesmo seja copiado para dentro da maquina que executou o código.

git log: Exibe todos os logs de alterações feitas no código.

git log --oneline: Ele exibe os logs em uma unica linha de maneira simplificada. Exibindo também agora as mensagems de commit.

git pull: Ele mais o link do repositorio, serve para atualiza-lo caso outra pessoa mande algo para o repositorio. Baixando as modificações feitas. Sem o pull tudo o que ja esta na maquina do(a) dev seria sobre escrito.

git init - Este comando ira criar uma pasta oculta chamada .git .Esse processo inicia o
repositorio e permite que sejam armazenadas as mudanças no código

git status - Este comando mostra o status do repositorio. Mostrando se tem alguma coisa que
deva ser commitada ou se existem arquivos não rastreados(untracked)

git add . - Esse comando serve para rastrear e adicionar mudanças feitas em algum arquivo
e em toda a pasta do projeto.
O git não faz atualizações automaticas, ou seja, sempre que houver uma alteração no codigo
ou seja criado um novo arquivo ou pasta, é necessario utlizar o git add .

git add * - Faz a mesma coisa que o git add .

git add nome_do_arquivo - É possivel adicionar arquivos um por um. A prefer é utilizar 
o git add . .Mas nem sempre ele pode ser o melhor comando.

git commit -m 'Seu commit' - O git add adiciona o arquivo a algo chamado container. Ele
tecnicamente não faz parte do arquivo ele é só um historico. Para mandar o cantainer para
o git utiliza-se este comando. Ao utiliza-lo, os arquivos estão oficialmete no repositorio.
Você pode escrever o que bem quiser. Mas o certo é escrever em poucas palavras o que foi
alterado como 'Correção de bugs no arquivo x.py', 'Implemntada função de contagem' ou
'Criação de arquivo P.py'

git commit -am 'Seu comentário' - Este comado não apenas faz um commit, mas também 
adiciona as modificações do arquivo. Porem ele não tem a função de rastrear. Isso quer
dizer que esse comando é inutil se você criar um novo arquivo. Se criar outro arquivo
sera necessario utilizar o git add .

O git não faz mutiplas versões de um arquivo, ele simplesmente deixa em um arquivo o 
historico de alterações. Armazenando somente as alterações feitas

git checkout hash_do_ponto - Ao fazer um commit é criado um código para a alteração
do container. Com este código o git sabe o que foi feito em uma versão especifica do 
arquivo e permite que ela seja utilizada. Para obter esse numero é só utilizar o git log
e pegar o código depois da palavra commit

git checkout master - Fazendo isto se retorna para a versão mais recente do seu repositorio

git checkout nome_do_arquivo - Serve para descartar alterações feitas no arquivo

git diff - Com este comando é possivel ver a diferença entre o commit feito e o que você
alterou ou adicionou agora

git reset HEAD nome_do_arquivo - Este comando reseta o que esta dentro o container. 
Impedido que va para o repositorio

git branch - No Git existem os branches ou ramos. Eles servem para criar um tipo de clone
do seu repositorio, que permite que você altere tudo o que você precisar sem afetar o
repositorio de verdade. O simples comando git branch serve apenas para ver em qual branch
nós estamos.

git checkout -b ramo_nome - Este é o comado que cria um ramo em seu repositorio. Por 
padrão todos os commits que você fizer apos a criação do branch vão ser atribuidos a ele.
O branch funciona normalmente. Todos os comandos irão funcionar e todos os commits serão
herdados nesse branch.

git checkout master - Este comando serve para sair de detro do branch e retornar para o 
branch master. Ao voltar ao ramo master todas as alterações feitas no seu branch irão
"desaparecer". As alterações ainda existem, o que ocorre é que elas estão ligadas
somente ao branch.

git merge ramo_nome - Este comando server para unir o branch ao ramo master. O que foi 
alterado no branch ira ser adicionado ao master e ser parte do arquivo. Porem podem existir
conflitos. Por exemplo: Existe o aqrquivo CPF.py. Se na linha 1 da master estiver escrito
Numeros, e na linha 1 da branch estiver escrito digitos, isso ira gerar um conflito.
Para resolver este conflito, no Visual Studio Code aparece uma opção no arquivo, 
perguntando qual alteração você deseja aceitar. Escolha se você quer ficar com o que esta
no master ou no seu branch. 

git remote - Este comando verifica se esse repositorio existe no GitHub.

git remote add origin https://github.com/PauloASC/1_Git-Github.git - Este comando serve
para ligar o repositorio local ao repositorio no GitHub. Mas antes disso você precisa 
criar um repositório no GitHub com o mesmo nome da pasta do projeto. Não é  complicado.
Apenas faça login(caso não tenha um crie uma conta). Na pagina principal (github.com),
você ira encontrar um botão escrito New. De nome ao repositorio, coloque uma descrição se
desejar ou precisar. E para finalizar você deve clicar em create repository no final da 
pagina. Depois de criado você sera redirecionado para a pagina com o seu github vazio 
e algumas instruções, nelas o link que deve ser colocado junto ao comando git remote add origin

git push -u origin master - Ele ira dar o ponta pé para mandar o conteudo do repositorio
para o github. 

git push -u - origin master precisa ser adicionado somente na primeira vez em que você
faz o envio do repositorio. Todas as outras não necessitam disso

git pull - Este comando ira puxar para a sua maquina algum conteudo diferente ou novo que
esteja no github mas não em sua maquina.

</h4>
