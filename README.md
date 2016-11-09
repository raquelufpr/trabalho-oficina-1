TRABALHO DE OFICINA DE COMPUTAÇÃO

# JOGO EM RACKET/SCHEME

(Vale 60% da nota, sendo 40% os exercícios)


## INSTRUÇÕES GERAIS:


1. Primeira parte:
	1. Escolha um jogo e apresente a ideia ao professor;
	2. Escreva uma especificação mais detalhada (o que o jogo vai ter?)
	3. Faça a análise de domínio inicial utilizando a receita Como Projetar Mundos
	4. Entregue ao professor a especificação e análise de domínio na data definida (12/10).
2. Crie um repositório no GitHub para o seu projeto ou faça um fork do projeto inicial fornecido pelo professor. Todo o trabalho deverá ser feito utilizando o controle de versão. A utilização desta ferramenta contará pontos na avaliação do trabalho.
3. Mãos ao código. Escreva o código seguindo as receitas de projeto, com base na análise de domínio realizada.
4. Apresentação de acompanhamento: em data definida (abaixo), deverá apresentar uma versão em funcionamento básica (no mínimo 70% feito), mas ainda em desenvolvimento.
5. Entrega e apresentação final

    OBS: Cada dupla deverá desenvolver um jogo diferente! Portanto peço que aqueles que tem preferência por um jogo específico  me informem qual desejam fazer o mais rápido possível. Acima tem sugestões de possíveis jogos que vocês podem fazer com algumas especificações mínimas (o jogo não poderá ser nem muito simples nem muito complexo, por isso deverão me apresentar a especificação e análise de domínio com antecedência).

## DATAS:

- DATA DA ENTREGA DA ESPECIFICAÇÃO E ANÁLISE DE DOMÍNIO: 12/10

- DATAS DE ENTREGAS DE CHECKPOINTS: A DEFINIR ENTREGA NO MOODLE.

- DATA DE APRESENTAÇÃO DE ACOMPANHAMENTO (MÍNIMO 70% FEITO E FUNCIONANDO BOA PARTE DAS COISAS): 16/11 e 17/11

- DATA DE ENTREGA E APRESENTAÇÃO FINAL: 14/12 e 15/12

    A proposta deve consistir em um documento explicando o objetivo do jogo, os elementos da tela, assim como uma análise de domínio inicial (conforme receita Como Projetar Mundos)
    Na apresentação individual, cada aluno deverá explicar ao professor como o programa foi desenvolvido e responder questionamentos do professor sobre o programa.

## CRITÉRIOS DE AVALIAÇÃO:

- Utilização das receitas de projeto: as funções devem ser escritas utilizando as receitas de projeto. Todas as funções devem ter testes. (Peso 3)
- Corretude e completude: os programas têm quer passar em todos os testes (e os testes devem estar corretos e com 100% de cobertura de código – exceto para função main / big-bang, que não precisa fazer teste unitário). (Peso 3)
- Boas práticas de programação: o código deve estar bem escrito e organizado; os recursos da linguagem devem ser usados corretamente. (Peso 3)
- Utilização do controle de versão: o histórico de commits será avaliado pelo professor a fim de verificar se o controle de versão foi utilizado corretamente. (Peso 2)


## INSTRUÇÕES DE PREPARAÇÃO DE AMBIENTE DE DESENVOLVIMENTO E USO DO GIT

O projeto deverá ser feito utilizando o SCV (Sistema de Controle de Versão) Git hospedado no GitHub. Para isso o recomendado é seguir os seguintes passos:

0. Primeiro é necessário se cadastrar no GitHub. Cada membro da equipe deve se cadastrar. Um dos membros (o que for fazer o fork, vide passo 1) deverá compartilhar o projeto para escrita ou administrar.

1. Criar um fork. Fazer um fork (do inglês, "garfo") de um projeto é pegar um projeto de código aberto existente e copiá-lo como um projeto próprio. Assim, é possível modificá-lo como se fosse seu próprio projeto. Quando você faz um fork de um projeto existente, vocês está criando uma nova ramificação dele.
	1. No GitHub, entre na página do projeto e clique em Fork.
	2. Pronto! Você já criou seu projeto. Explore a página do GitHub do seu projeto.
	3. Compartilhe o projeto com seu colega: No GitHub, no canto superior direito da página do projeto, clique em Settings. Vá em Collaborators e insira o nome de usuário de seu colega. Ele receberá um email aceitando o convite para ser colaborador do projeto, e poderá fazer 'push', como explicado abaixo.

2. Clone seu projeto.
	1. Na página do seu projeto "forkado", clique em Clone. Um comando aparecerá. Copie e cole no terminal. Se não tiver o Git instalado ainda, instale no Linux com 'sudo apt-get install git -y', e no Windows por meio de instalador. 
		1. Se estiver usando TortoiseGit no Windows, clique com o botão direito na pasta e procure a opção Clone. Cole o endereço do projeto onde for pedido. O mesmo se aplica aos demais comandos do Git: procure o equivalente na interface gráfica.
	2. Pronto! Seu repositório com o projeto já está em sua máquina.

3. Trabalhe no projeto
	1. No decorrer do projeto, é importante dar commit (consolidar) nas mudanças realizadas. Prefira dar commit sempre que você adiciona algo relevante, mesmo que seja mínimo.
		1. Primeiro, entre na pasta raiz de seu projeto e rode o comando 'git add --all'. Este comando fará o Git considerar todas as mudanças realizadas no projeto.
		2. Em seguida, rode o comando 'git commit -m "Mensagem de commit"'. Este é o comando que efetivamente fará o Commit em sua máquina (ainda não envia para o GitHub). A mensagem de commit é muito importante. Escreva nela resumidamente o que foi modificado neste último commit.
			1. Pode ser que apareça uma mensagem dizendo para você dizer quem é você. Ele irá sugerir que você execute alguns comandos para configurar seu nome e email. Os comandos são: 'git config --global user.email "you@example.com" && git config --global user.name "Your Name"'. Depois de feito isso, tente fazer novamente o commit.

	2. Após dar commit, suas alterações ainda não estarão no repositório do GitHub. É necessário fazer um Push (empurrar, "mandar pra frente"). Para isto, logo após realizar o commit, digite o comando 'git push'. Digite seu usuário e senha do GitHub. Confira se a alteração chegou no GitHub acessando a seção Commits do site.

4. Trabalhando em equipe
	1. Os commits e pushs constantes são necessários para coordenar o trabalho em equipe. Por isso, revisem o passo 3.
	2. Quando seu colega fez um commit e push, é necessário que você puxe suas alterações. Para isso, é necessário dar um Pull (puxar). Rode o comando 'git pull'.
	3. Pronto! As alterações do seu colega já estarão atualizadas na sua máquina e vocês estarão sincronizados.
	4 Se houver conflito (modificações na mesma linha de código), o Git irá avisar. Dê um 'git pull'. Entre no arquivo que deu conflito. Você verá que estará marcadas as duas versões. Apague a versão incorreta, deixando do modo como o código deve ficar. Dê um 'git add --all' seguido por um commit, deixando na mensagem que foi feito um merge (mescla) manual. Dê git push.
		
OBS: É possível executar todas as ações (e até utilizar mais recursos visuais) por meio de uma interface gráfica para o Git, instalada separadamente. No Windows recomenda-se o TortoiseGit. No Linux existem também várias opções, como o git-cola, RabbitVCS, syntevo, etc.




## INSTRUÇÕES PARA DESENVOLVIMENTO

Vocês podem desenvolver o programa em um único arquivo durante o desenvolvimento. No entanto, o ideal (contará mais nota) é se o trabalho final for entregue na linguagem Racket seguindo o padrão de separação dos arquivos do projeto inicial. Ou seja, a função main / big-bang deverá estar definida em "main.rkt", as demais funções do jogo (lógica e visão do jogo) deverão estar definidas em "jogo.rkt", as constantes em "constantes.rkt", as definições de tipos de dados em "dados.rkt", e os testes em "testes.rkt". Todos os arquivos já possuem um template que incluem as importações entre arquivos. 

A separação modular do programa, que deixa o código mais limpo, só é possível se o programa estiver implementado na linguagem Racket.



## INSTRUÇÕES PARA ENTREGA

O Trabalho deverá ser entregue até a data marcada, até 23:59, por e-mail. Vocês deverão enviar no Moodle o link do repositório no GitHub e um pacote .zip com os arquivos do projeto com o nome da dupla, dessa maneira: Fulano_Beltrano.zip. Caso faça sozinho, coloque somente seu nome.



