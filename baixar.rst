Baixar
======

Esta funcionalidade é exclusiva para usuários autorizados a acessar dados identificados do Cadastro Único, conforme explicado na seção :ref:`doc_quem_pode_ter_acesso`. Na aba “Baixar”, há um menu com quatro opções:

- ATUAL
- ANOS ANTERIORES
- CONSULTA MÚLTIPLOS CPFs
- HISTÓRICO DE DOWNLOADS

A base é baixada em arquivo compactado no formato “zip”, contendo os seguintes arquivos:

tudo.csv
    contém a base de dados de famílias e/ou pessoas cadastradas.
dicionário.csv
    contém o dicionário com o código e a descrição de cada variável (coluna) da base.
LEIAME.txt
    contém informações sobre a referência da base baixada, bem como sobre os filtros aplicados na consulta, como cidade, estado etc.
script_postgres_tudo.sql
    contém um script para a criação de uma tabela no banco de dados PostgreSql com os campos do arquivo csv baixado.

As bases são disponibilizadas em formato CSV (valores separados por vírgulas). Para trabalhar com as bases geradas pelo CECAD é fundamental ter conhecimento de Excel ou de software estatístico ou de banco de dados para seu manuseio. Também é imprescindível conhecer bem as regras, conceitos e formulários do Cadastro Único para a correta interpretação dos dados cadastrais.

.. Attention:: Se o município ou estado possuir mais de 1 milhão de famílias ou pessoas cadastradas, não é possível abrir ou trabalhar com a base utilizando o Excel, porque ele possui um limite de 1.048.576 linhas por planilha. Nesse caso, é necessário utilizar software estatístico ou de banco de dados.

.. TODO: 1 milhão ou 1.048.576?

ATUAL
-----

Aqui, o usuário pode baixar as bases de dados mais recentes disponíveis no CECAD, conforme temporalidades explicadas na seção :ref:`doc_temporalidade`. É possível escolher três tipos de bases para baixar: com informações identificadas somente sobre famílias, somente sobre pessoas e com informações sobre famílias e pessoas. Nas bases com informações sobre famílias + pessoas, os dados relativos à família são repetidos nas linhas correspondentes às pessoas da família. Assim, você pode definir qual base de dados é a que melhor atende as suas necessidades. Para acessar tais informações sigilosas, é necessário aceitar o “TERMO DE COMPROMISSO DE MANUTENÇÃO DE SIGILO”.

.. figure:: /img/baixar/baixar.jpg

   Figura 1: menu para baixar dados atuais

ANOS ANTERIORES
---------------

Aqui, o usuário pode acessar baixar as bases de dados do Cadastro Único de anos anteriores, a partir de 2012, sempre com referência ao mês de dezembro de cada ano. É possível escolher três tipos de bases para baixar: com informações identificadas somente sobre famílias, somente sobre pessoas e com informações sobre famílias e pessoas. Nas bases com informações sobre famílias + pessoas, os dados relativos à família são repetidos nas linhas correspondentes às pessoas da família. Assim, você pode definir qual base de dados é a que melhor atende as suas necessidades. Para acessar tais informações sigilosas, é necessário aceitar o “TERMO DE COMPROMISSO DE MANUTENÇÃO DE SIGILO”.

Na figura abaixo temos a imagem da busca de anos anteriores:

.. figure:: /img/baixar/anteriores.jpg

   Figura 2: menu para baixar dados de referências anteriores

CONSULTA MÚLTIPLOS CPFs
-----------------------

Esta funcionalidade permite que você consulte se uma lista de CPFs pertence a pessoas inscritas no Cadastro Único no mês de referência solicitado. É possível realizar a consulta por duas opções: enviar arquivo com CPFs ou colar CPFs.

Na opção de enviar arquivo com CPFs, é necessário fazer upload de uma planilha em formato CSV contendo na primeira coluna os CPFs que devem ser consultados. Para isso, basta apertar o botão “Escolher arquivo” e selecionar o arquivo a ser consultado.

Na opção colar CPFs, copie os CPFs a serem consultados de uma planilha Excel e cole no campo indicado. Os dados devem conter somente números (retirar pontos, traços, barras ou espaços) e somente pode ser consultado até 5.000 números de CPF por vez.

.. Attention:: O CPF não é um documento obrigatório para o Cadastro Único. Assim, é possível que algum dos CPFs consultados não sejam localizados, mas estão inscritos no Cadastro Único, mas sem o CPF registrado. Para garantir que a pessoa está no Cadastro Único ou não, recomenda-se utilizar a funcionalidade **BUSCAR** ou consultar via *MeuCadÚnico*.

Nesta figura podemos ver a opção para o preenchimento com múltiplos CPFs:
 
.. figure:: /img/baixar/lote.jpg

   Figura 3: menu para baixar dados referentes a múltiplos CPFs

Enquanto o **Tabulador** e a **Frequência Simples** possibilitam uma visão mais agregada e sistemática das características das pessoas e famílias cadastradas, nos municípios, DF e estados pesquisados, as ferramentas **Buscar** e **Baixar** permitem a realização de estudos mais detalhados, onde a menor unidade de análise é a família ou a pessoa.

.. TODO: adicionar links para as respectivas páginas

HISTÓRICO DE DOWNLOADS
----------------------

Sempre que o usuário autenticado com permissão de acesso aos dados identificados do Cadastro Único baixa alguma base de dados no CECAD, tanto por meio do **TABCAD** como pelas funcionalidades de **BAIXAR**, o download do arquivo não se inicia imediatamente. A solicitação é agendada no sistema, entrando numa fila para extração:

.. figure:: /img/baixar/historico.jpg

   Figura 4: mensagem de confimação da solicitação dos dados

Quando o arquivo fica pronto para ser baixado, o usuário recebe o link para download do arquivo no e-mail cadastrado no CECAD. É necessário que o usuário se certifique de que possui acesso ao e-mail informado para que possa efetuar o download e verifique as caixas de *SPAM/Lixo eletrônico*, pois em alguns casos o e-mail pode ser redirecionado para elas.

.. figure:: /img/baixar/mensagem.jpg

   Figura 5: e-mail com o link para baixar o arquivo com os dados solicitados

Esse processo pode demorar, de acordo com a quantidade de arquivos na fila para extração, deste modo, o usuário deve aguardar até receber a confirmação por e-mail. O usuário também pode acompanhar a situação da solicitação através da página **HISTÓRICO DE DOWNLOADS**.

Na página **HISTÓRICO DE DOWNLOADS**, os usuários poderão consultar todos os arquivos de bases de dados solicitados no CECAD. Esses arquivos ficam disponíveis para download por até 3 dias após o seu processamento e só poderá ser baixado uma única vez. Após o prazo de 3 dias ou se o download já tiver sido realizado, o arquivo será considerado como *Expirado* e não estará mais disponível para download e necessitará ser regerado pelo usuário novamente.

Após o processamento de cada arquivo será enviado um e-mail para o requisitante informando a sua disponibilidade bem com o link para o download, porém, caso isso não aconteça, o usuário poderá utilizar essa página para baixar o arquivo.