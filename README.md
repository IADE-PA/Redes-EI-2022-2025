# Redes e Comunicação de Dados 2022-2023 - Engenharia Informática
*Conteudos da Unidade Curricular de Redes de Computadores em exclusivo no curso de ***Engenharia Informática 1º ano*** do IADE/Universidade Europeia*

O objectivo da cadeira é dotar os alunos de conhecimentos da concepção das componentes protocolares das redes de computadores, bem como de algumas componentes práticas de redes TCP/IP e de equipamentos activos de rede.

Existem vários trabalhos a serem realizados para alunos em **avaliação continua**. Nas aulas teóricas os alunos deverão escolher **um paper de investigação cientifica** sobre temas da cadeira (Networking/IoT) e apresentar um resumo oralmente para a turma. Nas aulas práticas existem **um cojunto de trabalhos práticos, de acordo com as matérias lecionadas nos laboratórios**, incluindo um trabalho final de maior envergadura que consiste em implementar uma rede multi-serviço com divisão de tráfego, incluindo equipamentos ativos de rede, terminais e componentes IoT.
Antes de certas aulas existem também **um conjunto de laboratórios** que devem ser feitos para que possam ser esclarecidas as duvidas durante as aulas. Estes laboratórios estão enquadrados nos trabalhos práticos da unidade curricular.

***Esforço requerido aos alunos: 6 ECTS, com 42 horas em aula e 126 horas fora do ambiente de aula***

### Horário 
| Dia | Hora | Turma |
| :-----------: | :-----------: | :----------: |
| Quarta-feira | 16:00 - 18:40 | T2 |
| Quinta-feira | 16:00 - 18:40 | T1 |

## Programa
### Aulas Teóricas
-	Introdução a Redes de Computadores & Aplicações 
-	Modelo OSI - tecnologias (ethernet, wifi, 5g)  e layer 2 - VLANs, etc
-	Modelo OSI - layer 3/routing
- Modelo OSI - layer 4/transporte
- Modelo OSI - camadas aplicacionais
- Internet (história/breve)
- TCP/IP arquitetura, Unicast, Multicast
-	TCP/IP pacotes IP / layer IP
-	TCP/IP ICMP, TCP, UDP / layer transporte
-	TCP/IP endereçamento IPv4 (inclui subnetting)
-	Protocolos (DNS, DHCP, HTTP, SNMP, etc)
-	IPv4 vs IPv6 enquadrar IPv6 como “obrigatório” nos dias de hoje
-	IPv6 features e endereçamento (inclui diferentes dimensões de redes e distinções na divisão com IPv4)
-	IPv6 e serviços (DNSv6 e DHCPv6)
-	IoT enquadrar com serviços de Cloud/associar a virtualização; Fog computing; necessidades de networking, armazenamento em IoT; exemplos práticos (smart homes, buildings, cities, veículos autónomos, etc); referencia a big data; referencia a segurança em IOT, nem que seja apenas com exemplos estilo Mirai botnet, etc)

*Slides com conteudos disponiveis no Canvas*

### Aulas Práticas:
- [Laboratórios práticos](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/AulasLabsPraticos.md) de TCP/IP (endereçamento IP, routing em máquinas virtuais e Cisco Packet Tracer)
- Inclui a utilização de máquinas virtuais e do simulador de rede Cisco Packet Tracer (ver [aqui](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/AulasLabsPraticos.md#0-preparação-dos-laboratórios--pré-requisitos) quais os passos preparatórios para a realização dos laboratórios). Existe um [roteiro](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/roteiro-packet-tracer.md) para as aulas Packet Tracer;
- Apoio a realização do trabalho prático sobre Networking/IoT em Cisco Packet Tracer.

### Planeamento PREVISTO (pode sofrer ALTERAÇÕES!!!)[#planeamento]
| Aula | Data | Aula |
| :-----------: | :-----------: | :---------- |
| 01 | 30 jan | Apresentação; Introdução a Redes de Computadores & Aplicações; Introdução ao Modelo OSI  |
| 02 | 06 fev | Modelo OSI - tecnologias (ethernet, wifi, 5g)  e layer 2 - VLANs, etc;	Modelo OSI - layer 3/routing; Modelo OSI - layer 4/transporte; ***Laboratório 1 ([pré-requisito 0.1](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/AulasLabsPraticos.md#01-instalação-do-cisco-packet-tracer-labs-13-e-6) para elaborar o laboratório)***  |
| 03 | 13 fev | Modelo OSI - camadas aplicacionais; Internet (história/breve); TCP/IP arquitetura, Unicast, Multicast; ***Laboratório 2 ([pré-requisito 0.1](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/AulasLabsPraticos.md#01-instalação-do-cisco-packet-tracer-labs-13-e-6) para elaborar o laboratório)***|
| 04 | 20 fev | TCP/IP pacotes IP / layer IP; TCP/IP ICMP, TCP, UDP / layer transporte; TCP/IP endereçamento IPv4; |
| 05 | 27 fev | TCP/IP endereçamento IPv4 ; ***Laboratório 3 ([pré-requisito 0.2](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/AulasLabsPraticos.md#02-instalação-de-máquinas-virtuais-em-equipamentos-dos-alunos-labs-24-e-5) para elaborar o laboratório)***|
| 06 | 06 mar | TCP/IP endereçamento IPv4 (inclui subnetting); |
| 07 | 13 mar | TCP/IP endereçamento IPv4 (inclui subnetting); ***Laboratório 4 ([pré-requisito 0.2](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/AulasLabsPraticos.md#02-instalação-de-máquinas-virtuais-em-equipamentos-dos-alunos-labs-24-e-5) para elaborar o laboratório)*** |
| 08 | 20 mar | ***Semana sem aulas*** |
| 0 | 27 mar | Inicio do estudo de alguns Protocolos TCP/IP; **Entrega do trabalho Routing-I**  |
|   | 03 abr | *Páscoa*|
| 09 | 10 abr | Protocolos (DNS, DHCP, HTTP, SNMP, etc) – essencial: saber exatemente como se resolvem os nomes; saber exatamente como se distribui endereçamento IP dinamicamente; IPv4 vs IPv6 enquadrar IPv6 como “obrigatório” nos dias de hoje; **Apresentação do trabalho Routing-I** |
| 10 | 17 abr | ***Laboratório 5 ([pré-requisito 0.2](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/AulasLabsPraticos.md#02-instalação-de-máquinas-virtuais-em-equipamentos-dos-alunos-labs-24-e-5) para elaborar o laboratório)***; **Entrega do trabalho Routing-II** |
| 11 | 24 abr | IPv6 features e endereçamento (inclui diferentes dimensões de redes e distinções na divisão com IPv4); IPv6 e serviços (DNSv6 e DHCPv6); Laboratório 5; **Apresentação do trabalho Routing-II** |
| 12 | 01 mai | IoT enquadrar com serviços de Cloud/associar a virtualização; Fog computing; necessidades de networking, armazenamento em IoT; exemplos práticos (smart homes, buildings, cities, veículos autónomos, etc); referencia a big data; referencia a segurança em IOT, nem que seja apenas com exemplos estilo Mirai botnet, etc); ***Laboratório 6 ([pré-requisito 0.1](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/AulasLabsPraticos/AulasLabsPraticos.md#01-instalação-do-cisco-packet-tracer-labs-13-e-6) para elaborar o laboratório)***; **Entrega Trabalho Captura de pacotes com Wireshark/tcpdump** | 
| 13 | 08 mai | Apoio ao trabalho prático Networking/IoT; (possível salvaguarda para a realização de laboratórios atrasados, caso seja possível); **Apresentação do Trabalho Captura de pacotes com Wireshark/tcpdump** |
| 14 | 15 mai | **Teste Escrito** ; **Entrega do trabalho final em Packet Tracer Redes/IOT** |
| 15 | 22 mai | **Apresentações dos trabalhos práticos Networking/IoT** |

### Sumários
Os sumários das aulas podem ser consultados *aqui* (brevemente disponível)

## Avaliação Continua

### 1. Regras de Avaliacao Continua

De acordo com o **Regulamento Geral de Avaliação de Conhecimentos e Competências da Universidade Europeia.** (REG-046lV08 retirado do Portal do Docente em 27.01.2023), os alunos poderão fazer **avaliação continua** sendo que essa avaliação *inclui vários momentos de avaliação*

Recorde-se que, segundo o regulamento "*(...)A avaliação contínua é aquela que, com caráter regular e constante, decorre
durante o período letivo, refletindo uma permanente interação entre o docente e o estudante, através da realização de vários instrumentos de avaliação, executados individualmente e/ou em grupo.*"

Sendo assim:
- Ainda segundo o regulamento: *Os elementos de avaliação utilizados têm de contemplar uma ponderação igual ou superior a 4O% referente à avaliação individual no cálculo da classificação final da unidade curricular*. **Na UC o valor para o teste escrito será de 40%**.
- A realização do teste escrito será realizado durante as aulas na data marcada na calendarização da UC

Nesta UC são instrumentos da avaliação contínua:
- o Trabalho Teórico (15%) individual que inclui apresentação à turma
- os Trabalhos Práticos (50%) em grupo que no trabalho final inclui apresentação
- o Teste Escrito Individual Final (35%). 

**Notas Muito Importantes:** 

**I** Não são admitidos à realização da prova escrita de avaliação continua, os estudantes que obtiverem uma classificação inferior a 8 (oito) valores na média dos elementos de avaliação previstos, neste caso o Trabalho Teórico (15%) individual e os os Trabalhos Práticos (45%) em grupo. Poderá, no entanto, não realizar alguns trabalhos desde que a média seja de no minimo 8 valores (sem arredondamentos). 

**II** Os alunos que iniciem com Avaliação Continua têm até 30 dias antes da última aula para passarem para Avaliação Final. Data indicativa para o fazerem é até **26 de abril**

**III:** Os alunos que continuem no sistema de Avaliação Continua e que tenham más notas em elementos de avaliação já posteriormente aos 30 dias antes da última aula, vão para Exame de Recurso não podendo passar a Avaliação Final.

**IV:** Os alunos que, estando em Avaliação Continua, não obtenham o número de presenças obrigatórios, passam para Exame de Recurso não podendo passar a Avaliação Final.

**V** Os alunos deverão ter uma taxa de presenças de 70% nas aulas ou 40% nos casos excecionados no regulamento.

### 2. Elementos da Avaliação Continua 

#### 1. Trabalho Teórico (15%)
O trabalho teórico baseia-se na apresentação de um paper. Valerá 15% para a classificação final da Unidade Curricular.Este trabalho é individual.
Consulte o [Enunciado](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/TrabT/TrabT.md) para efetuar a escolha do tema. 

Importante escolher até **10 de fevereiro**.

Depois de distribuídos os temas (até 12 de fevereiro) as datas de apresentação estarão disponiveis [aqui](https://docs.google.com/spreadsheets/d/e/2PACX-1vTMy_qe4OHB00CZkNnUHM5vwgfh-NAXmvV0Iw97bwfDhC_wPiRoRPmBdslhEjiprcHu2RkLrXByPwSB/pubhtml?gid=467007833&single=true).

As apresentações começam na semana de 20 de fevereiro.

#### 2. Trabalhos Práticos (50%)
Enunciados dos [Trabalhos Práticos](https://github.com/pmrosa-classes/Redes-EI-2022-2023/blob/main/TrabsP/TrabsPraticos.md) da unidade curricular. Este trabalho é em grupo (3 alunos no máximo, 2 alunos no minimo, 4 alunos não são aceites).

Importante respeitar as datas de entrega. Não serão aceites adiamentos.

#### 3. Teste Escrito (35%)

Teste Escrito unico a realizar na data marcada na calendarização (penultima semana de aulas).

## Avaliação Final

Ainda de acordo com o mesmo regulamento, os estudantes têm o direito a optar pelo regime de **avaliação final** (avaliação por exame) que integra uma prova escrita, ou outros elementos, sobre a matéria toda lecionada. Esta avaliação final ainda não está completamente definida mas, ou terá também elementos distintos da prova escrita, ou terá 60% do valor teórico/prático escrito (portanto relacionado com os laboratórios e trabalhos práticos).

## Presenças

Os alunos podem acompanhar a percentagem de aulas a que assistem através da disponibilização pública, em Google Sheets, referente à sua turmas:
- Presenças da [T01](https://docs.google.com/spreadsheets/d/e/2PACX-1vTMy_qe4OHB00CZkNnUHM5vwgfh-NAXmvV0Iw97bwfDhC_wPiRoRPmBdslhEjiprcHu2RkLrXByPwSB/pubhtml?gid=1412701734&single=true)
- Presenças da [T02](https://docs.google.com/spreadsheets/d/e/2PACX-1vTMy_qe4OHB00CZkNnUHM5vwgfh-NAXmvV0Iw97bwfDhC_wPiRoRPmBdslhEjiprcHu2RkLrXByPwSB/pubhtml?gid=933545162&single=true)

## Método Pedagógico
Aos alunos é fornecida toda a documentação utilizada durante as aulas, nomeadamente:
- Ficheiros pdf com os slides das aulas teóricas (Plataforma Canvas)
- Laboratórios Práticos com exercícios práticos para configuração dos equipamentos em simulador Cisco Packet Tracer e exercicios práticos com máquinas virtuais (neste repositório)

## Discord
Deverá ser util juntarem-se ao Discord da cadeira: https://discord.gg/u8GEzwNV (invite criado em 27.01.2023).

Para terem acesso aos canais do Discord devem alterar o vosso *nick* para PrimeiroUltimo nome no servidor e colocar uma mensagem em **#general** com "Numero - Primeiro&UltimoNome - Turma" para serem atribuídos os roles adequados.

## Grupos
Os trabalhos práticos são em grupo (3 alunos no máximo, 2 alunos no minimo, 4 alunos não será admitido em nenhuma situação) e deve ser preenchida a tarefa respetiva no Canvas até dia 10 de fevereiro: https://mycampus.pt/courses/7345/assignments/8738.

A contituição dos grupos será disponibilizada [aqui](https://docs.google.com/spreadsheets/d/e/2PACX-1vTMy_qe4OHB00CZkNnUHM5vwgfh-NAXmvV0Iw97bwfDhC_wPiRoRPmBdslhEjiprcHu2RkLrXByPwSB/pubhtml?gid=592821258&single=true) 

## Resumo do Calendário da UC
*(em atualização)*
- até 10 de fevereiro - Escolha dos temas para os trabalhos teóricos (ver tarefa necessária para preencher)
- até 12 de fevereiro - Publicação [aqui](https://docs.google.com/spreadsheets/d/e/2PACX-1vTMy_qe4OHB00CZkNnUHM5vwgfh-NAXmvV0Iw97bwfDhC_wPiRoRPmBdslhEjiprcHu2RkLrXByPwSB/pubhtml?gid=467007833&single=true) da distribuição dos temas e datas de apresentação
- até 10 de fevereiro - Constituição dos grupos (ver tarefa necessária para preencher)
- a partir de 20 de fevereiro iniciam-se as apresentações dos trabalhos teóricos 
- até 31 de março - Trabalho de Routing I - Ponderação: 7,5%
- até 21 de abril - Trabalho de Routing II - Ponderação: 7,5%
- até 5 de maio - Trabalho Captura de pacotes com Wireshark/tcpdump - Ponderação: 5%
- até 19 de maio - Trabalho Cisco Packet Tracer / IoT - Ponderação: 25%
- semana de 22 e 26 de maio - Apresentações dos Trabalhos Cisco Packet Tracer / IoT 

## Bibliografia
- Computer Networks, Tanenbaum, Andrew S., Prentice Hall http://books.google.pt/books?id=Pd-z64SJRBAC
- Engenharia de Redes Informáticas, Edmundo Monteiro, Fernando Boavida, Editora FCA

## Log
- 2023.01.27: Disponibilização do Repositório.
