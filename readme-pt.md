 
Olá! Esse é meu github! 
 
Sou um Engenheiro de Software formado em Engenharia Elétrica pela UFMG. 
 
Alguns dos meus interesses são: software como ferramenta para a área de P&D, semicondutores, biotecnologia e a área de inovação e empreendedorismo. 
 
Você pode me encontrar [no LinkedIn](http://linkedin.com/in/blancblanc/) 
 
Este github contém (entre outras coisas): 
 
## Visualizador de terremotos 

[Live Demo](https://code-with-blanc.github.io/quake-viewer/)
[Repositório](https://github.com/code-with-blanc/quake-viewer)

Este é um visualizador de terremotos com React + Redux para o frontend e three.js para renderização 3D. Atualmente é apenas um projeto de hobby que atualizo de vez em quando, mas com sorte se torna uma ferramenta útil para divulgação científica.     :) 
 
![Captura de tela do visualizador de terremotos](./assets/quake-viewer.jpeg) 
 
## Pyblocks-sim - Simulador por diagrama de blocos em Python 
 

[Repository](https://github.com/OptMA-VLC/pyblocks)
[User Documentation](https://github.com/OptMA-VLC/pyblocks/tree/main/docs/tutorials) 
[INSCIT conference paper](https://ieeexplore.ieee.org/document/10693408)
 
Simulador usando diagrama de blocos em Python voltado à área de Comunicação em Luz Visível (VLC). 
Trabalho de conclusão do curso de graduação em Engenharia Elétrica na UFMG.

Features: 
    - Um arquivo de entrada no formato JSON descreve um diagrama de blocos - quais blocos serão usados e suas conexões 
    - Blocos são implementados como scripts em Python e são descobertos em tempo de execução 
    - Suporte nativo a séries temporais, com habilidade de extrair dados como gráficos ou arquivos csv de acordo com instruções fornecidas no arquivo de entrada 
    - Bloco de integração com LTSpice para a simulação de circuitos 
    - Arquivo de entrada pode especificar parâmetros que são fornecidos aos blocos 
    - Suporte a simulações do tipo varredura de parâmetros 
 
Durante a execução do programa, um diretório é escaneado para encontrar os blocos especificados no arquivo de entrada. O diagrama de blocos é modelado como um grafo, que é analisado para obter uma ordem de execução de acordo com as dependências de entradas e saídas de sinais. Os blocos são então executados sequencialmente. Uma interface CLI apresenta em tempo real o progresso da simulação e em caso de erro indica qual exceção ocorreu na execução de qual bloco. 
 
A camada CLI é completamente separada do motor de execução, respeitando o princípio que camadas de lógica de negócio não devem depender de camadas de E/S. As ferramentas de introspecção de código nativas do Python são usadas para descobrir arquivos que contém implementações válidas de blocos. O fato de ser uma linguagem interpretada é usado para carregar e executar o código implementado pelo usuário em tempo de execução. 

## Transpilação de Javascript dentro do navegador 
 
[Repositório]()https://github.com/code-with-blanc/p5x-playground 
 
Esse projeto foi idealizado como um editor de código online voltado para arte digital e se tornou uma exploração de como transpilar Js dentro do navegador. 
 
Features: 
    - Editor do VsCode 
    - Preview ao vivo da saída com layout picture-in-picture 
    - Capacidade de combinar vários arquivos em um só programa 
    - Transpilação usando rollup.js para permitir que o usuário escreva código em versões do Javascript / ECMAScript mais novas do que aquelas suportadas pelo navegador 
 
Como as ferramentas de build (ex: webpack, rollup.js) rodam tipicamente em um ambiente node.js com acesso ao sistema de arquivos do SO, foi um desafio interessante criar uma representação virtual dos arquivos sendo editados e configurar o rollup para funcionar sem um sistema de arquivo real. 
