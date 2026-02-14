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


#O que este Dashboard monitora?
Este dashboard oferece uma visão centralizada e em tempo real da saúde e performance de uma rede Wi-Fi corporativa. Ele foi desenhado para monitorar especificamente:

Switch Principal (nome do seu switch): Monitoramento individual de cada uma das 24 portas, mostrando o status operacional (ON/DOWN) de cada interface.
Access Points (APs): Acompanhamento detalhado de diversos pontos de acesso espalhados por setores como TI, RH, Administração entre outros.

#Principais Funcionalidades e Painéis:

Mapa Visual de Portas do Switch:

Utiliza um painel de Canvas com uma imagem de fundo customizada de um Switch de 24 portas.
Cada porta possui um indicador visual que muda de cor dinamicamente: se a porta estiver ativa, o status aparece como "ON"; se houver falha, ele destaca em vermelho como "DOWN".

#Saúde dos Access Points (Status em Tempo Real):

Disponibilidade (ICMP Ping): Monitora se o AP está online na rede.
Tempo de Atividade (Uptime): Mostra há quanto tempo o hardware está ligado sem interrupções.

Carga de Processamento: Monitora o Load Average dos APs (como no setor Almoxarifado) para identificar gargalos de performance.

Identificação por Setores:

O dashboard é organizado de forma que o administrador identifique instantaneamente qual setor está sofrendo com instabilidade (ex: AP-PLANEJAMENTO, AP-S.TREINAMENTO, AP-CCO).
