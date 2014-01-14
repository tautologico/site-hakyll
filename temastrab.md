---
title: Temas para trabalhos (Teoria/Linguagens Formais)
---

Temas para Trabalhos (Teoria/Linguagens Formais)
==============================================================

Algumas sugestões para trabalhos que podem ser apresentados 
para as disciplinas de Teoria da Computação e Linguagens Fomais 
e Autômatos.

Os trabalhos podem ser sobre qualquer coisa relacionada à teoria 
da computação ou linguagens formais. A sugestão é seguir um dos 
três tipos: 

1. Trabalho teórico
2. Trabalho de implementação
3. Trabalho de pesquisa sobre aplicação

O trabalho teórico visa elaborar e apresentar alguma parte 
da teoria da computação ou das linguagens formais que não 
faz parte do programa da disciplina. Isso pode ser um 
detalhamento sobre algum tópico que está no programa, ou 
algum tópico totalmente novo. 

Um trabalho de implementação tem como objetivo criar 
um programa de computador que implementa algo relacionado 
às disciplinas. Pode ser um simulador de algum tipo de 
autômato ou alguma aplicação que use as ideias 
apresentadas durante as aulas.

O trabalho sobre aplicação deve mostrar uma aplicação 
dos assuntos abordados nas disciplinas em outras áreas
do conhecimento, ou em tópicos de pesquisa atual. 

Seguem sugestões específicas para cada tipo de trabalho.


Trabalho teórico
----------------

- **Lambda-cálculo**: O &lambda;-cálculo é um sistema formal 
usado na teoria das linguagens de programação, na semântica 
de linguagens formais e naturais e em várias outras aplicações. 
O cálculo também pode ser usado como modelo geral de computação, 
com poder expressivo equivalente às Máquinas de Turing. Um trabalho 
sobre o &lambda;-cálculo pode enfatizar o cálculo como 
modelo de computação ou alguma das suas aplicações. 

- **Máquinas de Post**: Emil Post criou um outro modelo computacional
equivalente às Máquinas de Turing, conhecido como *Sistemas de Post* 
ou *Máquinas de Post*. Um trabalho sobre este assunto pode 
explicar o funcionamento do modelo e mostrar a equivalência dele 
com as Máquinas de Turing. 

- **Teoria das Funções Recursivas**: esta teoria é um outro 
modelo computacional geral, com poder expressivo equivalente às 
Máquinas de Turing. A teoria é bastante usada nos estudos mais 
avançados de computabilidade, e permite mais facilmente entender 
conceitos de computabilidade que são mais diretamente aplicáveis 
para programadores. Um trabalho sobre este assunto poderia 
apresentar a teoria, demonstrar alguns exemplos e mostrar 
a equivalência com as Máquinas de Turing. 

- **Cálculo e Análise Computáveis**: A análise computável é um 
ramo da teoria da computação que estuda as funções computáveis e 
suas propriedades, incluindo questões de computabilidade relativas
à diferenciação e integração. É uma visão computacional dos conceitos 
do cálculo diferencial e integral. Isso é importante em aplicações, por 
exemplo na inferência probabilística e programação probabilística, onde 
o resultado de um programa é uma função de probabilidade condicional.

- **O Problema SAT**: O problema de satisfatibilidade de fórmulas da 
lógica proposicional (SAT) foi o primeiro problema a ser provado 
como NP-Completo, e por isso até hoje é um dos exemplos mais conhecidos
desta classe de problemas. Como resultado dos estudos sobre redutibilidade 
para provar NP-completude de outros problemas, muitos problemas foram 
reduzidos ao SAT, e com isso muitas aplicações podem utilizar um 
"resolvedor" (ou *solver*) do problema SAT. Um trabalho teórico sobre 
o SAT poderia discutir propriedades mais profundas do problema, e algumas 
técnicas que são usadas para implementar *solvers* eficientes. 

Trabalho de implementação
-------------------------

- **Simulação de autômatos ou máquinas de Turing**: Criar um programa 
para simular algum tipo de autômato (Autômatos Finitos ou Autômatos de Pilha)
ou uma Máquina de Turing. O trabalho deve apresentar as ideias principais 
envolvidas na simulação, e alguns casos de exemplo. 

- **Analisador de Expressões Regulares**: Um programa que analise a 
estrutura de uma expressão regular, criando a árvore de operações 
básicas que formam a expressão (união, concatenação e fecho). O programa 
também poderia verificar se uma cadeia arbitrária pertence à linguagem 
gerada pela expressão regular, ou gerar cadeias pertencentes à 
linguagem da expressão. 

- **Implementar uma feature no rslex**: [rslex](http://github.com/tautologico/rslex)
pretende ser um gerador de analisadores léxicos para a linguagem de programação 
[rust](http://rust-lang.org). Um gerador de analisadores léxicos cria um 
programa que faz análise léxica (*tokenização*) da entrada a partir dos 
padrões especificados pelo usuário, na forma de expressões regulares. Este é 
o primeiro passo para fazer análise de linguagens ou formatos de dados, 
incluindo linguagens de programação (a análise léxica é a primeira etapa de 
todo compilador ou interpretador). O processo de geração envolve uma série de 
transformações que começa com a análise das expressões regulares e sua 
transformação para um Autômato Finito; este autômato passa por várias 
etapas de transformação até chegar a um autômato final que é traduzido 
para código. Este trabalho envolveria implementar uma parte deste 
processo, sob minha orientação. Para isso é necessário aprender a trabalhar 
com a linguagem [rust](http://rust-lang.org).


Trabalho sobre aplicação
------------------------

- **Compiladores**: uma das aplicações mais clássicas da teoria e técnicas 
das linguagens formais são os compiladores e interpretadores de linguagens 
de programação. Para analisar a linguagem entrada, um compilador possui 
como duas primeiras etapas a análise léxica (separar as "palavras" da entrada) 
e a análise sintática (descobrir a estrutura gramatical 
da entrada). A análise léxica é baseada 
nas linguagens regulares para descrever os padrões que formam as "palavras" (*tokens*)
da entrada, e usa expressões regulares e autômatos finitos na sua implementação. 
A análise sintática é baseada nas linguagens livres de contexto e usa as gramáticas 
livres de contexto como forma de descrição da estrutura gramatical das linguagens, 
e técnicas de reconhecimento que possuem similaridades ao funcionamento dos 
autômatos de pilha. Um trabalho sobre compiladores poderia falar de forma mais 
geral sobre essas duas fases, ou tratar apenas de uma dessas fases em maiores 
detalhes. O trabalho poderia falar sobre alguma das ferramentas existentes para 
facilitar na criação de analisadores léxicos e/ou sintáticos (geradores de analisadores 
léxicos como lex e flex; geradores de analisadores sintáticos como yacc, bison e antlr).

- **Processamento de Linguagem Natural**: o processamento de linguagens naturais 
envolve uma série de técnicas para fazer com que os computadores "entendam" 
as linguagens naturais humanas, seja por meio da fala ou do texto escrito. 
Muitas técnicas nessa área utilizam conceitos de linguagens formais, incluindo o 
uso de autômatos finitos para morfologia e o uso de gramáticas livres de contexto 
probabilística para fazer análise sintática do texto de entrada. Um trabalho 
neste tema poderia enfocar uma técnica específica ou apresentar um panorama 
geral do uso de linguagens formais na área de PLN. 

- **Métodos Formais e Verificação**: a área de métodos formais envolve o uso 
de modelos matemáticos para especificação, desenvolvimento e verificação de 
sistemas de hardware e software. Por exemplo, cada modelo de processador criado 
pela Intel ou AMD passa por um processo de verificação automática 
para evitar que exista algum erro na sua operação 
(como [o famoso bug de divisão do Pentium](https://pt.wikipedia.org/wiki/Pentium_FDIV_bug)). 
Métodos similares também são usados para verificação de software, principalmente 
para evitar falhas em sistemas críticos (como sistemas de controle em aviação
e usinas nucleares). Muitas técnicas nesta área usam conceitos relacionados a linguagens 
formais e teoria da computação. Por exemplo, algumas técnicas de 
[*model checking*](http://pt.wikipedia.org/wiki/Verifica%C3%A7%C3%A3o_de_modelos)
utilizam autômatos. 

- **Aplicações de resolvedores do SAT (ou SMT)**: Como discutido acima nos trabalhos 
teóricos, o problema SAT tem uma série de aplicações que envolvem problemas 
combinatórios. Os *solvers* do SAT são usados em vários contextos em diferentes 
sub-áreas da computação. Um trabalho sobre aplicações do SAT poderia 
selecionar algumas mais importantes ou entrar em maiores detalhes sobre 
uma aplicação específica. O problema SMT (Satisfiability Modulo Theories) é 
parecido com SAT mas está relacionado a lógicas mais expressivas, e *solvers*
para SMT também possuem um grande número de aplicações. Um trabalho poderia
tratar de SAT e SMT ou apenas de SMT. 

