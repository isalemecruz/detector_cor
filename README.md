<h1  align="center"> Detector de cor usando escala HSV</h1>
<h4 align="center">Isabela Leme Cruz</h4>
<h4 align="center">Turma 26 - 1°Semestre</h4>
<h4 align="center">Ilum Escola de Ciência (CNPEM)</h4>
<p style="text-align: justify;">Esse projeto corresponde ao trabalho final da disciplina Prática em Ciências de Dados, ministrada pelos professores doutores: Daniel Roberto Cassar, James Moraes de Almeida e Leandro Nascimento Lemos no 1° semestre de 2026.</p>
<h2>Descrição do projeto</h2>
<p style="text-align: justify;">O projeto consiste na realização de um sistema de detecção e identificação de cores em tempo real, utilizando visão computacional e a linguagem Python.<br>
Por meio da câmera do dispositivo do usuário, o sistema captura imagens continuamente e processar esses frames em tempo real. A partir das imagens capturadas, o projeto analisa uma área centralisada, na qual os valores das cores são convertidos para o modelo HSV (Hue, Saturation, Value), o que possibilita uma identificação mais precisa das cores, mesmo em diferentes iluminações.<br>
O código em Python faz a média dos valores capturados na região delimitada e mostra para o usuario a cor predominante, identificando as seguintes tonalinades: vermelho, laranja, amarelo, verde, ciano, azul, roxo e rosa e as variações: branco, preto e cinza. <br>
Para melhor visualização da cor detectada foi implementado um delay (mecanismo de atraso), evitando oscilações rápidas nas mudanças de cores.</p>
<h2>Notebooks e arquivos do projeto</h2>
<p style="text-align: justify;">README.md: Descrição do projeto.<br>
detectordecor.ipynb: Esse arquivo contém o programa que detecta e analias as cores e uma explicação detalhada de cada célula de código.</p>
<h2>Funcionamento</h2>
<h4><strong>Captura de video em tempo real</strong><h4>
  <p style="text-align: justify;">O sistema utiliza a câmera do dispositivo para capturar frames continuamente, permitindo analise posterior deles.</p>
<h4><strong>Processamento de imagem</strong></h4>
    <p style="text-align: justify;">Cada frame capturado é tratado utilizando a biblioteca OpenC, possibilitando a estração de informações relevantes.<br>
<strong>Conversão de cores para HSV</strong><br>
      <p style="text-align: justify;">As imagens convertidas do modelo RGB para o espaço HSV, garantindo maior precisão na identificação das cores.<br><p>
<h4><strong>Análise da região central da imagem e média das cores identificadas</strong></h4>
  <p style="text-align: justify;">O sistema identifica automaticamente uma área especifica no centro da tela para realizar a leitura das cores, faz uma média dos valores (matiz, saturação e brilho) identificados nela e mostra a cor predominante para o usuario.<br><p>
<h4><strong> Classificação automatica das cores, estabilidade de leitura e exibição para o usuario</strong></h4>
    <p style="text-align: justify;">O sistema identifica as cores vermelho, laranja, amarelo, verde, azul, roxo, rosa, além de tons neutros como branco, preto e cinza, implementa um delay para evitar oscilações rápidas e inlegiveis das cores e mostra na tela o nome da cor identifica, os valores HSV calculados, a área de análise destacada e o p onto central de leitura.
</p>
<h2>Bibliotecas utilizadas e versão do pyton</h2>
<h3>OpenCV</h3>
<p style="text-align: justify;">Usada para capturar imagens da camera, processar os frames em tempo real e exibição de informações na tela.</p>
<h3>Numpy</h3>
<p style="text-align: justify;">Usada para manipulação de arrays e calculo rápido dda média dos valores HSv da região analisada.</p>
<h3>Time</h3>
<p  style="text-align: justify;">Usada para controlar o tempo entre as atualizações e permitir que haja um delay entre elas, evitando mudanças muito rápidas.</p>
<h3>Versão do python usada</h3>
Python 3.13.7
<h2>Pré-requisitos e como rodar o projeto</h2>
  <p style="text-align: justify;"> Para executar o notebook, instale as bibliotecas necessárias rodando a célula abaixo no própio notebook:
    
  ```!pip install opencv-python numpy```
  
   e após isso clone o projeto usando o seguinte comando:
    
```
git clone https://github.com/07Soso/Logica_proposicional.git
```
  </p>
  
