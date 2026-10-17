# Observatório de Rede — Investigação de Incidente com PCAP

> *Incident investigation from packet captures: topology inference, asset inventory, timeline and CVE/KEV dossier.*

Investigação de um incidente de rede a partir de **capturas de tráfego (PCAP)** analisadas no **Wireshark**. O exercício parte do pacote cru e reconstrói o que aconteceu: quem são os ativos, como estão conectados e qual a linha do tempo do evento.

## 🎯 Objetivo

Praticar **análise forense de rede**: a partir de capturas, inferir a topologia, inventariar os ativos, montar a linha do tempo do incidente e correlacionar os serviços observados com vulnerabilidades conhecidas.

## 🧭 Metodologia

1. **Análise de PCAP (Wireshark):** inspeção de protocolos, conversas e fluxos; uso de filtros de exibição e estatísticas (Conversations, Protocol Hierarchy, Endpoints).
2. **Inferência de topologia:** a partir de ARP, broadcast e padrões de tráfego, deduzir a disposição da rede e os segmentos.
3. **Inventário de ativos:** identificação de hosts, serviços e sistemas pelo comportamento de rede e fingerprinting passivo.
4. **Linha do tempo:** ordenação cronológica dos eventos relevantes do incidente.
5. **Dossiê CVE/KEV:** correlação dos serviços/versões observados com CVEs conhecidas e checagem no catálogo **KEV da CISA**.

## 🛠️ Ferramentas

`Wireshark` · `tshark` · análise de protocolos (ARP, DNS, HTTP, SMB, MQTT) · `NVD` · `CISA KEV`

## 📊 Entregáveis

- Relatório da investigação (metodologia, achados e conclusões).
- Inventário de ativos inferido do tráfego.
- Linha do tempo do incidente.
- Correlação de vulnerabilidades (CVE/KEV).

## 📚 O que aprendi

- O pacote **não mente**: dá para reconstruir muita coisa sem acesso aos próprios hosts.
- Fingerprinting **passivo** e inferência de topologia só a partir do tráfego.
- Ligar o que se vê na rede a **vulnerabilidades reais** e ao risco de exploração ativa (KEV).

## 🔒 Nota de segurança

Material de **laboratório** focado em metodologia. Endereços e identificadores do ambiente foram **sanitizados**; nenhum dado sensível real é exposto.
