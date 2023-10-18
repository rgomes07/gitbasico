# GIT comandos e estrutura básica:

> Acesse 2 livros em PDF no diretório PDFs do projeto e boa leitura.


**- O que é GIT**

**- Como instalar o GIT**
       
    - Linux
    - Mac
    - Windows
    
**- O que são Branchs**

**- O que é merger**

**- Principais comandos GIT**

**- Criando e salvando a chave SSH-key**

**- Escolha um octodex para seu perfil**

**- Referências**

![gitcat](images/gitcat2.jpeg)

# O que é GIT:

**Git** é um sistema de controle de versão distribuído moderno e amplamente utilizado no mundo. Foi desenvolvido para gerenciar projetos com alta rapidez e eficiência. O sistema de controle de versão nos permite monitorar e trabalhar em conjunto com os membros da nossa equipe no mesmo espaço de trabalho.

Git foi criado por Linus Torvalds em 2005 para desenvolver o Kernel Linux. Também é usado como uma importante ferramenta de controle de versão distribuída para DevOps.

Git é fácil de aprender e tem desempenho rápido. É superior a outras ferramentas SCM como Subversion, CVS, Perforce e ClearCase.

**Alguns recursos notáveis ​​do Git são os seguintes:**

**- Código aberto**

Git é uma ferramenta de código aberto. É lançado sob a licença GPL (General Public License).

**- Escalável**

O Git é escalável, o que significa que quando o número de usuários aumenta, o Git pode lidar facilmente com tais situações.

**- Distribuído**

Um dos grandes recursos do Git é que ele é distribuído. Distribuído significa que em vez de mudar o projeto para outra máquina, podemos criar um “clone” de todo o repositório. Além disso, em vez de ter apenas um repositório central para o qual você envia alterações, cada usuário tem seu próprio repositório que contém todo o histórico de commits do projeto. Não precisamos nos conectar ao repositório remoto; a mudança é armazenada apenas em nosso repositório local. Se necessário, podemos enviar essas alterações para um repositório remoto.

**- Segurança**

Git é seguro. Ele usa **SHA1** (Secure Hash Function) para nomear e identificar objetos em seu repositório. Arquivos e commits são verificados e recuperados por sua soma de verificação no momento do checkout. Ele armazena seu histórico de tal forma que o ID de commits específicos depende do histórico completo de desenvolvimento que leva a esse commit. Uma vez publicado, não é possível fazer alterações em sua versão antiga.

**- Velocidade**

O Git é muito rápido, então pode completar todas as tarefas em pouco tempo. A maioria das operações git são feitas no repositório local, proporcionando uma velocidade enorme. Além disso, um sistema centralizado de controle de versão se comunica continuamente com um servidor em algum lugar.
Os testes de desempenho realizados pela Mozilla mostraram que ele era extremamente rápido em comparação com outros VCSs. Buscar o histórico de versão de um repositório armazenado localmente é muito mais rápido do que buscá-lo no servidor remoto. A parte central do Git é escrita em C, que ignora as sobrecargas de tempo de execução associadas a outras linguagens de alto nível.
Git foi desenvolvido para funcionar no kernel Linux; portanto, é capaz o suficiente para lidar com grandes repositórios de maneira eficaz. Desde o início, **velocidade** e **desempenho** foram os principais objetivos do Git.

**- Suporta desenvolvimento não linear**

Git suporta ramificação e fusão contínuas, o que ajuda a visualizar e navegar em um desenvolvimento não linear. Uma ramificação no Git representa um único commit. Podemos construir a estrutura completa do branch com a ajuda de seu commit parental.

**- Branching and Merging**

Ramificação e fusão são os grandes recursos do Git, o que o torna diferente de outras ferramentas SCM. O Git permite a criação de múltiplas ramificações sem afetar umas às outras. Podemos realizar tarefas como criação, exclusão e mesclagem em ramificações, e essas tarefas levam apenas alguns segundos. Abaixo estão alguns recursos que podem ser alcançados por ramificação:

 - Podemos criar um branch separado para um novo módulo do projeto, confirmá-lo e excluí-lo sempre que quisermos.
 - Podemos ter um ramo de produção, que sempre tem o que entra em produção e pode ser mesclado para testes no ramo de testes.
 - Podemos criar um branch demo para o experimento e verificar se está funcionando. Também podemos removê-lo, se necessário.

O principal benefício da ramificação é que, se quisermos enviar algo para um repositório remoto, não precisamos enviar todas as nossas ramificações. Podemos selecionar algumas de nossas filiais ou todas juntas.

**- Garantia de dados**

O modelo de dados Git garante a integridade criptográfica de cada unidade do nosso projeto. Ele fornece um ID de commit exclusivo para cada commit por meio de um algoritmo SHA. Podemos recuperar e atualizar o commit por ID de commit. A maioria dos sistemas centralizados de controle de versão não fornece tal integridade por padrão.

**- Área de preparação**

A área Staging também é uma funcionalidade exclusiva do Git. Pode ser considerado uma prévia do nosso próximo commit, além disso, uma área intermediária onde os commits podem ser formatados e revisados ​​antes de serem concluídos. Quando você faz um commit, o Git pega as alterações que estão na área de teste e as transforma como um novo commit. Temos permissão para adicionar e remover alterações da área de teste. A área de teste pode ser considerada como um local onde o Git armazena as alterações.
Embora o Git não tenha um diretório temporário dedicado onde possa armazenar alguns objetos que representam alterações de arquivo (blobs). Em vez disso, ele usa um arquivo chamado index.

**- Mantenha o histórico limpo**

Git facilita com Git Rebase; É um dos recursos mais úteis do Git. Ele busca os commits mais recentes do branch master e coloca nosso código em cima disso. Assim, mantém um histórico limpo do projeto.

# Como instalar o GIT

Antes de começar a usar o Git, você tem que torná-lo disponível em seu computador. Mesmo se ele já tiver sido instalado, é provavelmente uma boa idéia atualizar para a versão mais recente. Você pode instalá-lo como um pacote ou através de outro instalador, ou baixar o código fonte e compilá-lo.


# Instalando no Linux

Se você deseja instalar o Git no Linux através de um instalador binário, você pode geralmente fazê-lo através da ferramenta básica de gerenciamento de pacotes que vem com sua distribuição. Se você usar Fedora por exemplo, você pode usar o yum:

**$ sudo yum install git-all**

Se você usar uma distribuição baseada em Debian como o Ubuntu, use o apt-get:

**$ sudo apt-get install git-all**

Para mais opções de instruções de como instalar o Git em outros vários sistemas Unix, veja na página do Git, em http://git-scm.com/download/linux.

# Instalando no Mac

Existem várias maneiras de instalar o Git em um Mac. O mais fácil é provavelmente instalar as ferramentas de linha de comando Xcode. No Mavericks (10,9) ou acima, você pode fazer isso simplesmente rodando git a partir do Terminal pela primeira vez. Se você não tiver o Git instalado, ele irá pedir-lhe para instalá-lo.

Se você quiser uma versão mais atualizada, você também pode instalá-lo através de um instalador binário. Um instalador OSX Git é mantido e disponível para download no site do Git, pelo http://git-scm.com/download/mac.


# Instalando no Windows

Há também algumas maneiras de instalar o Git no Windows. A compilação mais oficial está disponível para download no site do Git. Basta ir ao http://git-scm.com/download/win e o download começará automaticamente. Note que este é um projeto chamado Git para Windows (também chamado msysGit), que é algo separado do Git; para mais informações sobre isso, vá para http://msysgit.github.io/.

Para fazer uma instalação automatizada, você pode usar o pacote Git do Chocolatey. Note que o pacote Chocolatey é mantido pela comunidade.

Outra forma fácil de obter Git instalada é através da instalação de GitHub para Windows. O instalador inclui uma versão de linha de comando do Git, bem como a GUI. Ele também funciona bem com o PowerShell, e configura o cache de credenciais sólidas e as devidas configurações CRLF. Vamos saber mais sobre isso um pouco mais tarde, por enquanto basta dizer que estas são coisas que você deveria ter. Você pode baixá-lo da página GitHub para Windows, em http://windows.github.com.

# O que são Branchs

Uma ramificação (branch) é uma cópia dos arquivos no repositório no momento em que você cria a ramificação. Você pode trabalhar em sua branch sem afetar outras branchs. Quando estiver pronto para adicionar suas alterações à base de código principal, você poderá mesclar (merger) sua ramificação na ramificação padrão, por exemplo, principal.

# Criando uma branch

Para criar uma ramificação de recurso:

**git checkout -b "nome da branch"**

O GitLab impõe regras de nomenclatura de ramificações para evitar problemas e fornece padrões de nomenclatura de ramificações para agilizar a criação de solicitações de mesclagem.

# Mudar para uma branch

Todo o trabalho no Git é feito em um branch. Você pode alternar entre ramificações para ver o estado dos arquivos e trabalhar nessa ramificação.

Para mudar para uma ramificação existente:

**git checkout "nome da branch"**

Por exemplo, para mudar para o branch principal:

**git checkout principal**


# O que é merger

Vamos imaginar que o time que está desenvolvendo um projeto de um livro de receitas, decidiu que a segunda receita está pronta para ser adicionada ao livro, portanto, podemos fazer o merge da branch segunda-receita para a branch main.

# Mas o que é um merge?

O merge é a união de duas branches, onde você está unindo o conteúdo da branch A para a branch B. No nosso caso, estamos unindo a branch segunda-receita para a branch main.

Durante o merge você está pedindo para o Git, que ele faça a união das duas branches, mas o Git não vai fazer isso de qualquer forma, ele vai verificar se existe algum conflito entre as duas branches, se existir, ele vai te avisar e você terá que resolver o conflito manualmente.

Lembrando que o que queremos é adicionar todo o conteúdo novo que criamos na branch segunda-receita para a branch main.

# Vamos para a branch main.

**git checkout main**

Agora vamos fazer o merge da branch segunda-receita para a branch main.

**git merge segunda-receita**

O comando acima pediu para o Git pegar o conteúdo da branch segunda-receita e adicionar para a branch main, uni-las, atualizando a nossa branch main.

A saida do comando será algo parecido com isso:

**Updating 7def92f..9eb025b
Fast-forward
 README.md | 1 +
 1 file changed, 1 insertion(+)**


Se tivesse algum conflito para resolver, seria nesse momento que o Git iria reclamar e pedir para você resolver o conflito.

Lembrando que sempre você poderá utilizar o comando git log para verificar o histórico de commits do seu repositório.

O próximo passo é atualizar o nosso repositório remoto.

**git push origin main**

Pronto! Agora a nossa branch main está com o conteúdo da branch segunda-receita.

# Principais comandos GIT

# 1. Git clone

Git clone é uma comando para baixar o código-fonte existente de um repositório remoto (como, por exemplo, o git.seduc.pa.gov.br). Em outras palavras, git clone, basicamente, faz uma cópia idêntica da versão mais recente de um projeto em um repositório e a salva em seu computador.

Há algumas maneiras de baixar o código-fonte, mas, em geral, pode se usar o **SSH** e o **HTTP**.

**git clone http://git.seduc.pa.gov.br/ricardo.gomes/gitbasico**

Por exemplo, se eu quiser baixar um projeto do Gitlab SEDUC, tudo o que eu preciso fazer é clicar no botão azul (que diz "Clone"), copiar o URL da caixa logo abaixo e colá-lo após o comando git clone que mostrei logo acima.

![clonerepor](http://git.seduc.pa.gov.br/ricardo.gomes/gitbasico/-/raw/main/images/clonerepor.png)

Isso fará uma cópia do projeto no seu espaço de trabalho local para que você possa começar a trabalhar nessa cópia.

# 2. Git branch

Branches (algo como ramificações, em português) são altamente importantes no mundo do git. Usando as branches, vários desenvolvedores conseguem trabalhar em paralelo no mesmo projeto simultaneamente. Podemos usar o comando git branch para criar, listar e excluir as branches.

Como criar uma branch:

**git branch "nome-da-branch"**

Esse comando criará uma branch em seu local de trabalho. Para fazer o push (algo como enviar) da nova branch para o repositório remoto, você precisa usar o comando a seguir:

**git push -u "local-remoto" "nome-da-branch"**

Como ver as branches:

**git branch ou git branch --list**

Como excluir uma branch:

**git branch -d "nome-da-branch"**

# 3. Git checkout

Esse também é um dos comandos do Git mais usados para trabalhar em uma branch, primeiro, é preciso "entrar" nela. Usamos git checkout, na maioria dos casos, para trocar de uma branch para outra. Também podemos usar o comando para fazer o checkout de arquivos e commits.

**git checkout "nome-da-branch"**

Existem alguns passos que você precisa seguir para trocar de branch com sucesso:

> As alterações em sua branch atual devem estar em um commit ou em um stash antes de você fazer a troca.
  A branch na qual você quer fazer o checkout deve existir no seu espaço de trabalho local

Também existe um comando de atalho que permite criar e automaticamente trocar para a branch criada ao mesmo tempo:

**git checkout -b "nome-da-branch"**

Esse comando cria a branch em seu espaço de trabalho local (a flag -b representa a branch) e faz o checkout na nova branch logo após sua criação.

# 4. Git status

O comando git status nos dá todas as informações necessárias sobre a branch atual.

git status

Obtemos as seguintes informações:

    Se a branch em que estamos no momento está atualizada
    Se precisamos fazer o commit, push ou pull de algo
    Se os arquivos estão em fase de stage, fora dessa fase ou se não estão sendo rastreados
    Se arquivos foram criados, modificados ou excluídos

# 5. Git add

Ao criarmos, modificarmos ou excluirmos um arquivo, essas alterações acontecerão em nosso espaço de trabalho local e não serão incluídas no próximo commit (a menos que alteremos as configurações).

Precisamos usar o comando **git add** para incluir as alterações de um ou vários arquivos em nosso próximo commit.

Para adicionar um único arquivo:

**git add "arquivo"**

Para adicionar tudo ao mesmo tempo:

**git add -A**

> Importante: o comando git add não altera o repositório. As alterações não são salvas até que se use o git commit.

# 6. Git commit

Talvez esse seja o comando mais usado do Git. Quando chegamos a determinado ponto em desenvolvimento, queremos salvar nossas alterações (talvez após uma tarefa ou resolução de problema específica).

**Git commit** é como definir um ponto de verificação no processo de desenvolvimento. Você pode voltar a esse ponto mais tarde, se necessário.

Também precisamos escrever uma mensagem breve para explicar o que desenvolvemos ou alteramos no código-fonte.

**git commit -m "mensagem do commit"**

> Importante: git commit salva suas alterações no espaço de trabalho local.

# 7. Git push

Após fazer o commit de suas alterações, a próxima coisa a fazer é enviar suas alterações ao servidor remoto. Git push faz o upload dos seus commits no repositório remoto.

**git push "repositório-remoto" "nome-da-branch"**

Entretanto, se a sua branch foi recém-criada, também é preciso fazer o upload da branch com o seguinte comando:

**git push --set-upstream "repositório-remoto" "nome-da-branch"**

ou

**git push -u origin "nome-da-branch"**

> Importante: git push somente faz o upload das alterações que já estão em um commit.

# 8. Git pull

O comando git pull é usado para obter as atualizações de um repositório remoto. Esse comando é uma combinação de **git fetch** e **git merge**, o que significa que, quando usamos **git pull**, ele recebe as atualizações do repositório remoto (git fetch) e aplica imediatamente as alterações mais recentes em seu espaço de trabalho local (git merge).

**git pull "repositório-remoto"**

> Essa operação pode causar conflitos que você precisará resolver manualmente.

# 9. Git revert

Às vezes, precisamos desfazer as alterações que fizemos. Existem várias maneiras de se desfazer as alterações em nosso espaço de trabalho local ou remotamente (dependendo do que você necessita), mas devemos usar esses comandos com cuidado para evitar exclusões indesejadas.

# 10. Git merge

Quando você concluir o desenvolvimento em sua **branch** e quando tudo funcionar bem, a etapa final é fazer o **merge** (mesclar ou unir, em português) da branch com a branch pai (dev ou master/main, em geral). Isso é feito com o comando **git merge**.

Git merge, basicamente, integra sua branch com o recurso e todos os seus commits na branch de desenvolvimento (dev) ou na branch principal (master ou main). É importante lembrar que, primeiro, você precisa estar na branch específica na qual você quer fazer o **merge** de sua branch com o recurso.

Por exemplo, ao querer fazer o merge de sua branch do recurso na branch dev:

Primeiro, troque para a branch dev:

**git checkout dev**

Antes do merge, atualize sua branch dev local:

**git fetch**

Por fim, faça o merge da sua branch do recurso em dev:

**git merge "nome-da-branch-com-o-recurso"**

> Dica: certifique-se de que sua branch dev tem a versão mais recente antes de fazer o merge de suas branches de recurso. Do contrário, você pode ter que lidar com conflitos e outros problemas indesejados.

Esses são os 10 comandos mais usados do GIT para DEVOps.

# Criando e salvando a chave SSH-key

Antes de conectar o repositório local com o repositório remoto, precisamos adicionar a nossa chave SSH no Gitlab. Isso é necessário para que o Gitlab saiba que você é o dono do repositório e que você tem permissão para fazer alterações no repositório.

Você pode utilizar autenticacao via senha, mas vamos fazer da maneira mais elegante e segura, que é utilizando a autenticação via chave SSH.

Antes de mais nada, vamos criar uma chave SSH. Para isso, vamos utilizar o comando ssh-keygen.

**ssh-keygen -t rsa -b 4096 -C "Nossa chave SSH"**

O que esse comando faz é criar uma chave SSH com o algoritmo RSA, com 4096 bits e com a descrição Nossa chave SSH.

A saida do comando será essa:

    Generating public/private rsa key pair.
    Enter file in which to save the key (/home/ricardo.gomes/.ssh/id_rsa): /home/ricardo.gomes/.ssh/id_rsa_git
    Enter passphrase (empty for no passphrase): 
    Enter same passphrase again: 
    Your identification has been saved in /home/ricardo.gomes/.ssh/id_rsa_git
    Your public key has been saved in /home/ricardo.gomes/.ssh/id_rsa_git.pub
    The key fingerprint is:
    SHA256:+JCvAhk34WLjAbkDBA3IvtsaZBdEhMkV6CfmrrxkasQ Nossa chave SSH
    The key's randomart image is:
    +---[RSA 4096]----+
    |O=B*.            |
    |=*o .            |
    |+o o .           |
    |o=*.=  o         |
    |+*+O .+ S        |
    |oE=    +         |
    |o+o.    o        |
    |=+...  .         |
    |=+o  ..          |
    +----[SHA256]-----+
    
Eu criei a chave SSH com o nome id_rsa_git, mas você pode criar com o nome que quiser, o padrão é id_rsa.

Agora vamos adicionar a nossa chave SSH no GitLab. Para isso, vamos utilizar o comando ssh-add.

**ssh-add ~/.ssh/id_rsa_git**

Caso você já possua uma chave SSH, você pode utiliza-la sem problemas, normalmente ela fica em ~/.ssh/id_rsa.pub.

Agora vamos copiar a nossa chave SSH para o clipboard. Para isso, vamos utilizar o comando cat.

**cat ~/.ssh/id_rsa_git.pub | xclip -selection clipboard**

Se você não tem o comando xclip instalado, você pode instalar com o comando abaixo:

**sudo apt install xclip**

Agora vamos adicionar a nossa chave SSH no Gitlab:

    Vá até a página de configurações do Gitlab
    Depois em SSH and GPG keys
    Clique em New SSH key
    Cole a sua chave SSH no campo Key
    Adicione um título para a sua chave SSH no campo Title
    Click em Add SSH key

Pronto! Sua chave SSH foi adicionada com sucesso.

Agora volte no seu terminal e execute o comando abaixo:


**ssh -T git@git.seduc.pa.gov.br**

┌─(/rgomes/gitprojetos/gitbasico)───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────(rgomes@suricato:pts/1)─┐
└─(16:18:17 on main)──> ssh -T git@git.seduc.pa.gov.br                                                                                                                        ──(ter,out17)─┘
Welcome to GitLab, @ricardo.gomes!

Pronto! Agora você já pode conectar o seu repositório local com o repositório remoto, afinal você acabou de validar que a sua chave está correta.

# Octodex (octocat), use um octodex em seu perfil

![octocat](octodex/plumber.jpg)

Configure seu perfil com um octocat, acesse o diretório **octodex** do projeto e veja um mascote legal para customizar seu perfil.

# Referências:

    https://www.javatpoint.com/git
    https://git-scm.com/docs/gittutorial
    https://www.freecodecamp.org/portuguese/news/tutorial-de-git-e-github-controle-de-versao-para-iniciantes/
    https://embarcados.com.br/tutorial-git/   
    https://docs.gitlab.com/ee/gitlab-basics/start-using-git.html
    https://www.simplilearn.com/tutorials/git-tutorial
    https://octodex.github.com/
    https://productoversee.com/tudo-que-voce-queria-saber-sobre-git-e-github-mas-tinha-vergonha-de-perguntar/
    https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git
