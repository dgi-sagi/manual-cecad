TABCAD: como gerar tabelas simples e cruzadas
=============================================

O menu TABCAD pode ser acessado sem necessidade de login e senha. Ele permite gerar frequências simples, e tabelas cruzadas e a aplicação de filtros. Os dados dessa funcionalidade não são identificados, por isso, são abertos à consulta de todos.
Gerando uma tabela de frequência simples.

A diferença entre uma **tabela de frequência simples** e uma **tabela cruzada** consiste no número de variáveis selecionadas. Para uma tabela de frequência simples, selecione apenas uma variável para a coluna (opção :guilabel:`Variável Coluna`) e clique no botão :guilabel:`Valor Absoluto`.

Primeiramente, é necessário selecionar se os dados precisam ou não da marcação de beneficiários do Programa Bolsa Família, conforme explicado na seção :ref:`doc_temporalidade`.

Em seguida, deve-se selecionar a abrangência geográfica de interesse. Na versão de acesso público do CECAD, no campo “Selecione um estado”, é possível selecionar a Unidade da Federação (Estado ou Distrito Federal), as Regiões ou Brasil. Ao selecionar uma Unidade da Federação, aparecerá o campo :guilabel:`Selecione um município`, onde é possível selecionar um município específico daquele estado. Para escolher um estado, por exemplo, basta deixar o campo para a escolha do município em branco, como na figura abaixo:


.. figure:: /img/tabcad/estado.jpg

   Figura 1: selecionando um estado no TabCad

No exemplo a seguir temos o resultado para a variável ``Bloco 2 – Forma de escoamento sanitário``, detalhando que **quase 13 milhões** declaram possuir *Rede coletora de esgoto ou pluvial* enquanto **mais de 8 milhões** declaram possuir *Fossa rudimentar*, *Vala a céu aberto* ou *Direto para um rio, lago ou mar*.

.. figure:: /img/tabcad/tabulador.jpg

   Figura 2: exemplo de consulta

Ao clicar no botão :guilabel:`% Total` é possível ver os valores em porcentagem (%). O exemplo abaixo mostra que **46%** das famílias do Cadastro Único declaram ter **Rede Coletora de esgoto ou pluvial**, e outros **44%** declaram ter **fossa séptica**, **rudimentar**, **vala a céu aberto**, **escoamento direto em um rio, lago, mar** ou **outra forma**, enquanto **10%** não responderam.

.. figure:: /img/tabcad/familia2.jpg

   Figura 3: resultado da consulta de exemplo (valores percentuais)


Gerando uma tabela cruzada
--------------------------

Para criar uma tabela cruzada, selecione uma variável para a coluna (opção :guilabel:`Variável Coluna`), outra variável para a linha (opção :guilabel:`Variável Linha`) e clique no botão :guilabel:`Valor Absoluto`.

No exemplo abaixo, temos o resultado para as variáveis ``Bloco 2 – Forma de escoamento sanitário`` e ``Bloco 4 – Recebe Bolsa Família``. A partir deste cruzamento, temos **quase 8 milhões** que **não recebem PBF** e declaram possuir **Rede coletora de esgoto ou pluvial** enquanto **cerca de 5,6 milhões** que **Recebem PBF** e declaram possuir **Rede coletora de esgoto ou pluvial**.

.. figure:: /img/tabcad/cruzada.jpg

   Figura 4: resultado de consulta de uma tabela cruzada

Ao clicar no botão :guilabel:`% Total` temos os valores representados em percentuais. Veja o resultado abaixo, em que **27%** das famílias do Cadastro Único **não recebem PBF** e possuem **Rede coletora de esgoto ou pluvial** e **19%** **recebem PBF** e declaram possuir **Rede coletora de esgoto ou pluvial**.

.. figure:: /img/tabcad/percentual.jpg

   Figura 5: resultado de consulta de uma tabela cruzada (valores percentuais)

Ao clicar no botão :guilabel:`% Linha` é possível fazer a análise percentual por linha. Veja no exemplo abaixo que, das famílias que **não Recebem PBF**, **54%** possuem **Rede coletora de esgoto ou pluvial**, ao passo que das famílias que **Recebem PBF** apenas **39%** possuem **Rede coletora de esgoto ou pluvial**. Se analisarmos a resposta **Fossa rudimentar** é possível notar uma diferença de **6 pontos percentuais** a mais para quem **recebe PBF**. Isso mostra que as famílias do Bolsa Família estão em situação mais crítica de vulnerabilidade a respeito do tema saneamento básico.

.. figure:: /img/tabcad/linha.jpg

   Figura 6: resultado de consulta de uma tabela cruzada (valores percentuais por linha)

Ao clicar no botão :guilabel:`% Coluna`, é possível fazer a análise percentual por coluna. Veja no exemplo abaixo coluna a coluna. Nota-se que apenas a resposta **Rede coletora de esgoto ou pluvial** possui proporção maior de famílias que **não recebem PBF**. A resposta **Fossa séptica** possui proporção igual para **PBF** e **não PBF**, e as demais respostas todas possuem maior proporção de famílias do Bolsa Família. Essa proporção é muito maior inclusive na opção **Sem Resposta**, pois devido à vulnerabilidade crítica dessas famílias muitas nem respondem.

.. figure:: /img/tabcad/coluna.jpg

   Figura 7: resultado de consulta de uma tabela cruzada (valores percentuais por coluna)


Extrair listagem referente ao resultado do tabulador
----------------------------------------------------

Os usuários autorizados a acessar dados identificados do Cadastro Único, conforme explicado na seção :ref:`doc_quem_pode_ter_acesso` e que fizeram login no CECAD possuem a opção de extrair listagem de famílias e pessoas cadastradas de acordo com o resultado da busca realizada. Após acessar os resultados de uma tabela simples ou cruzada, para acessar as listagens, basta clicar sobre o ícone *“presentinho”* e baixar o arquivo. Para acessar tais informações sigilosas, é necessário aceitar o “TERMO DE COMPROMISSO DE MANUTENÇÃO DE SIGILO”.

Assim, por exemplo, se o município quiser fazer uma ação específica para famílias indígenas que não são beneficiárias do Programa Bolsa Família, basta selecionar as variáveis e aplicar os filtros necessários. A partir do resultado, ao clicar no ícone *“presentinho”* da linha e coluna correspondente às famílias indígenas e não beneficiárias do PBF é possível gerar a lista com o nome, endereço e outras informações dessas famílias.

.. figure:: /img/tabcad/listagem.jpg

   Figura 8: botão de extração de dados




