# Configurando o Arduino Nano 33 BLE Sense
###### Autora: [Letícia Morais](https://github.com/letsticia)

Nesta seção, iremos aprender a configurar o [Arduino Nano 33 BLE Sense](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense) para que seja possível conectá-lo aos seus projetos no [_Edge Impulse_](https://edgeimpulse.com/).

### Hardware e Software Necessários para a configuração

É necessário um computador e acesso à Internet para a instalação das dependências assim como para a criação da conta no [_Edge Impulse_](https://edgeimpulse.com/).

* Uma conta no Edge Impulse é necessária para o [Edge Impulse Studio](https://edgeimpulse.com/);

* É necessário instalar o [_Edge Impulse CLI_](#2-instalando-o-edge-impulse-cli) e suas [dependências](#passo-21-instalando-o-python) para a conexão com o [_Edge Impulse_](https://edgeimpulse.com/);

* É necessário instalar o [_Arduino CLI_](https://arduino.github.io/arduino-cli/0.35/) para o reconhecimento da porta que o microcontrolador estará;

* É necessário o microcontrolador [Arduino Nano 33 BLE Sense](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense) e seu cabo de conexão micro-USB.


## 1. Criando uma conta no [_Edge Impulse_](https://edgeimpulse.com/)

O [_Edge Impulse_](https://edgeimpulse.com/) é uma plataforma que permite que criemos (e/ou otimizemos) nossos próprios modelos de de _machine learning_ visando embarcar em microcontroladores e/ou em dispositivos móveis.

Dessa forma, é imprecindível a criação de uma conta nesta plataforma para, enfim, podermos embarcar e criar nossos próprios algoritmos de TinyML. Caso já possua uma conta, você pode pular essa parte e ir para a [próxima](#2-instalando-o-edge-impulse-cli).

### Passo 1.1: acessando a página de cadastro

Clincando [neste link](https://studio.edgeimpulse.com/signup), você será redirecionado para a tela de cadastro do Edge Impulse, conseguindo ver essa página:

<div>
  <img src= assets/image.png>
</div>
<i>Tela de Cadastro do Edge Impulse</i>

### Passo 1.2: preenchendo os dados necessários

Nos campos acima, são necessários o seu nome (ou como você quiser que apareça na plataforma), um nome de usuário único, um e-mail (podendo ser pessoal, da empresa ou da sua faculdade) e uma senha.

Também é necessário aceitar a caixinha que faz com que você concorde com a política de privacidade do site, assim como os termos de serviço da comunidade e, por último, a licença de IA responsável.

Por fim, clique no botão azul escrito _Sing Up_ e sua conta será    criada. Se você tiver preenchido todos os dados necessários, uma tela parecida com essa deve aparecer em seu navegador:

<div>
  <img src=assets/image-1.png>
</div>
<i>Criação de conta no Edge Impulse</i>

### Passo 1.3: Criando o primeiro projeto

Se você clicar no botão roxo da imagem acima, o _Edge Impulse_ irá criar um projeto com o nome (seunome-projec-1) redirecionando para a página inicial deste. 

<div>
  <img src=assets/image-2.png>
</div>
<i>Primeiro projeto no Edge Impulse</i>

Agora, iremos instalar as dependências necessárias para que o site do edge impulse reconheça que há um [Arduino Nano 33 BLE Sense](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense) conectado a este projeto.

# 2. Instalando o Edge Impulse CLI

Esta [_Edge Impulse CLI_](https://docs.edgeimpulse.com/docs/tools/edge-impulse-cli/cli-installation) é uma _command-line interface_ (ou Interface de linha de comando, traduzindo para o português) que permite que o usuário faça operações envolvendo o edge impulse e seu microncontrolador a partir de comandos via terminal.

### Passo 2.1: instalando o python

Para uma execução bem sucedida da [_Edge Impulse CLI_](https://docs.edgeimpulse.com/docs/tools/edge-impulse-cli/cli-installation) é necessário ter uma versão do Python 3 em seu computador. Caso você já o possua, passe para o [próximo passo](#passo-22-instalando-o-nodejs-e-suas-ferramentas-adicionais).

Para ir para a página de downloads do Python [clique aqui](https://www.python.org/downloads/). Nesta página você irá baixar o instalador do python referente ao seu sistema operacional. 


<div>
  <img src=assets/image-3.png>
</div>
<i>Página de downloads do Python</i>

#### Após o download do instalador, abra o programa, selecione as duas caixas de marcação e, por fim, selecione "Install now" para iniciar a instalação. 

<div>
  <img src=assets/image-4.png>
</div>
<i>Imagem retirada do site Python.org</i>

#### Se a instalação for bem sucedida, essa será a tela exibida.

<div>
  <img src=assets/image-5.png>
</div>
<i>Imagem retirada do site Python.org</i>

Você pode testar a execução do Python abrindo o seu terminal e digitando `python --version`, a saída esperada é:

``` python <versão que você instalou>```

### Passo 2.2: Instalando o Node.js e suas ferramentas adicionais

Assim como o python, o Node.js é um pré-requisito para um bom funcionamento da [_Edge Impulse CLI_](https://docs.edgeimpulse.com/docs/tools/edge-impulse-cli/cli-installation). Dessa forma, é importante fazer sua instalação e de suas ferramentas adicionais. Se você já tiver o Node.js e suas ferramentas instaladas, você pode ir para o [último passo](#passo-2.3-instalando-a-edge-impulse-cli) da [seção 2](#2-instalando-o-edge-impulse-cli). 

Caso você não saiba como instalar o [Node.js](https://nodejs.org/en/), neste [link](https://www.alura.com.br/artigos/como-instalar-node-js-windows-linux-macos), há um artigo do alura, em português, com um tutorial para a instalação correta em cada sistema operacional. 

### Passo 2.3: Instalando a Edge Impulse CLI

Se você tiver todas as dependências instaladas, basta abrir o prompt de comando e digitar o seguinte código para a instalação da [_Edge Impulse CLI_](https://docs.edgeimpulse.com/docs/tools/edge-impulse-cli/cli-installation):

* Windows:
``` 
npm install -g edge-impulse-cli --force 
```

* Linux:

```
npm install -g edge-impulse-cli
```

## 3. Instalando a [_Arduino CLI_](https://arduino.github.io/arduino-cli/0.35/)

Agora iremos instalar a última dependência, a [_Arduino CLI_](https://arduino.github.io/arduino-cli/0.35/). Ela é necessária porque é este programa quem irá detectar os microcontroladores que estão no nosso computador. Se você já possui a [_Arduino CLI_](https://arduino.github.io/arduino-cli/0.35/) intalada, verifique se esta está no PATH para poder executar a configuração corretamente. Caso você já tenha feito a instalação e a configuração necessária, passe para o [próximo passo](#4-conecte-o-microcontrolador-ao-seu-computador)

Clique [neste link](https://arduino.github.io/arduino-cli/0.35/installation/) para acessar a página de downloads da [_Arduino CLI_](https://arduino.github.io/arduino-cli/0.35/). Desça para a parte de Downloads e selecione o arquivo correspondente ao seu sistema operacional.

<div>
  <img src=assets/image-6.png>
</div>
<i>Parte de Downloads da Arduino CLI</i>

Ao clicar no arquivo correspondente, o download de um arquivo compactado será iniciado. Após o download, extraia este arquivo em um caminho que já esteja no PATH ou adicione o caminho onde este foi extraido ao PATH para que consiga fazer a utilização correta.

Para testar se a adição ao PATH foi sucedida, abra o prompt de comando e digite `arduino-cli`, se tiver sido sucedida, a seguinte saida será exibida:

<div>
  <img src=assets/image-7.png>
</div>
<i>Saída ao comando arduino-cli no terminal</i>

Caso não tenha sido sucedida, a seguinte saída será exibida:

```
'arduino-cli' não é reconhecido como um comando interno ou externo, um programa operável ou um arquivo em lotes.
```

Para resolver, adicione o caminho onde o arquivo compactado da [_Arduino CLI_](https://arduino.github.io/arduino-cli/0.35/) foi extraído ao PATH do seu sistema.

# 4. Conecte o microcontrolador ao seu computador

Utilize o cabo micro-USB que acompanha o Kit para fazer a conexão com o seu computador.
<div>
  <img style="display: block;-webkit-user-select: none;margin: auto;background-color: hsl(0, 0%, 90%);" src="https://84771188-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FGEgcCk4PkS5Pa6uBabld%2Fuploads%2Fgit-blob-c47c9b3fde5e9a23528f23e997f35a51c1e3be3e%2Fb302301-out.gif?alt=media">
</div>
<i>Pressione RESET duas vezes para iniciar o Bootloader do microcontrolador</i>


# 5. Atualizando o firmware do microcontrolador

Após o passo anterior, faça o download [Edge Impulse firmware](https://cdn.edgeimpulse.com/firmware/arduino-nano-33-ble-sense.zip) e faça a extração do arquivo após finalizado. Este passo é necessário pois o microcontrolador não vem com o firmware certo ainda.


Execute o flash referente ao seu sistema operacional acessando o caminho onde o arquivo fora extraido pelo prompt de comando. Após isso, execute o flash usando `./` e o nome referente ao sistema.

* Windows:
```
./flash_windows.bat
```
* Mac:
```
./flash_mac.command
 ```
* Linux:
```
./flash_linux.sh
```

Espere até que a execução do código seja finalizada e, por fim, pressione o botão RESET uma vez para executar o novo firmware.

# 6. Configurando o microcontrolador à sua conta

Após executarmos o flash, podemos utilizar do comando `edge-impulse-daemon` para conectarmos o [Arduino Nano 33 BLE Sense](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense) com a conta que criamos no [passo 1](#1-criando-uma-conta-no-edge-impulse) ou qualquer outra.

Após a execução do comando `edge-impulse-daemon` no prompt de comando, será pedido ao usuário o e-mail vinculado à conta do [_Edge Impulse_](https://edgeimpulse.com/) e, depois, a senha desta conta. 

Depois disso, a [_Edge Impulse CLI_](https://docs.edgeimpulse.com/docs/tools/edge-impulse-cli/cli-installation) irá procurar pelo microcontrolador, selecione a porta correspondente a ele (você pode verificar na aba de gerenciador de dispositivos).

Por fim, você será perguntado a qual projeto você quer conectar o dispositivo e, após isso, qual nome você quer dar a ele.

<div>
  <img src=assets/image-8.png>
</div>
<i>Saída ao comando edge-impulse-daemon, imagem retirada do site Edge Impulse.</i>

Caso tudo ocorra bem, a seguinte saída deve sair no seu terminal:

<div>
  <img src=assets/image-9.png>
</div>
<i>Execução bem sucedida, imagem retirada do site Edge Impulse.</i>

Você pode verificar o dispositivo na seção _devices_ do [_Edge Impulse_](https://edgeimpulse.com/) e, se seu dispositivo estiver conectado, aparecerá com um pequena bolinha verde como na imagem abaixo:

<div>
  <img src=assets/image-10.png>
</div>
<i> Dispositivo conectado, imagem retirada do site Edge Impulse.</i>

Com isso, você pode utilizar o [Arduino Nano 33 BLE Sense](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense) para fazer inúmeros projeos de TinyML!
