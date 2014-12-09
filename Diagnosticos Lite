#Diagnósticos Lite#

#Plano de Gerenciamento de Configuração#

#LITE – PGC – v.1.0#

# Histórico de Versões

<table>
  <tr>
    <td>Data</td>
    <td>Versão</td>
    <td>Descrição</td>
    <td>Autor</td>
  </tr>
  <tr>
    <td>08/12/2014</td>
    <td>V.1.0</td>
    <td>Criação do documento</td>
    <td>Elsa Martins</td>
  </tr>
  <tr>
    <td><dd/mm/aaaa></td>
    <td><1.1></td>
    <td></td>
    <td><autor></td>
  </tr>
</table>



# 1. Introdução

Este documento descreve o Plano de Gerência de Configuração para o projeto de desenvolvimento do sistema CFC – Controle de Fluxo de Cheques.

## 1.1 Finalidade

*[Especifique a finalidade deste Plano de Gerenciamento de Configuração.]*

## 1.2 Escopo

*[Uma breve descrição do escopo deste Plano de Gerenciamento de Configuração; o modelo ao qual ele está associado e tudo o que é afetado ou influenciado por este documento.]*

## 1.3 Definições, Acrônimos e Abreviações

*[Esta subseção apresenta as definições de todos os termos, acrônimos e abreviações necessários para a correta interpretação do Plano de Gerenciamento de Configuração. Essas informações podem ser fornecidas mediante referência ao Glossário do projeto.]*

## 1.4 Referências

*[Esta subseção apresenta uma lista completa de todos os documentos mencionados no Plano de Gerenciamento de Configuração. Identifique os documentos por título, número de relatório (se aplicável), data e organização responsável pela publicação. Especifique as fontes a partir das quais as referências podem ser obtidas. Essas informações podem ser fornecidas por um anexo ou outro documento.]*

## 1.5 Visão Geral

*[Esta subseção descreve o conteúdo restante do Plano de Gerenciamento de Configuração e explica como o documento está organizado.]*

# 2. Gerenciamento de Configuração de Software

## 2.1 Organização, Responsabilidades e Interfaces

### 2.2.1 Organização

As seções subsequentes deste documento estão organizadas: 

* Seção 2 descreve os papeis e responsabilidades da gerência de configuração, ferramentas utilizadas, ambiente e infraestrutura; 

* Seção 3 é apresenta o plano de configuração onde é definido como serão identificados os itens configuráveis, como será o agrupamento desses itens, as configurações bases do projeto, a estrutura do repositório e o controle de acesso; 

* Seção 4 define como serão feitas as requisições à GC, padronizando um processo a ser seguido; 

* Seção 5 define quais os treinamentos e recursos necessários para implantação da GC;

* Seção 6 apresenta o cronograma das auditorias de configuração e o que será verificado.

## 2.2 Ferramentas, Ambiente e Infraestrutura

### 2.1.1 Ferramentas utilizadas para gerência de configuração

<table>
  <tr>
    <td>Software</td>
    <td>Propósito</td>
    <td>Ambiente</td>
    <td>Release/Versão</td>
  </tr>
  <tr>
    <td>Git</td>
    <td>Controle de Repositório</td>
    <td>Desenvolvimento. Ambiente configurado em servidor interno.
Capacidade máxima de armazenamento: 1Tb</td>
    <td></td>
  </tr>
  <tr>
    <td>TortoiseGIT</td>
    <td>Acesso ao repositório </td>
    <td>Desenvolvimento.
Acessa o repositório local.</td>
    <td>1.8.12.0</td>
  </tr>
</table>


### 2.1.2 Ferramentas do ambiente de desenvolvimento

<table>
  <tr>
    <td>Software</td>
    <td>Propósito</td>
    <td>Ambiente</td>
    <td>Release/Versão</td>
  </tr>
  <tr>
    <td>Sistema Operacional</td>
    <td>Windows 7 x64/ Ubuntu 12.10</td>
    <td>Desenvolvimento</td>
    <td></td>
  </tr>
  <tr>
    <td>Máquinas Virtuais</td>
    <td>VMWare Player</td>
    <td></td>
    <td>6.0.2</td>
  </tr>
  <tr>
    <td>MS-Office</td>
    <td>Documentos do Word</td>
    <td>Todos</td>
    <td>2013</td>
  </tr>
  <tr>
    <td>MS-Project</td>
    <td>Edição do cronograma</td>
    <td>Desenvolvimento</td>
    <td>2010</td>
  </tr>
  <tr>
    <td>Qt </td>
    <td>Desenvolvimento C++</td>
    <td>Desenvolvimento</td>
    <td>4.7.4</td>
  </tr>
  <tr>
    <td>Visual Studio</td>
    <td>Desenvolvimento C++</td>
    <td>Desenvolvimento</td>
    <td>2010</td>
  </tr>
  <tr>
    <td>Enterprise Architect</td>
    <td>Modelagem de diagramas de dados</td>
    <td>Todos</td>
    <td>8.0.863</td>
  </tr>
  <tr>
    <td>JIRA</td>
    <td>Controle de atividades e documentação de TS, REQ e Testes</td>
    <td>Todos</td>
    <td>6.4</td>
  </tr>
</table>


### 2.1.3 Estrutura do Ambiente

<table>
  <tr>
    <td>Ambiente</td>
    <td>Descrição</td>
    <td>Transição</td>
  </tr>
  <tr>
    <td>Desenvolvimento</td>
    <td>Ambiente que servirá para desenvolvimento da aplicação</td>
    <td>Uma "feature" será considerada finalizada quando todo o requisito for implementado e validado através de testes unitários e revisão de código.</td>
  </tr>
  <tr>
    <td>Integração</td>
    <td>Ambiente em que serão realizados os testes de integração</td>
    <td>Quando uma ou mais “features” estão implementadas e com um nível satisfatório de integração. </td>
  </tr>
  <tr>
    <td>Release</td>
    <td>Ambiente em que as versões serão geradas</td>
    <td>Quando uma ou mais “features” planejadas estão integradas e prontas para validação.</td>
  </tr>
</table>


# 3. O Programa de Gerenciamento de Configuração

## 3.1 Identificação da Configuração

### 3.1.1 Métodos de Identificação

*[Descreva como os artefatos do projeto ou produto devem ser nomeados, marcados e numerados. O esquema de identificação deve abranger o hardware, o software do sistema, os produtos de terceiros (COTS) e todos os artefatos de desenvolvimento de aplicativos listados na estrutura de diretórios do produto; por exemplo, planos, modelos, componentes, software de teste, resultados e dados, executáveis e assim por diante.]*

### 3.1.2 Itens de Configuração

*[Relacionar os artefatos ou grupos de artefatos, separando por tipo, modulo ou subsistema, responsável ou momento em que deverão ser incluídos em baselines.*

* *"Inclusão em Baseline" em branco significa que o grupo de artefatos não participará de baseline. Pode ser expresso como uma data ou identificador de uma baseline, fase ou ponto de controle*

* *"Responsável": indicar nominalmente, sempre que possível]*

<table>
  <tr>
    <td>Item (ou Tipo de Item)</td>
    <td>Responsável na equipe</td>
    <td>Inclusão em Baseline</td>
  </tr>
  <tr>
    <td><grupo de itens de configuração></td>
    <td><nome do responsável></td>
    <td><momento a partir do qual o conjunto de artefatos será incluído em baseline></td>
  </tr>
</table>


### 3.1.3 Baselines do Projeto

*[As baselines funcionam como um padrão oficial no qual os trabalhos subseqüentes são baseados. Somente mudanças autorizadas podem ser efetuadas nas baselines.* *Descreva em que pontos do ciclo de vida do projeto ou produto as baselines devem ser estabelecidas. As baselines mais comuns devem ser definidas ao final de cada uma das fases de Iniciação, Elaboração, Construção e Transição. Elas também podem ser geradas no final de iterações ocorridas dentro das várias fases ou com freqüência ainda maior.* *Descreva quem autoriza uma baseline e o que ela contém.]*

### 3.1.4 Estrutura do Repositório de Versões

*[Descreva a organização de diretórios do seu repositório e que itens/arquivos devem ser armazenados em cada diretório.]*

## 3.2 Controle de Configuração e Mudança

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança

As solicitações de mudanças nas "Baselines" devem ser registradas na ferramenta JIRA, no projeto “Change Request”, obedecendo o seguinte fluxo:

![image alt text](image_0.png)

### 3.2.2 Comitê de Controle de Mudança (CCB)

<table>
  <tr>
    <td>Responsáveis:</td>
    <td>Funções:</td>
  </tr>
  <tr>
    <td>Analista de Sistemas</td>
    <td>Recebe solicitação de mudança e realiza estudo do impacto da realização da mudança.</td>
  </tr>
  <tr>
    <td>Gerente de Projetos</td>
    <td>Analisa a viabilidade da implementação com base no estudo de impacto. Responsável por planejar a realização da mudança e estimar os prazos.</td>
  </tr>
  <tr>
    <td>Gerente de Configuração</td>
    <td>Verifica o que será necessário para integrar a mudança, garantindo integridade do que não foi alterado</td>
  </tr>
</table>


# 4. Padrões e Procedimentos

## 4.1 Padrão de Estrutura de Pastas 

O projeto deverá seguir a seguinte estrutura de pastas e subpastas no repositório:

<table>
  <tr>
    <td>Git <br />
+-branches <br />
|  +-Lite 4.1.0_VideoCard <br />
    |  +-Acompanhamento e Controle <br />
    |  +-Construção <br />
    |  |  +-Análise <br />
    |  |  +-Implementação <br /> 
    |  |  +-Revisão de Código <br />
    |  |  +-Testes <br />
   |  +-Planejamento e Elaboração <br />
    |  |  +-Especificação Técnica <br />
    |  |  +-Requisitos <br />
    |  |  +-Planejamento de Teste <br />
    |  |  +-Planejamento de Desenvolvimento <br />
+-tags <br />
 |  +-<VERSÃO > - <ID > <br />
    |  +-Lite 4.0.0 <br />
+-master <br />
 |  +-Lite 4.1.0 <br />
    |  +-Acompanhamento e Controle <br />
    |  +-Construção <br />
    |  |  +-Análise <br />
    |  |  +-Implementação <br />	
    |  |  +-Revisão de Código <br />
    |  |  +-Testes <br />
    |  +-Planejamento e Elaboração <br />
    |  |  +-Especificação Técnica <br />
    |  |  +-Requisitos <br />
    |  |  +-Planejamento de Teste <br />
    |  |  +-Planejamento de Desenvolvimento <br />
</td>
  </tr>
</table>


Se em algum determinado momento do projeto a estrutura de pastas não atender as necessidades, será gerada uma adaptação e esta deverá ser descrita no Plano de Projeto.

A movimentação dos arquivos nas diferentes pastas ficará a cargo do Gerente de Configuração.

# 5. Treinamento e Recursos

*[Descreva as ferramentas de software, o pessoal e o treinamento necessários para implementar as atividades de CM especificadas.]*

# 6. Auditorias de Configuração

O cronograma de verificações de Gestão de Configuração deve ser planejado na Ferramenta de Gestão de Projetos – MS Project. Este cronograma será elaborado a cada Release (ciclo de vida até a entrega para o cliente) e conterá todas as atividades de GC do projeto. Elas podem ainda, estar planejadas no Gmail, para facilitar a integração com o calendário das pessoas que serão diretamente afetadas.
Se, durante as audições, forem detectadas falhas na Gestão de Configuração, o auditor responsável deverá criar uma requisição de mudança no projeto "Auditoria", que se encontra na ferramenta JIRA e segue o mesmo modelo de aprovação de uma solicitação de mudança de “baseline” (seção *3.2.1 Processamento e Aprovação de Solicitações de Mudança*), atribuindo esta requisição ao Gerente de Configuração, que irá avaliar se será realizada ou não a mudança.