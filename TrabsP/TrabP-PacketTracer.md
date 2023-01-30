# Trabalho Prático - Packet Tracert Networking/IoT (27,5%)

*Este trabalho prático deve ser realizado no simulador Cisco Packet Tracer utilizado nas aulas práticas*

**Enunciado temporário. Pode sofrer alterações**

# A Smart Campus: Smart Factory & Smart Buildings

## Implementação de todas as componentes de uma rede de suporte a uma Empresa, incluindo equipamentos IoT associados aos edificios inteligentes da empresa.

**Descrição genérica do trabalho:**
1.	O objetivo principal é concretizar uma rede de uma empresa que interliga vários equipamentos de rede e equipamentos IoT (Internet of Things).
2.	A empresa está sediada num *Campus* de dimensão significativa no Oeste de Portugal.
3. Atualmente é composta por quatro contruções (edifício A, fábrica F e datacenter D) mas o *Campus* tem capacidade para um crescimento significativo em número de edificios;
4.  A utilização de equipamentos IoT para gerir os espaços é fundamental para a empresa, com vista a contribuir positivamente para o meio ambiente e ao mesmo tempo reduzir os custos e aumentar a qualidade de vida no *Campus*. Esse foi também o motivo de ter feito um quarto pequeno edificio exclusivamente para Datacenter.
5.	O primeiro edifício (A) têm 5 andares que aloja um total de ~150 funcionários, estando previsto a duplicação do número de funcionários nos próximos 3 anos, caso a evolução da empresa se mantenha nos atuais níveis. 
6.	Tendo o edifício uma largura de cerca de 80m, o seu backbone é duplo, ou seja, dois bastidores por piso (devidamente espaçados), interligados a um lugar central no piso 1. 
7.	A Fábrica (F) além de infraestrutura de rede tem um elevado numero de equipamentos IoT, uns wired e outros wireless, necessitando de infraestrutura de rede capaz de suportar todos esses equipamentos.
8.	O Datacenter (D) fica localizado num pequeno edificio, construído para o efeito, onde estão também centralizadas as comunicações.
9.	A infraestrutura central de rede e o acesso à Internet estão dentro do Datacenter.
10.	Os edifícios têm ainda a infraestrutura necessária para interligar diversas componentes de IoT para suporte à gestão inteligente do campus e dos edifícios.
11. Todos os pisos têm disponíveis 4 pontos de acesso sem fios por piso.
12. A empresa têm ainda atualmente muitos funcionários a trabalhar remotamente devido à pandemia.

**Objetivos a concretizar:**
1.	Elaborar um relatório com a descrição da empresa e tecnologias utilizadas, incluindo diagramas de rede.
2.	Para tal deve escolher um negócio imaginário e caracterizar a empresa de forma adequada e justificada (máximo de duas páginas A4).
3.	O objetivo principal do trabalho é planear, instalar e configurar a rede necessária para servidores, postos de trabalho, portáteis/telemoveis, equipamentos IoT (que suportem a gestão inteligente do Campus e dos Edificios) e capacidade de acesso remoto para tele-trabalho.
4.	Os mapas de rede deverão ser claros e organizados, eventualmente utilizando anotações necessárias para explicações necessárias.
5.	Deverão quantificar o número de switchs a colocar nos pisos dos edifícios e na fábrica, tendo em conta o número de funcionários da empresa e uma margem que considerem interessante para crescimento imediato. No edificio (A) os funcionários estão espalhados de forma muito semelhante a partir piso 2. O piso 1  tem cerca de 50% dos funcionários dos restantes pisos uma vez que há espaços ludicos e de refeição em ambos os locais.
6.	Deverão escolher os equipamentos mais adequados a colocar no edifício, fábrica e Datacenter, sabendo que apenas existe routing no Datacenter.
7.	Os equipamentos devem ter as portas necessárias configuradas e com respetivas descrições.
8.	A escolha dos modelos dos equipamentos e sua respetiva configuração a nível de hardware é da responsabilidade dos grupos, que devem ser capazes de justificar as suas escolhas (*conselho: não "inventar" muito em relação ao utilizado nos laboratórios práticos*).
9.	Devem ser usadas, pelo menos, as seguintes VLANs, dependendo muito do negócio escolhido a necessidade de existirem mais:
```
VLAN 2 – 172.16.2.0/24 – 2001:1:1:2::/64 – servidores (DHCP, DNS)
VLAN 3 – 172.16.3.0/24 – 2001:1:1:3::/64 – servidores (Web, Mail, IoT)
VLAN 10 – 172.16.10.0/22 – 2001:1:1:10::/64 – IoT
VLAN 20 – 172.16.20.0/24 – 2001:1:1:20::/64 – Apoio Administrativo/Financeiro
VLAN 21 – 172.16.21.0/24 – 2001:1:1:21::/64 – Recursos Humanos
VLAN 22 – 172.16.22.0/24 – 2001:1:1:22::/64 – Marketing/Comunicação
VLAN 23 – 172.16.23.0/24 – 2001:1:1:23::/64 – Direção
VLAN 25 – 172.16.25.0/24 – 2001:1:1.25::/64 – Equipamentos portáteis / rede sem fios
VLAN 30 – 172.16.30.0/24 – 2001:1:1:30::/64 – Laboratórios (ou algo adequado ao negócio)
VLAN 50 – 172.16.50.0/24 – 2001:1:1:51::/64 – Investigação (ou algo adequado ao negócio)
VLAN 60 - 172.165.60.0/22 - 2001:1:1:60::/64 - Fábrica
```
10.	Devem ser utilizados vários servidores no Datacenter:
```
VLAN 2 - srv01 – 172.16.2.11 - DHCP  – com configuração de todas as pools necessárias para postos de trabalho e equipamentos IoT.   
VLAN 2 - srv02 - 172.16.2.12 - Servidor Primário DNS - Deverão ser colocados os registos dos nomes de todos os servidores no DNS.
VLAN 2 - srv03 - 172.16.2.13 - Servidor VPN
VLAN 3 - srv04 – 172.16.3.11 - Servidor de HTTP - com página levemente customizada da Instituição
VLAN 3 - srv05 – 172.16.3.12 - Servidor de Mail – exemplificar com 10 contas de mail
VLAN 3 - srv06 – 172.16.3.13 - Servidor de Registo de IoT - para todos os equipamentos IoT da empresa.
```
11.	Sendo edifícios inteligentes, devem ser implementadas as seguintes funcionalidades:
-	Gerir a **temperatura** interna em cada edifício através de um display adequado.
-	Os edifícios têm **sistema de deteção de incêndios** em todos os pisos. Caso seja detetado um incendio deve tocar uma **sirene** e **ligado o sistema de extinção de incêndios**.
-	Os edifícios têm **sensores de CO2**. Uma vez detetado um valor superior a 75% as **janelas devem ser abertas** e a **extração de ar deve ser ligada**. Todo o sistema deve ser desligado quando voltarem a valores inferior a 60%.
-	Os edifícios têm **sensores de mónoxido de carbono**. Uma vez detetado as **janelas devem ser abertas** e a **extração de ar deve ser ligada**
-	As portas de entrada dos edifícios têm **controlo por RFID**. Só os utilizadores com cartões válidos devem poder entrar (exemplificar com alguns casos). Sempre que algum cartão inválido seja lido, deve ser ligada uma sirene.
12.	Criar uma rede externa, que simula o acesso à Internet, interligando com o router da empresa. Devem ser criados dois websites: portal.pt e google.pt (que deverão existir nos servidores de DNS). Deve ser configurada a interligação dessa rede com o router da empresa através de uma rede de 30 bits.

**Notas:**
- Colocar alguns computadores pessoais a título de exemplo em cada piso. Não é, obviamente, necessário todos os computadores pessoais.
- Quaisquer informações ausentes podem ser resolvidas pelos alunos, justificando as suas escolhas na apresentação a realizar.
- Todos os equipamentos devem fazer ping a todos os outros (não são implementados mecanismos de segurança que, em produção, deveriam ser considerados).
- A configuração de todos os equipamentos deve ser efetuada em dual stack (Ipv4 e IPv6).

**Datas:**
- Verificar data de entrega/apresentação no calendário da cadeira.

**Entregáveis:**
- Descrição da empresa;
- Ficheiro(s) packet tracer;
- Notas adicionais para a correta avaliação por parte do Docente.

**Deve entregar um unico ficheiro ZIP, na respetiva tarefa no Canvas, com a identificação do grupo e do trabalhoo: Gxx-TrabPacketTracerI.zip**
