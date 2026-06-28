# Simulação de Rede NForge

Uma simulação de infraestrutura de rede para a **NForge**, uma empresa especializada na produção de placas de vídeo e investigação de soluções de Inteligência Artificial. Este projeto foi desenvolvido utilizando **Cisco Packet Tracer** para a disciplina de "Redes e Comunicações de Dados".

[![License: MIT](https://img.shields.io/badge/License-MIT-3da639.svg)](LICENSE)
![Status](https://img.shields.io/badge/status-concluído-6f42c1)

[Portuguese](README.pt.md) | English

## Sobre

A NForge é uma empresa em crescimento com três edifícios principais: **Sede**, **Fábrica** e **Data Center**. O projeto simula toda a topologia de rede necessária para suportar as operações administrativas, de fabrico e de gestão de dados, incluindo integrações modernas de IoT.

A rede foi desenhada utilizando uma **Topologia em Árvore**, garantindo conectividade escalável e robusta entre todos os setores.

## Funcionalidades

- **Design de Rede Hierárquico**: Implementação de uma topologia em árvore interligando a Sede, Fábrica e Data Center.
- **Segmentação por VLAN**: Uso extensivo de Redes Locais Virtuais (VLANs) para separar departamentos e serviços (ex: Administração, RH, I&D, IoT, etc.).
- **Serviços Abrangentes**:
  - **DHCP & DNS**: Atribuição automática de IPs e resolução de nomes para IPv4 e IPv6.
  - **Serviços Web (HTTP)**: Portais internos da empresa.
  - **Serviços de Email**: Servidores de correio dedicados para vários departamentos.
- **Integração IoT**: Gestão inteligente de edifícios incluindo:
  - **Controlo de Temperatura**: Gestão automática de climatização (HVAC).
  - **Deteção de Incêndio/Gases**: Alarmes automáticos e ventilação (CO/CO2) baseados em limiares de sensores.
  - **Controlo de Acesso (RFID)**: Gestão segura de portas baseada em permissões de ID por edifício.
- **Implementação Dual-Stack**: Suporte completo para protocolos **IPv4** e **IPv6**.

## Arquitetura de Rede

### Edifícios
- **Sede**: 4 pisos abrangendo administração, engenharia, marketing, logística e RH.
- **Fábrica**: Abrange montagem, armazém, I&D e engenharia de hardware.
- **Data Center**: A espinha dorsal da empresa, alojando os serviços core (DHCP, DNS, HTTP, Mail e Registo de IoT).

### VLANs Principais
| VLAN ID | Propósito |
| --- | --- |
| **20** | Servidores (DHCP, DNS, Web, Mail, Registo IoT) |
| **30** | Dispositivos IoT |
| **40-46** | Setores administrativos (RH, Financeiro, Marketing, etc.) |
| **60-62** | Engenharia, I&D e Fábrica |

## Requisitos

| Ferramenta | Versão mínima |
| ---- | --------------- |
| Cisco Packet Tracer | 8.0+            |

## Como executar

1. Descarregue o ficheiro de simulação (se fornecido).
2. Abra o ficheiro no **Cisco Packet Tracer**.
3. Explore a topologia para observar a conectividade entre edifícios e a automação IoT.

## Licença

Distribuído sob a licença **MIT**, © 2024 Nycolas Souza.

É uma licença permissiva: qualquer pessoa pode usar, copiar, modificar e distribuir o código, inclusive em projetos comerciais, desde que mantenha o aviso de copyright e o texto da licença.

O texto completo está em [LICENSE](LICENSE).
