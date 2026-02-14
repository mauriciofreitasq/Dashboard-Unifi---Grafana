# Dashboard-Unifi-Grafana
Desenvolvi este dashboard para centralizar a gestão dos ativos de rede de forma visual e intuitiva. A ideia foi transformar dados brutos em informações rápidas para tomada de decisão.

​Como funciona:
​Coleta: O Zabbix faz o trabalho pesado, coletando métricas via SNMP e verificando a disponibilidade dos ativos.

​Visualização: O Grafana consome esses dados para criar este painel dinâmico.

​O que estamos monitorando aqui?

​Status de Portas: Visão em tempo real das portas do Switch principal (Up/Down).

​Access Points: Monitoramento de disponibilidade (On/Off) segmentado por departamentos.

​Performance: Tráfego de dados (Mb/s) no Gateway e latência da rede (Ping).

​Uptime: Tempo de atividade dos equipamentos para controle de estabilidade.

​O resultado? Mais proatividade para identificar falhas antes mesmo que os usuários percebam! 


<img width="1918" height="1000" alt="image" src="https://github.com/user-attachments/assets/f7eeb409-0928-449d-8d78-c90e544d872c" />


# Monitoramento de Rede UniFi e Infraestrutura de TI
Painel de gestão operacional para Switches e Access Points.

---

## Descrição do Projeto
Este repositório contém o arquivo de configuração (JSON) de um dashboard desenvolvido no Grafana para o monitoramento centralizado de ativos de rede. O projeto integra dados coletados via Zabbix para fornecer visibilidade sobre a saúde dos dispositivos e o estado das interfaces físicas.

O diferencial deste dashboard é a implementação de um painel de Canvas que replica a disposição física de um switch de 24 portas, permitindo diagnósticos rápidos de conectividade.

---

## Funcionalidades Principais

* **Status das Portas (Switch):** Mapeamento visual das interfaces do Switch 01.
    * **ON:** Indica porta operacional.
    * **DOWN:** Indica porta desconectada ou com erro.
* **Monitoramento de Pontos de Acesso (APs):** Cobertura de diversos setores, incluindo TI, RH, Administração, Almoxarifado, Planejamento, Sala de Reunião e CCO.
* **Métricas de Performance:** * **Disponibilidade (ICMP):** Verificação constante de conexão.
    * **Tempo de Atividade (Uptime):** Monitoramento de reinicializações inesperadas.
    * **Carga de Processamento (Load):** Análise de consumo de CPU dos dispositivos de rede.

---

## Requisitos Técnicos

Para a correta importação e visualização dos dados, são necessários:
1.  **Grafana v11.0** ou superior (compatível com o recurso de Canvas).
2.  **Plugin Zabbix** (`alexanderzobnin-zabbix-datasource`) instalado.
3.  **Fonte de dados (Data Source):** Instância do Zabbix configurada com os nomes de hosts e grupos correspondentes (ex: Grupo "Acess Points").

---

## Instruções de Instalação

1.  Efetue o download do arquivo `Unifi Dash.json` presente neste repositório.
2.  No seu ambiente Grafana, acesse o menu **Dashboards** e selecione a opção **Import**.
3.  Carregue o arquivo JSON baixado.
4.  Associe o dashboard à sua **Data Source do Zabbix** quando solicitado pelo sistema.
5.  Ajuste os filtros de Host e Grupo caso a sua nomenclatura no Zabbix seja diferente da utilizada no projeto original.

---

Desenvolvido para fins de gestão de infraestrutura de rede.
