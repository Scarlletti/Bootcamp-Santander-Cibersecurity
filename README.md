# Simulação: Ataques de Força Bruta com Medusa — Relatório do Experimento

## Descrição do Experimento

Este repositório contém os prints (capturas de tela) produzidos durante um desafio prático de cibersegurança do bootcamp do Santander de Cibersegurança, sendo uma **simulação de ataques de força bruta** usando **Kali Linux** como máquina atacante e **Metasploitable / DVWA / serviços vulneráveis** como alvos em ambiente controlado (VirtualBox, rede host-only).

O objetivo é demonstrar os conceitos vistos no módulo: configuração do ambiente, execução de ataques (FTP, Web/DVWA, SMB), documentação dos comandos utilizados, resultados obtidos e recomendações de mitigação.

## Objetivos de Aprendizagem

- Compreender e executar ataques de força bruta em serviços como FTP, formulários web e SMB.
- Documentar processos técnicos de forma clara e reproduzível.
- Identificar vulnerabilidades e propor medidas de mitigação.

## Ambiente de Teste

- Host: Máquina física do aluno (VirtualBox).
- VMs:
  - **Kali Linux** (atacante)
  - **Metasploitable 2 / DVWA / serviços vulneráveis** (alvo)
- Rede: `Host-only` (rede interna isolada do host), sem acesso à Internet para as VMs (recomendado).
- Ferramentas usadas: `medusa` e `nmap`.

## Recomendações de Mitigação

- Desativar contas/serviços desnecessários (FTP antigo).
- Implementar políticas de senha fortes e bloqueio de conta após várias tentativas.
- Habilitar autenticação multifator (MFA) onde possível.
- Monitorar logs e configurar alertas para múltiplas tentativas de autenticação.
- Usar controles de rate-limiting e firewalls para limitar tentativas de força bruta.
