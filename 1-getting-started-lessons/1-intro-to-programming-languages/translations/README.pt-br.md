# Introdução a Linguagens de Programação e Ferraments do Mercado

Essa lição aborda os fundamentos das linguagens de programação. Os tópicos abordados aqui se aplicam à maioria das linguagens de programação modernas de hoje. Na seção "Ferramentas do Mercado", você vai aprender sobre softwares úteis que o ajudarão como desenvolvedor.

![Intro Programming](webdev101-programming.png)

> Sketchnote by [Tomomi Imura](https://twitter.com/girlie_mac)

## Questionário pré-aula

[Questionário pré-aula](https://nice-beach-0fe9e9d0f.azurestaticapps.net/quiz/1)

## Introdução

Nessa lição, nós vamos abordar:

- O que é programação?
- Tipos de linguagens de programação
- Elementos básicos de um programa
- Software e ferramentas úteis para o desenvolvedor profissional

## O que é programação?

Programação (também conhecido como codificação) é o processo de escrever instruções para um dispositivo, como um computador ou um celular. Nós escrevemos essas instruções com uma linguagem de programação, que é então interpretada pelo dispositivo. Esses conjuntos de intruções podem ser chamados de vários nomes, mas _programa_, _programa de computador_, _aplicativo (app)_ e _executável_ são os nomes mais populares.

Um _programa_ pode ser qualquer coisa escrita com código; websites, jogos e aplicativos de celular são programas. Embora seja possível criar um programa sem escrever código, a lógica subjacente é interpretada para o dispositivo e essa lógica provavelmente foi escrita com código. Um programa que está _rodando_ ou _executando código_ está carregando instruções. O dispositivo que você está lendo esta lição está rodando um programa para imprimir a lição para a sua tela.

✅ Faça uma pequena pesquisa: quem é considerado o primeiro programador do mundo?

## Linguagens de Programação

Linguagens de programação têm um propósito principal: para desenvolvedores criem instruções para enviar a um dispositivo. Dispositivos só podedm entender binário (1 e 0), e para a _maioria_ dos desenvolvedores, essa não é a maneira mais eficiente de se comunicar. Linguagens de programação são um veículo para comunicação entre humanos e computadores.

Linguagens de programção vêm em diferentes formatos e podem servir para propósitos diferentes. Por exemplo, Javascript é principalmente usado para aplicações web, enquanto Bash é principalmente usado para sistemas operacionais.

_Linguagens de baixo nível_ normalmente requerem menos etapas do que _linguagens de alto nível_ para um dispositivo interpretar as instruções. Contudo, o que torna as linguagens de alto nível populares é a sua legibilidade e suporte. Javascript é considerado uma linguagem de alto nível.

O código a seguir ilustra as diferenças entre uma linguagem de alto nível com Javascript de uma linguagem de baixo nível com código assembly ARM.

```javascript
let number = 10;
let n1 = 0,
  n2 = 1,
  nextTerm;

for (let i = 1; i <= number; i++) {
  console.log(n1);
  nextTerm = n1 + n2;
  n1 = n2;
  n2 = nextTerm;
}
```

```c
 area ascen,code,readonly
 entry
 code32
 adr r0,thumb+1
 bx r0
 code16
thumb
 mov r0,#00
 sub r0,r0,#01
 mov r1,#01
 mov r4,#10
 ldr r2,=0x40000000
back add r0,r1
 str r0,[r2]
 add r2,#04
 mov r3,r0
 mov r0,r1
 mov r1,r3
 sub r4,#01
 cmp r4,#00
 bne back
 end
```

Acredite ou não, _eles estão fazendo a mesma coisa_: imprimindo uma sequência de Fibonacci até 10.

✅ A sequência de Fibonacci é [definida](https://en.wikipedia.org/wiki/Fibonacci_number) como um conjunto de números tal que cada número é a suma de dois anteriores, começando em 0 e 1.

## Elementos de um programa

Uma única instrução em um programa é chama de _declaração_ e geralmente terá um caractere ou espaçamento de linha que marca onde a instrução _termina_. Como um programa termina varia com cada linguagem.

A maioria dos programas depende do uso de dados de um usuário ou de qualquer outro lugar, onde as declarações podem depender de dados para realizar as instruções. Dados podem alterar o comportamento de um programa, então as linguagens de programação vêm com uma maneira de armazenar dados temporariamente que podem ser usados posteriormente. Esses dados são chamados de _variáveis_. Variáveis são declarações que instruem a um dispositivo a salvar dados em sua memória. Variáveis em programas são semelhantes às da álgebra, onde têm um nome exclusivo e seu valor pode mudar com o tempo.

Há uma chance de que algumas instruções não sejam executadas por um dispositivo. Isso geralmente ocorre por design, quandp escrito pelo desenvolvedor ou por acidente, quando ocorre um erro inesperado . Esse tipo de controle de um aplicativo o torna mais robusto e sustentável. Normalmente essas mudanças em controle acontecem quando certas decisões são cumpridas. Uma instrução comum em uma linguagem de programação moderna para controlar como um programa é executado é a instrução `if..else`.

✅ Você vai aprender mais sobre esse tipo de instrução nas próximas lições

## Ferramentas do Mercado

[![Tools of the Trade](https://img.youtube.com/vi/69WJeXGBdxg/0.jpg)](https://youtube.com/watch?v=69WJeXGBdxg "Tools of the Trade")

Nesta seção, você vai aprender sobre alguns softwares que podem ser muito úteis ao iniciar sua jornada de desenvolvimento profissional.

Um **ambiente de desenvolvimento** é um conjunto de ferramentas e recursos que um desenvolvedor vai usar frequentemente ao escrever software. Algumas dessas ferramentas foram personalizadas para as necessidades específicas de um desenvolvedor e podem mudar com o tempo se um desenvolvedor alterar as prioridades de trabalho ou projetos pessoais, ou quando usar uma linguagem de programação diferente. Os ambientes de desenvolvimento são tão exclusivos quanto os desenvolvedores que os utilizam.

### Editores

Uma das ferramentas mais cruciais para desenvolvimento de software é o editor. Editores são onde você escreve seu código e algumas vezes inde você roda o código.

Desenvolvedores dependem de editoires por alguns motivos adicionais:

- _Depuração_ Descobrir bugs e erros percorrendo o código, linha por linha. Alguns editores têm recurso de depuração, ou podem ser personalizados e adicionados para linguagems de programação específicas.
- _Realce de sintaxe_ Adicionar cores e formatação de texto ao código, tornam-o mais fácil de ler. A maioria dos editores permite personalizar realce de sintaxe.
- _Extensões e Integrações_ Adições especializadas para desenvolvedores, por desenvolvedores, para acesso a ferramentas adicionais que não são incorporadas ao editor de base. Por exemplo, muitos desenvolvedores também precisam de uma maneira de documentar seu código e explicar como ele funciona, e instalarão uma extensão de verificação ortográfica para verificar erros de digitação. A maiorira dessas adições se destina ao uso em um editor específico, e a maioria dos editores vem com uma maneira de pesquisar as extensões disponíveis.
- _Costumização_ A maioria dos editores são extremamente personalizáveis, e cada desenvolvedor vai ter seu prório ambiente de desenvolvimento exclusivo que atende às suas necessidades. Muitos também permitem que desenvolvedores criem suas próprias extensões.

#### Editores Populares e Extensões de desenvolvimento web

- [Visual Studio Code](https://code.visualstudio.com/)
  - [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
  - [Live Share](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack)
  - [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Atom](https://atom.io/)
  - [spell-check](https://atom.io/packages/spell-check)
  - [teletype](https://atom.io/packages/teletype)
  - [atom-beautify](https://atom.io/packages/atom-beautify)

### Navegadores

Outra ferramenta crucial é o navegador. Desenvolvedores web dependem de um navegador para observar como seu código roda na web, também é usado para visualizar elementos visuais de uma página web escritas no editor, como HTML.

Muitos navegadores vêm com _ferramentas de desenvolvedor_ (DevTools) que contêm um conjunto de recursos e informações úteis para ajudar os desenvolvedores a coletar e capturar percepções importantes sobre suas aplicações. Por exemplo: se uma página web tem erros, às vezes é útil saber quando eles ocorreram. DevTools em um navegador pode ser configurado para capturar essas informações.

#### Navegadores populares e DevTools

- [Edge](https://docs.microsoft.com/microsoft-edge/devtools-guide-chromium?WT.mc_id=academic-13441-cxa)
- [Chrome](https://developers.google.com/web/tools/chrome-devtools/)
- [Firefox](https://developer.mozilla.org/docs/Tools)

### Ferramentas de Linha de Comando

Alguns desenvolvedores preferem uma visualização menos gráfica para suas tarefas diárias e contam com a linha de comando para fazer isso. O desenvolvimento de código requer uma quantidade significativa de digitação e alguns desenvolvedores preferem não interromper seu fluxo no teclado e usarão os atalhos do teclado para alternar entre as janelas da área de trabalho, trabalhar em arquivos diferentes e usar ferramentas. A maioria das tarefas pode ser concluída com um mouse, mas um benefício de usar a linha de comando é que muito pode ser feito com ferramentas de linha de comando sem a necessidade de alternar entre o mouse e o teclado. Outro benefício da linha de comando é que eles são configuráveis e você pode salvar a sua configuração personalizada, alterá-la posteriormente e também importá-la para novas máquinas de desenvolvimento. Como os ambientes de desenvolvimento são tão exclusivos para cada desenvolvedor, alguns evitarão o uso da linha de comando, outros dependerão dela inteiramente e alguns preferem uma combinação dos dois.

### Opções de Linha Comando populares

Opções para a linha de comando variam de acordo com o sistema operacional que você usa.

_💻 = vem pre-instalado no sistema operacional._

#### Windows

- [Powershell](https://docs.microsoft.com/powershell/scripting/overview?view=powershell-7?WT.mc_id=academic-13441-cxa) 💻
- [Command Line](https://docs.microsoft.com/windows-server/administration/windows-commands/windows-commands?WT.mc_id=academic-13441-cxa) (also known as CMD) 💻
- [Windows Terminal](https://docs.microsoft.com/windows/terminal/?WT.mc_id=academic-13441-cxa)
- [mintty](https://mintty.github.io/)

#### MacOS

- [Terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac) 💻
- [iTerm](https://iterm2.com/)
- [Powershell](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-macos?view=powershell-7?WT.mc_id=academic-13441-cxa)

#### Linux

- [Bash](https://www.gnu.org/software/bash/manual/html_node/index.html) 💻
- [KDE Konsole](https://docs.kde.org/trunk5/en/applications/konsole/index.html)
- [Powershell](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-linux?view=powershell-7?WT.mc_id=academic-13441-cxa)

#### Linhas de Comando Populares

- [Git](https://git-scm.com/) (💻 on most operating sytems)
- [NPM](https://www.npmjs.com/)
- [Yarn](https://classic.yarnpkg.com/en/docs/cli/)

### Documentação

Quando um desenvolvedor quer aprender algo novo, provavelmente recorrerá à documentação para aprender como usá=la. Os desenvolvedores geralmente contam com a documentação para orientá-los sobre como usar as ferramentas e linguagens de forma adequada, e também para obter um conhecimento mais aprofundado de como funciona.

#### Popular Documentation on Web Development

#### Documentações populares sobre desenvolvimento web

- [Mozilla Developer Network](https://developer.mozilla.org/docs/Web)
- [Frontend Masters](https://frontendmasters.com/learn/)

✅ Faça uma pesquisa: Agora que você já sabe o básico do ambiente de desenvolvimento web, compare e contraste com o ambiente de um web designer.

---

## 🚀 Desafio

Compare algumas linguagens de programação. Quais são alguns dos traçoes exclusivos de Javascript vs. Java? Que tal COBOL vs. Go?

## Questionário pós-aula

[Questionário pós-aula](https://nice-beach-0fe9e9d0f.azurestaticapps.net/quiz/2)

## Revisão e auto estudo

Estude um pouco sobre as diferentes linguagens à disposição do programador. Tente escrever uma linha em uma linguagem, e então refaça em outras duas. O que você aprendeu?

## Tarefa

[Lendo os dcoumentos](assignment.md)
