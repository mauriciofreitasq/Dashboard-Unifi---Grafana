# Dashboard-Unifi---Grafana
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
