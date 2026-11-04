# FM Acessível

Acessibilidade para **Football Manager 26** (e, em breve, Football Manager 27) para pessoas cegas
ou com baixa visão.

O FM Acessível é um programa que roda ao lado do jogo. Ele mostra a tela atual do Football Manager
como uma lista que você percorre com as setas, fala cada item com o NVDA, o JAWS ou com uma voz
própria, e **narra as partidas** com uma voz de locutor.

> **Versão de testes (0.1.0).** Esta é a primeira versão pública. Algumas telas podem aparecer
> incompletas ou com nomes estranhos. Relatos de problemas são muito bem-vindos na aba Issues.

## Download

[Baixar o FM Acessível (FMAcessivel.exe)](https://github.com/LeoAlves11/football-manager-accessibility/releases/latest/download/FMAcessivel.exe)

É um único arquivo, que já traz tudo o que precisa instalar. Não é preciso extrair nada: basta
baixar e abrir. Este link sempre baixa a versão mais recente.

Se preferir, a página de [Releases](https://github.com/LeoAlves11/football-manager-accessibility/releases/latest)
também tem o **FMAcessivel.zip**, com o mesmo programa, o manual em texto (LEIA-ME.txt) e as licenças.

## O que você precisa

- Windows 10 ou 11 (64 bits).
- Football Manager 26 instalado pela Steam.
- Opcional: NVDA ou JAWS. Sem leitor de tela, o próprio FM Acessível fala usando as vozes do
  Windows. Para uma voz em português, instale a voz "Português (Brasil)" em Configurações do
  Windows, Hora e idioma, Fala.

Não é preciso instalar .NET nem mais nada: tudo vem dentro do FMAcessivel.exe.

## Instalação

1. Feche o Football Manager.
2. Abra o **FMAcessivel.exe**. Se o Windows mostrar o aviso "O Windows protegeu o computador",
   escolha "Mais informações" e depois "Executar assim mesmo". O aviso aparece porque o programa
   ainda não tem assinatura digital.
3. O programa diz quais jogos encontrou. Pressione **Alt+J** para abrir o menu Jogo, escolha
   o seu Football Manager e depois **Instalar o mod**.
4. Ainda no menu Jogo, escolha **Abrir o jogo**.

**Importante:** a primeira vez que o jogo abre depois de instalar demora alguns minutos e fica
em silêncio. Isso é normal. Espere o FM Acessível dizer **"Conectado ao FM26"**. Das próximas
vezes, o jogo abre no tempo normal.

## Como usar

Use a janela do FM Acessível, não a janela do jogo. O jogo continua rodando ao fundo e reage a
tudo o que você faz na lista.

A janela tem duas listas:

- **Tela do jogo:** tudo o que está na tela agora. Painéis aparecem como `== Nome do painel ==`,
  seguidos dos textos e controles daquele painel. Diálogos e janelas por cima aparecem primeiro.
- **Histórico de falas:** tudo o que foi falado, para reler com calma. Alterne entre as listas
  com **F6**.

Quando uma tela nova abre, o FM Acessível fala o título. A lista é atualizada sozinha.

### Teclas na lista "Tela do jogo"

- **Setas para cima e para baixo:** navegar pelos itens.
- **Enter:** ativar o item (clicar no botão, marcar a caixa, escolher a opção). Em campos de
  texto, abre uma caixa para você digitar.
- **Setas para a esquerda e para a direita:** trocar a opção de listas suspensas sem abri-las.
- **Page Down e Page Up:** pular para o próximo painel ou para o anterior.
- **Ctrl + seta para baixo e Ctrl + seta para cima:** pular direto para o próximo controle
  (botão, caixa, lista), ignorando os textos.
- **Letras:** pular para o próximo item que começa com aquela letra.
- **Backspace:** voltar para a tela anterior.
- **F3 ou Ctrl+Enter:** Continuar (avançar o jogo).
- **F2:** falar o título da tela atual.
- **F5:** atualizar a lista.
- **Ctrl+P:** placar da partida.
- **Ctrl+R:** repetir a última narração.
- **Esc:** silenciar.
- **F1:** ouvir a ajuda.

### Teclas que funcionam em qualquer lugar

Estes atalhos funcionam mesmo com a janela do jogo em primeiro plano:

- **Ctrl+Alt+F:** trazer a janela do FM Acessível para a frente.
- **Ctrl+Alt+C:** Continuar.
- **Ctrl+Alt+V:** voltar.
- **Ctrl+Alt+P:** placar.
- **Ctrl+Alt+T:** título da tela.
- **Ctrl+Alt+R:** repetir a última narração.
- **Ctrl+Alt+N:** ligar ou desligar o narrador.
- **Ctrl+Alt+S:** silenciar.

## Narrador de partidas

Durante as partidas, o narrador lê cada lance da barra de comentários do jogo. Ele também anuncia
os gols com um som curto e o placar, avisa quando um gol é anulado e fala o início e o fim de
cada tempo.

Por padrão, o narrador usa uma voz separada da voz dos menus, para soar como um locutor de rádio,
mesmo que você use NVDA ou JAWS.

## Configurações

Abra o menu **Voz** com **Alt+V** e escolha **Configurações de voz e narrador**. Lá você escolhe:

- **Saída da interface:** automático (usa o NVDA ou o JAWS se estiverem abertos, senão a voz
  própria), sempre NVDA, sempre JAWS ou sempre a voz própria.
- **Motor de voz própria:** vozes modernas do Windows (recomendado) ou vozes SAPI 5.
- **Voz e velocidade** da interface e do narrador.
- **Ler a lista com voz própria:** útil se você não usa leitor de tela.
- Narrador ligado ou desligado, narrador com voz própria, som nos gols e leitura das
  notificações do jogo.

O botão **Testar narrador** toca um exemplo de narração de gol.

## Problemas comuns

- **O programa não diz "Conectado":** na primeira vez, espere alguns minutos. Se continuar sem
  conectar, feche o jogo, use o menu Jogo, "Atualizar o mod", e abra o jogo de novo.
- **O jogo não foi encontrado:** use o menu Jogo, "Escolher pasta do jogo manualmente", e
  selecione a pasta onde fica o arquivo `fm.exe`.
- **Um atalho Ctrl+Alt não funciona:** outro programa já usa aquela combinação. O FM Acessível
  avisa no Histórico de falas quais atalhos não puderam ser registrados.
- **Uma tela aparece incompleta ou com nomes estranhos:** atualize com F5. Se continuar, abra um
  relato na aba Issues dizendo em qual tela aconteceu.

## Desinstalar

No menu Jogo, escolha o seu Football Manager e depois **Remover o mod**. Para remover também o
BepInEx (o carregador de mods), apague da pasta do jogo: `winhttp.dll`, `doorstop_config.ini`,
`.doorstop_version` e as pastas `BepInEx` e `dotnet`. Por fim, apague o `FMAcessivel.exe` e a
pasta `%LocalAppData%\FMAcessivel` (configurações e arquivos temporários do programa).

## Licenças e créditos

- FM Acessível: GPL-3.0 (arquivo LICENSE).
- Inclui o [BepInEx](https://github.com/BepInEx/BepInEx) (LGPL-2.1) e o cliente do
  [NVDA](https://www.nvaccess.org/) (LGPL-2.1).
- Inspirado no projeto
  [FM26 Access](https://github.com/DnDeezNuts/Football-Manager-2026-Access).
- Nenhum arquivo do Football Manager é incluído ou distribuído. Football Manager é marca da
  Sports Interactive e da SEGA; este projeto não tem ligação com elas.
