# Intro: #
sigla de **CO**mmon **B**usiness **O**riented **L**anguage, Linguagem Comum Orientada para os Negócios é uma linguagem de programação orientada para o processamento de banco de dados comerciais.É a linguagem de programação inteira mais usada, produto do Departamento de Defesa norte-americano sob a direção da contra-almirante Grace Murray Hopper.
    
    Bibliografia:
    	https://pt.wikipedia.org/wiki/COBOL

# História: #
A decisão de criar uma fonte de Linguagem apropriada para dados comerciais foi tomada em Maio de 1959 numa reunião no Pentágono em Washington, DC. Participantes desta reunião eram representantes de usuários de computadores na indústria privada e governo, fábricas de computadores e outras partes interessadas.

O propósito era discutir a necessidade de uma Linguagem geral direcionada para serviços dentro de dados comerciais, e a possibilidade de criar desta maneira uma Linguagem. Como resultado uma comissão foi nomeada com o nome de CODASYL (Conference On Data System Languages).

A comissão começou a analisar as questões discutidas na reunião e uma subcomissão foi diretamente incumbida da tarefa de definir uma Linguagem adaptada para administrar processamento de dados.

Em 1.960 a gramática foi publicada, usualmente chamada Relatório COBOL-60. Esta Linguagem continha inúmeros erros e logo foi revisada em 1.961 e o Relatório COBOL-61 foi publicado. Ele forma a base para os mais comuns compiladores COBOL.

A continuação do trabalho da comissão estava mais concentrada em seguir todas as passos originados no Relatório COBOL-61. Isto levou a uma versão ampliada do COBOL, descrita em um Relatório provisório “COBOL-61 – Versão Estendida”, que foi publicada em 1.962. Formalmente, isto significava que um número de novos elementos foi adicionado ao Relatório anterior.

Um Relatório completamente novo foi publicado no fim do ano de 1.965, e foi definido como COBOL-65. Ele continha praticamente todos os elementos de “Versão Estendida”, porém numa forma totalmente revisada, junto com alguns elementos novos, projetado principalmente por causa do uso expressivo das memórias de acesso aleatório (RAM).

Embora o COBOL tenha sido desenvolvido e mantido pela CODASYL, ele foi também estabelecido como uma Linguagem Padrão pelo Instituto Americano de Padrões Nacionais (ANSI). Os fornecedores dos compiladores COBOL geralmente se baseavam no COBOL Padrão Nacional Americano. Um padrão inicial, noticiado em 1.968, foi revisado em 1.974 e novamente na metade dos anos 80.
    
    Bibliografia:
   		https://fagnersoliveira.wordpress.com/2012/10/08/curiosidade-cobol/

# COBOL NO MERCADO: #

COBOL é uma velha Linguagem de Programação, então o que a faz permanecer popular ?

* Amplamente usada – É bem correspondida por arquivos direcionados (parte essencial da Programação Comercial) como armazenamento e restauração de informações;
* Documentação – Suporta muito bem o idioma Inglês como Linguagem de Programação, portanto é auto – documentável e suas instruções são de fácil leitura e compreensão.
* Compatibilidade – A Linguagem é uma máquina independente. Um programa escrito em COBOL para um tipo de computador pode ser executado em qualquer outro tipo, somente com algumas modificações;
* Padronização – Existe uma versão do COBOL que foi aceita como padrão pelo Instituto Americano de Padrões Nacionais (ANSI);
* Com o crescimento de novas necessidades, o COBOL é constantemente revisado e atualizado;
* Ótimos programas já foram escritos em COBOL. A Linguagem ficou tão enraizada na maioria dos negócios, que se tornou permanente.

Após todas estas vantagens você pode perguntar porquê o COBOL não é abordado mais amplamente nas Escolas e Universidades. Bem existem algumas desvantagens:

* Por causa de sua auto – documentação, o COBOL é demorado. Você perde mais tempo codificando e digitando programas nesta Linguagem do que em outros tipos;
* Abrangência Limitada – COBOL não é uma Linguagem universal para todos os tipos de processamento.

        Bibliografia:
   			 https://fagnersoliveira.wordpress.com/2012/10/08/curiosidade-cobol/

# Estrutura do COBOL: #
Um programa COBOL é formado por 4 partes principais, que são chamadas de Divisions:

* IDENTIFICATION DIVISION – Explica a finalidade do programa, seu nome, autor, data e local onde foi escrito e compilado.
* ENVIRONMENT DIVISION – Fornece informações sobre o Ambiente, ou seja, o computador em que o programa será compilado e onde a Linguagem de máquina resultante será processada. Fornece também um nome em COBOL para todos os arquivos que serão processados designando um dispositivo de E / S para cada um.
* DATA DIVISION – Fornece uma breve descrição de cada arquivo e campos de dados utilizados pelo programa. Estes campos são armazenados em uma área da memória chamada Working Storage.
* PROCEDURE DIVISION – É onde se encontram as instruções que informam ao computador o processamento que deve ser realizado.

# S E C T I O N S: #

Cada Division de um programa COBOL é subdividida em Sections, que iniciam por linhas denominadas Cabeçalhos de Seção. Cada uma das Sections é por sua vez subdividida em Parágrafos.

    Bibliografia:
    https://fagnersoliveira.wordpress.com/2012/10/08/curiosidade-cobol/
 
# Classificação do COBOL: #

É uma linguagem que não possui vínculo ao processador utilizado e a semântica de termos é mais genérica podendo ser utilizada em outras plataformas;
Seu ciclo iniciou-se em 1960 com o COBOL e 1963 com a linguagem BASIC.
Criada para o desenvolvimento de aplicações comerciais: estoque, contabilidade, folha pagamento. Disponível em todas as plataformas existentes.  Atualmente possui versões orientadas a objeto e visuais. É considerada, portanto, uma linguagem estruturada.

    Bibliografia:
   		http://objota.com.br/poo/iniciando-em-programacao-tipos-de-linguagem.html

# COMPARAÇÃO: #
Bom, para explicar melhor a comparação que farei dessa linguagem com outras que estou familiarizado usarei um exemplo de código em cobol:


    
     *----------------------------------------------------------------*
       IDENTIFICATION DIVISION.
       PROGRAM-ID.notas.
      *----------------------------------------------------------------*
       ENVIRONMENT DIVISION.
       CONFIGURATION SECTION.
      *----------------------------------------------------------------*
       SPECIAL-NAMES.
       CRT STATUS CBL-KEY
       DECIMAL-POINT  IS COMMA.
      *----------------------------------------------------------------*
       DATA DIVISION.
       WORKING-STORAGE SECTION.
      *----------------------------------------------------------------*
       COPY "TCKEYS.CPY".
       01  VARIAVEIS-WORKING.
       05  W-BRANCOS   PIC X(55) VALUE SPACES.
       05  W-ALUNO PIC X(50) VALUE SPACES.
       05  W-NOTA1 PIC 9(03) VALUE ZEROS .
       05  W-NOTA2 PIC 9(03) VALUE ZEROS .
       05  W-NOTA3 PIC 9(03) VALUE ZEROS .
       05  W-NOTA4 PIC 9(03) VALUE ZEROS .
       05  W-TOTAL-NOTAS   PIC 9(03) VALUE ZEROS .
       05  W-MEDIA PIC 9(02) VALUE ZEROS .
      *----------------------------------------------------------------*
       PROCEDURE DIVISION.
       00000-PRINCIPAL SECTION.
       PERFORM 10000-INICIA
       PERFORM 20000-PROCESSA
       PERFORM 90000-FINALIZA
      
           STOP RUN
           .
       99999-FIM-PRINCIPAL.
           EXIT.
      *----------------------------------------------------------------*
       10000-INICIA SECTION.
           
           INITIALIZE VARIAVEIS-WORKING
           
           DISPLAY "Informe o Aluno.:" AT 0607
           DISPLAY "Nota 1o Bimestre:" AT 0907
           DISPLAY "Nota 2o Bimestre:" AT 1007
           DISPLAY "Nota 3o Bimestre:" AT 1107
           DISPLAY "Nota 4o Bimestre:" AT 1207
           DISPLAY "Total das Notas.:" AT 1607
           DISPLAY "Media das Notas.:" AT 1707
           DISPLAY "Menssagem.......:" AT 2007
           
           .
       19999-FIM-INICIA.
           EXIT.
      *----------------------------------------------------------------*
       20000-PROCESSA SECTION.
           DISPLAY "Informe o nome do aluno"
                                       AT 2025
           ACCEPT W-ALUNO              AT 0625
           DISPLAY W-BRANCOS           AT 2025
           IF KEY-ESC
              DISPLAY "Fim"            AT 2025
              STOP " "
              GO 89999-FIM-PROCESSA
           END-IF
           IF W-ALUNO = SPACES
              DISPLAY "Campo obrigatorio"
                                       AT 2025
              STOP " "
              DISPLAY W-BRANCOS        AT 2025
              GO 20000-PROCESSA
           END-IF
           .
       20100-ENTRA-NOTA-1.
           DISPLAY "Informe a primeira nota do aluno"
                                       AT 2025
           ACCEPT W-NOTA1              AT 0925
           DISPLAY W-BRANCOS           AT 2025
           IF KEY-ESC
              GO 20000-PROCESSA
           END-IF
           
           ADD W-NOTA1                 TO W-TOTAL-NOTAS
           DISPLAY W-TOTAL-NOTAS       AT 1625
           .
       20200-ENTRA-NOTA-2.
           DISPLAY "Informe a segunda nota do aluno"
                                       AT 2025
           ACCEPT W-NOTA2              AT 1025
           DISPLAY W-BRANCOS           AT 2025
           
           ADD W-NOTA2                 TO W-TOTAL-NOTAS
           DISPLAY W-TOTAL-NOTAS       AT 1625
           .
       20300-ENTRA-NOTA-3.
           DISPLAY "Informe a terceira nota do aluno"
                                       AT 2025
           ACCEPT W-NOTA3              AT 1125
           DISPLAY W-BRANCOS           AT 2025
           
           ADD W-NOTA3                 TO W-TOTAL-NOTAS
           DISPLAY W-TOTAL-NOTAS       AT 1625
           .
       20400-ENTRA-NOTA-4.
           DISPLAY "Informe a primeira nota do aluno"
                                       AT 2025
           ACCEPT W-NOTA4              AT 1225
           DISPLAY W-BRANCOS           AT 2025
           
           ADD W-NOTA4                 TO W-TOTAL-NOTAS
           DISPLAY W-TOTAL-NOTAS       AT 1625
           .
       20500-CALCULA-MEDIA.
           DIVIDE W-TOTAL-NOTAS        BY 4
                                   GIVING W-MEDIA
           DISPLAY W-MEDIA             AT 1725
           
           IF W-MEDIA < 50
              DISPLAY "REPROVADO!!!"   AT 2025
           ELSE
              IF W-MEDIA < 70
                 DISPLAY "RECUPERACAO!!!"
                                       AT 2025
              ELSE
                 DISPLAY "APROVADO!!!" AT 2025
              END-IF
           END-IF
           STOP " "
           .
       89999-FIM-PROCESSA.
           EXIT.
      *----------------------------------------------------------------*
       90000-FINALIZA SECTION.
       99999-FIM-FINALIZE.
           EXIT.
 


Agora vamos entender passo-a-passo...



      *----------------------------------------------------------------*
       IDENTIFICATION DIVISION.
       PROGRAM-ID.     boletim.
      *----------------------------------------------------------------*



**IDENTIFICATION DIVISION**, é uma divisão do cobol obrigatória.





      *----------------------------------------------------------------*
       ENVIRONMENT DIVISION.
       CONFIGURATION SECTION.

      *----------------------------------------------------------------*
       SPECIAL-NAMES.
           CRT STATUS     CBL-KEY
           DECIMAL-POINT  IS COMMA.
      *----------------------------------------------------------------*




**ENVIRONMENT DIVISION**, é uma divisão do cobol obrigatória.

**CONFIGURATION SECTION** é a seção de configuração. Definimos que a tecla que ira controlar as ações(pra cima, pra baixo, esc, etc) é CBL-KEY e definimos que o ponto decimal é virgula (COMMA).





      *----------------------------------------------------------------*
       DATA DIVISION.
       WORKING-STORAGE SECTION.
      *----------------------------------------------------------------*
       COPY "TCKEYS.CPY".
       01  VARIAVEIS-WORKING.
           05  W-BRANCOS               PIC X(55) VALUE SPACES.
           05  W-ALUNO                 PIC X(50) VALUE SPACES.
           05  W-NOTA1                 PIC 9(03) VALUE ZEROS .
           05  W-NOTA2                 PIC 9(03) VALUE ZEROS .
           05  W-NOTA3                 PIC 9(03) VALUE ZEROS .
           05  W-NOTA4                 PIC 9(03) VALUE ZEROS .
           05  W-TOTAL-NOTAS           PIC 9(03) VALUE ZEROS .
           05  W-MEDIA                 PIC 9(02) VALUE ZEROS .
      *----------------------------------------------------------------*




DATA DIVISION, é uma divisão do cobol obrigatória.
WORKING-STORAGE SECTION é a seção onde declaramos nossas variáveis. Uma variável é onde se armazena alguma informação do seu programa, como por exemplo alguma informação digitada ou um cálculo.
COPY "TCKEYS.CPY" é uma copia do arquivo TCKEYS.CPY, para não ter que digitar tudo que está neste arquivo, utilizamos o comando COPY. Este arquivo se encontra na pasta C:\tinycobol\copys.
Uma variável, por exemplo W-BRANCOS é uma variável alfanumérica "X" e tem o tamanho de 55 posições (55) e é uma variável com o valor inicial vazia (VALUE SPACES).
Uma variável, por exemplo W-NOTA1 é uma variável numérica "9" e tem o tamanho de 03 posições (03) e é uma variável com valor inicial zerada (VALUE ZEROS).



      *----------------------------------------------------------------*
       PROCEDURE DIVISION.
       00000-PRINCIPAL SECTION.
           PERFORM 10000-INICIA
           PERFORM 20000-PROCESSA
           PERFORM 90000-FINALIZA
          
           STOP RUN
           .
       99999-FIM-PRINCIPAL.
           EXIT.
      *----------------------------------------------------------------*




DATA DIVISION, é uma divisão do cobol obrigatória.

00000-PRINCIPAL SECTION é a seção onde se inicia o programa, poderia se qualquer nome. 
PERFORM é um comando do cobol, onde sua função é EXECUTAR, no nossa caso ele irá executar a seção 10000-INICIA, que vai do 10000-INICIA SECTION até o EXIT que está no paragrafo 19999-FIM-INICIA, que também poderia ter outro nome.
STOP RUN é o comando onde finaliza o programa.







      *----------------------------------------------------------------*
       10000-INICIA SECTION.
           
           INITIALIZE VARIAVEIS-WORKING
           
           DISPLAY "Informe o Aluno.:" AT 0607
           DISPLAY "Nota 1o Bimestre:" AT 0907
           DISPLAY "Nota 2o Bimestre:" AT 1007
           DISPLAY "Nota 3o Bimestre:" AT 1107
           DISPLAY "Nota 4o Bimestre:" AT 1207
           DISPLAY "Total das Notas.:" AT 1607
           DISPLAY "Media das Notas.:" AT 1707
           DISPLAY "Menssagem.......:" AT 2007
           
           .
       19999-FIM-INICIA.
           EXIT.
      *----------------------------------------------------------------*



10000-INICIA SECTION é a seção onde se inicia o programa, pode ter qualquer nome.
INITIALIZE VARIAVEIS-WORKING significa que vamos inicializar (mover zeros para as variáveis numéricas e espaço para as variáveis alfanuméricas). A variável VARIAVEIS-WORKING se refere à um grupo de variáveis declaradas na WORKING-STORAGE SECTION. Então tudo que eu fizer com está veriável será refletida nas demais.
DISPLAY é o comando responsável por mostrar alguma informação, por exemplo DISPLAY "Informe o Aluno.:". Iremos mostrar o aluno na posição 0607. Linha 06 coluna 07 da tela do DOS, que é onde executamos nosso programa.
Obs* O ponto (.) antes do final de cada paragrafo é obrigatório.





      *----------------------------------------------------------------*
       20000-PROCESSA SECTION.
           DISPLAY "Informe o nome do aluno"
                                       AT 2025
           ACCEPT W-ALUNO              AT 0625
           DISPLAY W-BRANCOS           AT 2025
           IF KEY-ESC
              DISPLAY "Fim"            AT 2025
              STOP " "
              GO 89999-FIM-PROCESSA
           END-IF
           IF W-ALUNO = SPACES
              DISPLAY "Campo obrigatorio"
                                       AT 2025
              STOP " "
              DISPLAY W-BRANCOS        AT 2025
              GO 20000-PROCESSA
           END-IF
           .



ACCEPT é o comando onde o usuário irá digitar algo no programa e você armazenará em alguma variável, no nosso caso W-ALUNO, ou seja, tudo que ele digitar nesse momento irá ficar armazenado nesta variável.
IF KEY-ESC esté comando teste se o usuário apertou a tecla ESC, para ver as teclas válidas acesso o COPY das TECLAS. Se o usuário tiver apertado ESC irá mostrar uma mensagem na tela e o comando STOP " ", significa que o usuário deve apertar alguma tecla, após isso irá finalizar o processo enviando para o final da seção (GO 89999-FIM-PROCESSA). Nunca devemos esquecer do END-IF, ele é obrigatório quando você fez um IF.





       20200-ENTRA-NOTA-2.
           DISPLAY "Informe a segunda nota do aluno"
                                       AT 2025
           ACCEPT W-NOTA2              AT 1025
           DISPLAY W-BRANCOS           AT 2025
           
           ADD W-NOTA2                 TO W-TOTAL-NOTAS
           DISPLAY W-TOTAL-NOTAS       AT 1625
           .



Neste paragrafo temos de diferente o comando ADD, que funciona da seguinte forma. Irá adicionar o valor que está na variável W-NOTA2 na variável W-TOTAL-NOTAS, ou seja, a veriável W-TOTAL-NOTAS será uma acumuladora de valores.





       20500-CALCULA-MEDIA.
           DIVIDE W-TOTAL-NOTAS        BY 4
                                   GIVING W-MEDIA
           DISPLAY W-MEDIA             AT 1725
           
           IF W-MEDIA < 50
              DISPLAY "REPROVADO!!!"   AT 2025
           ELSE
              IF W-MEDIA < 70
                 DISPLAY "RECUPERACAO!!!"
                                       AT 2025
              ELSE
                 DISPLAY "APROVADO!!!" AT 2025
              END-IF
           END-IF
           STOP " "
           .



Neste outro paragrafo temos outra informação nova, é o comando DIVIDE, que é o comando da divisão, ou seja, irá dividir o valor da variável W-TOTAL-NOTAS por 4 e armazenar (GIVING) na variável W-MEDIA, após isto é mostrado a média do aluno.
O comando ELSE significa SENÃO, ou seja, se a média for menor que 50 o aluno é reprovado, senão verificamos se é menor que 70, senão é aprovado.


A seção 90000-FINALIZA não utilizamos para nada neste programa, mas não tem problema em deixá-la ali.



Notas importantes....


DISPLAY - Mostra algo em algum lugar...
ACCEPT - Recebe algo em algum lugar...
IF - Testa algo, faz algo e END-IF...
GO - Vai para algum lugar...O comando GO deve mandar sempre para algum paragrafo, nunca para uma linha especifica no código.

Bom, tudo bem que não é o foco da linguagem um programa como esse, mas nas comparações read, write e expressividade
como visto em aula, essa linguagem estaria com péssima avaliação em todos.
    

	Bibliografia
    http://tudocobol.blogspot.com.br/

# Curiosidades #
* Em 1999, o grupo Gartner fez uma pesquisa e concluiu que 80% das aplicações corporativas em execução no mundo naquele momento eram escritas em Cobol. Os outros 20% eram compartilhados pelas demais linguagens. Este dado tem 9 anos hoje, no entanto, a realidade não deve ser tão diferente nos dias atuais. Basta levar em consideração que BOA parte deste código estava presente em aplicações de missão crítica que, com alta probabilidade, ainda estão em execução hoje. Aliás, um estudo mais recente do mesmo instituto, comprovou que atualmente (artigo de 2006), há aproximadamente **180 bilhões** de linhas de código escritas em Cobol em execução atualmente.

* Cobol é orientado a objetos. O padrão Cobol 2002 aceita orientação a objetos. E tanto Fujitsu quanto Microfocus oferecem compiladores que suportam o paradigma. Mais interessante ainda: se você programa na plataforma .net, pode experimentar Cobol se quiser. Aliás, logo aparecerá um compilador para Java também. É apenas questão de tempo.

* Em 2002, uma pesquisa do grupo Gartner comprovou a existência de **dois milhões** de programadores Cobol no mundo.
 
* Cobol paga bem. Dada a necessidade por profissionais que saibam trabalhar com Cobol, e a escassez de mão-de-obra, temos como resultado um aumento significativo dos salários destes programadores. Os salários podem chegar a até R$ 12.000. No exterior, a situação é ainda melhor.

* Programas feitos em Cobol costumam ficar em execução por décadas, ou seja, estes sistemas estão em execução não porque simplesmente “já existem”, mas sim porque são extremamente fáceis de se manter. Boa parte do problema do agora risível “bug do milênio” se deveu ao fato de que os desenvolvedores iniciais daquelas aplicações (a maior parte, escrita em… adivinha!) não imaginava que elas fossem durar tanto tempo.
Dado que o ponto forte de venda de plataformas como Java e .net é justamente a facilidade de manutenção destes sistemas, soa quase “conspiracionista” pensar no porquê deste fato ser tão pouco mencionado.

**Bibliografia:
http://www.itexto.net/devkico/?p=135**