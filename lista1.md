# Git (exercícios) - Lista 1

#### 1. Qual o comando para obter a versão instalada do Git? 
<pre> git version </pre> 

#### 2.Qual o efeito da execução de cada um dos comandos abaixo? 
####  a.git config -l 
<pre> O comando git config -l lista todos as configurações do úsuario em questão. </pre> 

#### b.git mv a.txt b.txt 
<pre> O comando é usado para renomear arquivos como a.txt para b.txt </pre> 
 
#### c.git reset --hard 
<pre> Reset os commit, passando a exibir o último commit </pre> 
 
#### d.git log -27 
<pre> Exibe os últimos 27 commits. </pre> 

#### e.git help 
<pre> Exibe os comandos e descreve a função de cada um. </pre>

#### f.git help reset 
<pre> Abre o arquivo  em um nova guia sobre explicações,exemplos do git reset. </pre>
 
#### g.git add --all 
<pre> O arquivo é mandado para staging area e preparado para ser considerado  no próximo commit.  </pre>

#### h.git add -u  
<pre> Adiciona os arquivos editados e que são monitorados pelo  Git .  </pre>

#### 3.O fluxo “clássico” de interação com o Git é algo como “realizar trabalho em um ou mais arquivos e diretórios”, “acrescentá-los para serem contemplados” e, finalmente, executar um “commit”. Quais os comandos necessários para realizar os dois últimos “passos” desse fluxo? 
Comandos para um arquivo ser acrescentado 
<pre>
git add ... 
git rm ... 
git mv... 
Executar um "commit" 
git commit... 
</pre>
#### 4.Qual o comando deve ser executado para identificar o que foi alterado desde o último “commit”? 
<pre> Git show comando usado para exibir o último commit. </pre>
 
#### 5.Em um dado repositório, arquivos simplesmente copiados para lá, ou seja, untracked, podem ser exibidos/identificados com que comando? 
<pre> git status</pre> 
#### 6.Qual o comando para efetuar um commit? 
<pre>Git commit -m "comentário sobre produto". </pre>

#### 7.Qual o comando que devemos empregar para descartar mudanças ocorridas no arquivo teste.txt, por exemplo? 
<pre> Git checkout -- <arquivo>... </pre>

#### 8.O que deve ser feito para que um determinado diretório do seu repositório seja ignorado pelo Git? 
<pre>Deve criar um arquivo .gitignore  para que assim ele seja ignorado pelo Git. </pre>

#### 9.O que acontece se o seu repositório local for removido? 
<pre>Haverá a perda do Repositório Local. </pre>

#### 10.Como clonar um repositório remoto? 
<pre>Git clone</pre>

#### 11.Em alguns cenários git log pode produzir extensos resultados. Se houver interesse em visualizar o histórico de um repositório, onde cada mudança é fornecida exatamente em uma única linha, qual o comando que deve ser empregado? 
<pre> git log --pretty=oneline </pre>
 
#### 12.Em qual arquivo o Git armazena informações de configuração empregadas por usuário? 
Armazena no arquivo 
<pre> ~/.gitconfig </pre>

#### 13.Qual o comando para criar um repositório local? 
<pre> Criar uma nova pasta ,abra-a e execute o comando git init.  </pre>

#### 14.Qual o nome do diretório criado pelo Git quando se executa o comando git init? 
<pre> O nome será o mesmo do repositório onde foi executado e endereço onde encontrar,como por exemplo , Reinitialized existing Git repository in C:/Users/keslley/Teste/.git/ 
</pre>
#### 15.Qual o comando para adicionar todos os arquivos modificados? (Aqueles para os quais git status identificam como modified?) 
<pre>Git add --all </pre>

#### 16.O Git faz uso do valor de hash conhecido por SHA1. O que isto significa? Qual o propósito? O que é SHA1? 
<pre> Git tem seu checksum (valor para verificação de integridade) calculado antes que seja armazenado e então passa a ser referenciado pelo checksum. Isso significa que é impossível mudar o conteúdo de qualquer arquivo ou diretório sem que o Git tenha conhecimento.O mecanismo que o Git usa para fazer o checksum é chamado de hash SHA-1.O SHA-1 é uma string de 40 caracteres composta de caracteres hexadecimais (0-9 e a-f) que é calculado a partir do conteúdo de um arquivo ou estrutura de um diretório no Git. 
</pre>
#### 17.Qual a palavra para indicar o último commit em vez do valor de hash SHA1 correspondente? 
<pre> -abbrev-commit </pre>

#### 18.Quando se cria dois arquivos usando um editor de texto qualquer e, na sequência, executamos o comando git add -u, os dois arquivos criados passam de untracked para new file? 
<pre> Não,pois git add -u adiciona os arquivos editados e que são monitorados pelo git. </pre>

#### 19.Qual o efeito da execução dos dois comandos abaixo, nesta ordem, em um dado repositório? 
<pre>
git reset --soft HEAD~1 ,git reset --hard 
git reset --soft HEAD~1 (volta ao último commit e mantém os últimos arquivos no Stage) 
git reset --hard(exibe o úlitmo commit) 
 </pre>
#### 20.Após o emprego de um ambiente integrado de desenvolvimento (IDE), é comum a criação de arquivos e diretórios. Qual o comando que podemos empregar para remover arquivos e diretórios untracked? 
<pre> Git clean -f </pre>

#### 21.Qual o nome do arquivo no qual podemos inserir a indicação para o Git de arquivos e diretórios a serem ignorados? 
<pre> arquivo .gitignore  </pre>

#### 22.Quando se cria o arquivo MinhaClasse.class em um dado diretório e desejamos que o Git ignore não apenas este, mas arquivos .class em geral, por todos os membros de uma equipe que estão contribuindo com um dado projeto? 
Basta colocar 
<pre>*.class  </pre>

#### 23.jQuery é uma famose biblioteca em JavaScript. Consulte detalhes em http://jquery.com. O repositório Git correspondente encontra-se disponível em https://github.com/jquery/jquery.git. Faça o clone deste repositório jqueryrepo. 

#### 24.No repositório jqueryrepo, criado no passo anterior, qual o efeito do comando git shortlog -sne? 
<pre> Exibe nome e email dos participantes. </pre>
 
#### 25.No repositório jqueryrepo, qual o efeito de git remote -v? 
<pre>Exibe a URL remota do diretirio jqueryrepo. </pre>

#### 26.Um repositório Git pode ser etiquetado ao longo do tempo. Ou seja, commits específicos podem ser “marcados” ou “etiquetados” para facilitar referências posteriores. Para listar todas as “etiquetas” (tags) estabelecidas para um dado repositório, qual comando deve ser executado? 
<pre>Deve ser executado git tag para listar todas as tags </pre>

#### 28.Caso um dato repositório retorne muitas “marcas” ou “etiquetas” para o comando git tag, como retornar apenas aquelas que atendem a determinado padrão, por exemplo, iniciadas por 2.0? 
<pre>git tag -a <nome>  </pre>

#### 29.Qual o efeito do comando git tag -a 3.4-gold -m “minha versão ouro”? 
A partir do comando cria uma tag e armazena com a mensagem "minha versão ouro". 
Após executado o comando acima, qual o efeito de git show 3.4-gold? 
<pre>Após executado vai exibir os dados da tag junto com o commit. </pre>

#### 30.O que o comando git push origin 3.4-gold teria como efeito? 
<pre>O comando mostra a informação da pessoa que criou a tag, a data de quando o commit foi taggeado, e a mensagem antes de mostrar a informação do commit. 
</pre>

#### 31.Após executar um commit, qual o efeito de git commit --amend? 
<pre> Usado para simplesmente editar a mensagem de commit anterior sem alterar o seu instantâneo. Funde o antigo commit com o novo(o antigo com corre 
</pre>
#### 32.Após executar git add x.txt, qual o efeito de git reset HEAD x.txt? 
<pre> O git reset HEAD x.txt retira o arquivo x.txt da staging Area </pre>

#### 33.Após alterar o conteúdo de um arquivo committed em passo anterior, qual o efeito do comando git checkout -- a.txt? 
<pre> Descarta as mudanças ocorridas no arquivo. </pre>

#### 34.Qual a diferença entre os comandos git reset HEAD x.txt e git checkout -- a.txt? 
<pre> O git reset HEAD x.txt retira o arquivo x.txt da staging Area,já o git checkout -- a.txt descarta as mudanças feitas no arquivo
</pre>











