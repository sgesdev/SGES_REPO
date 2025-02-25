---
layout: default
title: "Your first markdown webPage using git"
description: "index page how to show markdown files on html."
published_on: 2015-09-30
updated_on: 2015-10-06
translation_priority: 1
order: 3
---
<p id="equipamentos"></p>

# 13. Equipamentos

Neste módulo são feitas ações sobre os equipamentos. 
Estas só poderão ser realizadas caso no separador *Estabelecimento* esteja indicado que existe equipamento médico pesado. Apenas entidades públicas, à exceção de ACES e ARSs, podem possuir equipamento médico pesado.
O utilizador pode consultar a lista de equipamentos associados a um estabelecimento através do separador *Equipamentos* ([](#figEqpEstabelecimento))

![figEqpEstabelecimento](img/pages/cap12/12_1_v1.jpg)

<p class="caption" id="figEqpEstabelecimento"> Equipamentos de um estabelecimento</p>

<p id="criaEquipamento"></p>

## 13.1. Criar Equipamento
Para criar um novo equipamento, o utilizador pode clicar em **CRIAR** na página de equipamentos de um estabelecimento ([](#figEqpEstabelecimento)) à qual pode aceder através do menu Entidade ou do menu Equipamentos.
Na página de criação de equipamento, o utilizador deverá preencher os campos obrigatórios do painel *Identificação* para poder 
efetuar o registo do equipamento.

<p id="identificao"></p>
### 13.1.1. Identificação

|    | Campos Obrigatórios da Identificação do Equipamento ([](#figCriarEquipamento))         |     |
|----|----------------------------------------------------|----------|
| a) | Designação                                         |      |
| b) | Tipo de Equipamento                                         |  Equipamentos Médicos Pesado    |
|    |                                                             |  Outros Equipamentos Médicos    |
| c) | Equipamento é Novo ou Upgrade?                                         |  NOVO    ||
|    |                                                             |  UPGRADE**    | Nr. de Série do equipamento a ser substituído|
| d) | Número de série                                    |      |
| e) | Posto de trabalho (todos os serviços a que um equipamento se encontra associado devem ser considerados)                           |      |
| f) | Marca                                              |      |
| g) | Modelo                                             |      |
| h) | Se Designação = Acelerador Linear,Angiógrafo,Câmara Gama, Câmara Hiperbárica,RM, RM (Dedicada exclusivamente à Radioterapia),TC ou TC (Dedicada exclusivamente à Radioterapia)                           |Característica Técnica|
| i) | Se Tipo de Equipamento = Outros Equipamentos Médicos                           |Especificações Técnicas| 
| j) | Produção para Exterior?                          | Sim     |
|    |                                                  | Não     |
| k) | O equipamento é partilhado por mais alguma entidade? | Sim| A entidade pertence ao SNS?| |Sim| Tipo de Entidade| |Entidade*|
|    |                                                      |Não| Qual o nome da entidade?|    ||     |||

\* Para que seja possível selecionar a entidade o utilizador deve, primeiro, selecionar o tipo de entidade.

** A opção "UPGRADE" deve ser utilizada nos casos em que o equipamento que está a ser criado seja a substituição de um equipamento anterior. Esta opção apenas se aplica se o equipamento a ser substítuido estiver com o estado assinalado como "Substituido/Upgrade" (ver tabela Localização/Estado para alteração do estado). Esta opção abre um campo de pesquisa, onde é possível pesquisar o equipamento a substituir por designação, marca e número de série ([](#figPesquisaUpgrade)).

![figCriarEquipamento](img/pages/cap12/12_1_1_1_v1.png)

<p class="caption" id="figCriarEquipamento"> Criar novo Equipamento - Identificação</p>

![figPesquisaUpgrade](img/pages/cap12/40.1.jpg)

<p class="caption" id="figPesquisaUpgrade"> Menu de pesquisa de equipamento a ser substituido </p>

Após o registo dos dados deve clicar em **GUARDAR** para gravar o equipamento. Após clicar irá ser notificado com o resultado da operação.

<p id="outros-painis"></p>
### 13.1.2. Outros painéis

|    | Outros módulos a preencher                 |
|----|--------------------------------------------| 
| a) | Contratação ([](#figContratacao))            |
| b) | Localização/Estado ([](#figLocalizacao))     |
| c) | Manutenção  ([](#figManutencao))
| d) | Atividade   ([](#figAtividade))            |
| e) | Autorização Ministerial / Licença de Instalação ([](#figAutorizacao))|
| f) | Recursos Humanos Afetos ([](#figRhAfetos))|


|    | Campos Obrigatórios do módulo Contratação ([](#figContratacao))                                      |
|----|------------------------------------------------------------------------------------------------------|
| a) | Se Tipo de Contrato = Aquisição, Concessão, Locação/Leasing, Oferta |  Nº inventário/ID Equipamento                                       | 
|    |                                |  Data de publicação da abertura do concurso                         |
|    |                                | Custo de aquisição                                                   |
|    |                                | Data de ínicio de funcionamento                                      |
| b) | Se Tipo de Contrato = Outros |  Nº inventário/ID Equipamento                                       | 
|    |                                |  Data de publicação da abertura do concurso                         |
|    |                                | Custo de aquisição                                                   |
|    |                                | Data de ínicio de funcionamento                                      |
|    |                                | Especificações (tipo de contrato Outros)                             |

![figContratacao](img/pages/cap12/12_1_2_1.jpg)

<p class="caption" id="figContratacao"> Criar novo Equipamento - Contratação</p>

|    | Campos Obrigatórios do módulo Localização/Estado ([](#figLocalizacao)) | | |
|----|----------------------------------------------------|----------||
| a) | Estado                               		      | Abatido    ||
||                                                        | Avariado    ||
||                                                        | Em Funcionamento ||
||                                                        | Não Instalado ||
||                                                        | Parado       ||
||                                                        | Substituido/Upgrade       ||
| b) | Instalação Fixa				                      | Sim| Localização |
||                                                        | Não ||
| c) | Se Estado = Abatido ou Substituido/Upgrade         | Data de Alteração do Estado||
| d) | Se Estado = Avariado                    	          | Data de Alteração do Estado||
|    |                                                    | Motivo ||
| e) | Se Estado = Não instalado ou Parado                | Motivo ||

![figLocalizacao](img/pages/cap12/12_1_2_2_v1.jpg)

<p class="caption" id="figLocalizacao"> Criar novo Equipamento - Localização/Estado</p>

|    | Campos Obrigatórios do módulo Atividade ([](#figAtividade)) | | 
|----|----------------------------------------------------|----------|
| a) | Tipo Atividade                               	| Partilhada (Programada/Urgência) |
||                                                      | Programada    |
||                                                      | Urgência ||
| b) | Se Estado diferente urgência				        | Carga Semanal| 
| c) | Se Estado diferente urgência				        | Nº dias por semana| 
| d) | Tipo de Utilização                    	        | Exclusiva do serviço* |
|                                                       | Partilhada por Diferentes Serviços |

\* Caso o tipo de utilização seja exclusiva do serviço, têm de existir os serviços que constam nas especialidades do estabelecimento ([](#figEspecialidade)).

![figAtividade](img/pages/cap12/12_1_2_4.PNG)

<p class="caption" id="figAtividade"> Criar novo Equipamento - Atividade</p>


|    | Campos Obrigatórios do módulo Manutenção ([](#figManutencao)) ||
|----|----------------------------------------------------|----------|
| a) | Ano               			                	  | |
| b) | Tipo de Manutenção                           	  | Corretiva|
|	|        		                         	          | Preventiva |
|	|        		                         	          | Preventiva e Corretiva |
| c) | Duração   Contrato                           	  | Anual|
|	|        		                         	          | Bianual |
|	|        		                         	          | Quadrienal |
|	|        		                         	          | Quinquenal |
|	|        		                         	          | Semestral |
|	|        		                         	          | Trianual |
| d) |  Se Tipo de Manutenção = Corretiva, Preventiva ou Preventiva e Corretiva | Preventiva com Peças|
| e) | Se Designação=TC, com ampola                       | Sim |
|	|        		                         	          | Não |
| f) | Detetores                              	          | Sim |
|	|        		                         	          | Não |
| g) | Outros                             	          	  |  |
| h) | Nome da empresa                            	      |  |
| i) | Custo                             	          	  |  |
| j) | Horas de paragem/Ano                                   |  |


![figManutencao](img/pages/cap12/12_1_2_3.PNG)

<p class="caption" id="figManutencao"> Criar novo Equipamento - Manutenção</p>


|    | Campos Obrigatórios do módulo Autorização Ministerial/ Licença de Instalação ([](#figAutorizacao)) | | |
|----|----------------------------------------------------|----------|--|
| a) | Autorização Ministerial*                         	  | Sim||
||                                                   	  | Não||
| b) | Instalação licenciada pela DGS?                    | Sim| Data da Licença* |
||                                                   	  | Não||
| c) | Observação                                         |    | |                   

\* O campo *autorização ministerial* não é aplicável para equipamentos com Designação =Câmara Hiperbárica, RM, RM (Dedicada Exclusivamente à Radioterapia), Robot Cirúrgico (tipo D’avinci), Simulador, TC, TC-Simulador e TC (Dedicada exclusivamente à radioterapia); 

Depois de o utilizador selecionar a data da licença, o campo *período de vigência* (que se encontra sempre inativo) fica, automaticamente, preenchido com 5 anos.

![figAutorizacao](img/pages/cap12/12_1_2_5.jpg)

<p class="caption" id="figAutorizacao"> Criar novo Equipamento - Autorização Ministeria/ Licença de Instalação</p>

Depois de preencher cada um dos painéis referidos anteriormente  utilizador deve clicar em **GUARDAR** para que a informação fique gravada.

Para o utilizador aceder ao painel *Recursos Humanos Afetos*([](#figRhAfetos)) deverá clicar na *tab* respectiva, e selecionar o ano pretendido.
Para que o botão **CRIAR** esteja ativo, é necessário que o campo *Data de Início de Funcionamento* do campo *Contratação* esteja preenchido.
O utilizador tem, ainda, a possibilidade de replicar a informação do ano imediatamente anterior ao selecionado. 
Após clicar em **ALTERAR** irá ser notificado com o resultado da operação.

|    | Campos Obrigatórios do módulo Recursos Humanos Afetos ([](#figRhAfetos)) | | 
|----|----------------------------------------------------|----------|
| a) | Ano               			                	  | |
| b) | Grupo Profissional                         	      | |
| c) | Área Afetação   		                           	  | |
| d) | ECTS 		   		                           	  | |


![figRhAfetos](img/pages/cap12/12_1_2_6.PNG)

<p class="caption" id="figRhAfetos"> Criar novo Equipamento - Recursos Humanos Afetos</p>


<p id="alteraEquipamento"></p>

## 13.2. Editar Equipamento

A página de edição de um equipamento está disponível através da consulta de equipamento clicando no botão **EDITAR EQUIPAMENTO**. O utilizador pode aceder
a esta página através do menu Entidade ou, diretamente, através do menu Equipamentos.

 Na página de equipamentos de um estabelecimento ([](#figEqpEstabelecimento)) o utilizador pode navegar diretamente para a edição após selecionar um equipamento da lista e clicar no botão **EDITAR**.
A edição deve respeitar o preenchimento dos campos obrigatórios identificados no ponto [13.1 Criar Equipamento](#criar-equipamento).
Para gravar as alterações o utilizador  deve clicar no botão **GUARDAR**. Após clicar irá ser notificado com o resultado da operação.
O utilizador pode navegar entre os equipamentos do estabelecimento clicando em **SEGUINTE** ou **ANTERIOR**.

<p id="consultaEquipamento"></p>

## 13.3. Consultar Equipamento

Na página de equipamentos de um estabelecimento ([](#figEqpEstabelecimento)), o utilizador pode navegar diretamente para a consulta após selecionar um equipamento da lista e clicar no botão **CONSULTAR**. O utilizador pode aceder
a esta página através do menu Entidade ou, diretamente, através do menu Equipamentos.

<p id="transfereEquipamento"></p>

## 13.4. Transferir Equipamento

Na página de equipamentos de um estabelecimento([](#figEqpEstabelecimento)), o utilizador pode navegar diretamente para a página de transferência de equipamento após selecionar um equipamento da lista e clicar no botão **TRANSFERIR**. O utilizador pode aceder
a esta página através do menu Entidade ou, diretamente, através do menu Equipamentos.
Para poder transferir o equipamento, o utilizador deve preencher os campos obrigatórios e clicar em **TRANSFERIR**.

|    | Campos Obrigatórios para transferir equipamento ([](#figTransfEquipamento))         |
|----|----------------------------------------------------|
| a) | Data de Fim                                        | 
| b) | Motivo                                             | 
| c) | Tipo de Entidade                                   | 
| d) | Entidade                                           | 
| e) | Estabelecimento                                    | 

![figTransfEquipamento](img/pages/cap12/12_4_1_v1.jpg)

<p class="caption" id="figTransfEquipamento"> Transferir Equipamento</p>

<p id="historicoEquipamento"></p>

Na página de transferência o utilizador pode consultar toda a informação respeitante ao equipamento que vai transferir.

## 13.5. Histórico de Equipamento
A página de histórico de um equipamento pode ser acedida através da página de equipamentos de estabelecimento ([](#figEqpEstabelecimento)), ou através da página do equipamento no canto superior direito ([](#figCriarEquipamento)), clicando no botão **HISTÓRICO**.
O utilizador pode aceder a esta página através do menu Entidade ou, diretamente, através do menu Equipamentos.
Uma vez na página de histórico, o utilizador poderá visualizar as versões resultantes da edição da entidade, a data em que as alterações foram efetuadas, o utilizador que as realizou, identificação dos campos alterados, bem como a informação anterior e a informação nova. O menu permite ainda pesquisa das alterações efetuadas através de filtros como intervalo de tempo (data de - data até), Seccção, Utilizador, ou Campo ([](#figMenuHistorico)). É ainda possível efetuar a extração do resultado da pesquisa realizada. Este menu apenas apresenta as próprias alterações, apenas com as devidas permissões, apresenta todo o histórico de alterações de todos os utilizadores.

![figMenuHistorico](img/pages/cap12/40.1.1.jpg)
<p class="caption" id="figMenuHistorico"> Menu do histórico de alterações do equipamento</p>

