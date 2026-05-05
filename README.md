# notas-estudo
minhas notas de estudo do téc SENAC 2026

markdown 


## configurando Git:

para utilizar o Git na minha maquina eu preciso configurar determinado comandos , sendo eles: Git --version para verificar se o git esta instalado, 

'''bash 
git config --global 
'''
## como configurar Github :
use os comados: Git config --global user.name "seu nome"
 Git config --global use.email "seuemail@gmail.com"

## SSH - Como configurar a maquina para GitHub :
verificar se existe chave ssh.
adicionar uma nova chave 
ssh-keygen -t ed25519 -c "your_email@exemple.com"
iniciar agente-ssh
eval "$(ssh-agent-s)"
adicione chave ssh no agente.
 ssh-add -/ssh/id_ed25519

## como criar um repositório :
entre no GitHub, vá em repositório aperte no botão "new" coloque um nome e uma descrição no repositorio e ative o README 

## REVISÃO

HTML- Marcação
SCC -  enfeitar 
JS -  manipular o DOM 

## ALERT:
serve para exibir uma mensagem
- Não recebe resposta
- Bloqueia a tela até o usuario confirma 
- ideal para exemplos simples e aprendizagem 

detalhe:
o código para e espera i usuário

## PROMPT:
ele ira nos permitir realizar duas ações
- mostra uma pergunta
- recebe uma resposta do usuário

detalhe importante:
toda reposta do prompt é texto (script), mesmo que o usuário digite um número.

## PROMPT + VARIÁVEIS
aqui nasce algo poderoso:guardar respostas.
- o valor digitais digitados pode ser armazenados 
- variáveis passam a ter significado real
- o codigo começa a reagir ao usuario sem varialvel, a resposta se perde.

## GETELEMENTBYID
função: retorna uma referencia ao elemento pelo seu ID 
Uso principal; selecionar elementos unicos em uma página para manipulação ou leitura de dados.
cosnt element = document.getElememntbtId('my-element');
element.style.color= 'blue'

## CREATEELEMENT
função: cria um novo elemento HTML
Uso principal: adicionar novos elementos á página dinamicamente.
cosn newDiv = document.createElement('div');
bewDiv.textContent = 'hello, world!';
document.body.appendchild(newDiv).

## APPENDCHILD
Função: adiciona um nó ( elemneto) como o último filho de um elemento pai especificado.
Uso peincipal: inserir elementos novos ou existentes na árvore DOM
const parent = document.getElementById('parent-element');
const child = document.createelement('p');
child.textContent = 'this is a new paragraph';
parent.appendChild(child);

## CLICK
didparado quando um elemento é clicado
const button = document.getElementById('my-button');
button.addEventListener('click', () => {alert('button was clicked');
});

## FUNÇÃO
por hora serão utilizadas apenas para reaproveitar código.
são declaradas da seguinte forma:
>function exemplo () {...
}
const buttonExercicio3 = document.getElementById("exercicio3")
buttonExercicio3.addEventListener('click', () => {exemplo()})

## IF/ELSE
o if e else são condicionais que permitem executar diferentes blocos de código com base em uma condição ou expressão booleana.

maria62065166@JLE106D060761 MINGW64 ~
$ cd Documents/

maria62065166@JLE106D060761 MINGW64 ~/Documents
$ git clone git@github.com:Dudadorn/OutroRepo.git
Cloning into 'OutroRepo'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

maria62065166@JLE106D060761 MINGW64 ~/Documents
$ cd OutroRepo/

maria62065166@JLE106D060761 MINGW64 ~/Documents/OutroRepo (main)
$ code .


function exercicio1() {
    alert("OIE")
}
// getElement
const batata = document.getElementById("exercicio1")
// addEventlistner
batata.addEventListener('click', () => { exercicio1() })


## HTML
O HTML (HyperText Markup Language) é uma linguagem de marcação usada para estruturar e organizar o conteúdo de páginas web. Ele define a disposição de elementos como textos, imagens, links, tabelas, vídeos e outros componentes que compõem uma página na internet. Apesar de ser essencial para o desenvolvimento web, o HTML não é uma linguagem de programação, pois não permite criar lógica ou manipular dados diretamente.

## CSS
-ESTILIZAÇÃO VISUAL: Define a apar~encia dos elementos,como cores, fontes, tamanho e estilo de bordas.
-LAYOUT E POSICIONAMENTO: Organiza o layout da página, controlando como os elementos são dispostos e como se comportam em diferentes tamanhos de tela(responsividade).
-RESPONSIVIDAE:Permite que as páginas se adaptam a diferentes dispositivos e tamanhos de tela, como desktops, tablets e smartphone.
-MANUTENÇÃO E CONSISITENCIAS: Facilita a manutenção do estilo através da separação da apresentação consistente e reutilizável em toda a aplicação.

## JS
- não e responsabilidade do HTML ou CSS dar dinamismo ou validar informaç~~oes.
- segue uma estrutura (sintaxe) própria.

-INTERATIVIDADE E DINAMISMO: JavaScript é o que transforma uma página estática em uma experi~encia viva: cliques. animações, feedback imediato, estados que mudam sem recarregar a página
-MANIPULAÇÃO DO DOM (DOCUMENT OBJECT MODEL):O DOM é a ponte entre JavaScript r o HTML real que o navegador renderiza. Manipular o DOM é, na prática, alterar a estrutura, o conteúdo e o estado visual da aplicação em tempo real.

## REACT
O React é uma biblioteca JavaScript de código aberto criada pelo Facebook, amplamente utilizada para construir interfaces de usuário (UI) interativas e eficientes. Ele permite o desenvolvimento de aplicações web modernas e escaláveis, utilizando uma abordagem baseada em componentes reutilizáveis. Esses componentes funcionam como blocos de construção que podem ser combinados para criar interfaces complexas, promovendo organização e manutenção simplificada no código.
 
COMPONENTIZAÇÃO: Facilita a manutrenção e reutilização de código.
DESEMPENHO: Virtual DOM melhora a performace.
COMUNIDADE: Grande suporte e muitas bibliotecas.

Vai no terminal digite npm o react-router-dom 
Depois vai na seta pra baixo e clica em git bash 
Em seguida vai em package.json e confere se foi depois crie uma pasta dentro  da pasta src com o nome pages 
Destro da pasta pages crie uma pasta com o nome About e Home dentro dessas pasta coloque uma pasta chamada índex.jsx e contra com o nome style.css
Depois vai em Main.jsx e nomeio dos códigos  StrictMode e App coloque o código <BrowserRouter>
Depois vai em App.jsx
Apaga o list e coloca <Rautes> e <Raute path =“/“ element ={Home} />
Abra a pasta Home e abra a pasta índex.jsx
Escreva import ‘./style.css’;
Function Home() {
Return ( 
<>
<h2> Bem vindo ao meu sistema </h2>
</>
)
}
Export default Home 

