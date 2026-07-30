## Configuração do Servidor Educacional

```mermaid
graph LR
A[Cliente]<--<b>Dados-->B[Servidor]
```
---
**Objetivos**:
- Experiência real de mercado
- Administração de Recusrsos
- Experiência de servidores Linux
---

### Servidor de Arquivos

Servidor educacional para arquivos, mas não dependendo da rede extrernar

```mermaid
graph TD
A[Servidor Senai \\10.87.36.10] --> B[Computador] --> R1[Mouse]
```
---
## Servidor de Desenvolvimento

Cada aluno, recebe o seu proprio acensso

Cada maquiana possui um ip deferente

```mermaid
graph LR
B[Ip da maquina 1263594] --> C[192.168.10.11]

```
|Recurso|Configuração|
|-------|------------|
|CPU|2 cores|
|RAM|521 MB|
|DISCO| 6 MB|
|SISTEMA OPERACIONAL| Ubuntu 26.04 LTS|
|ACESSO| SSH (Secure Shell)|


### Comandos no mobaXsterm

|Comando|Funcionalidade|
|---------------------------------------|----|
|password| Mudar senha 
|htop| 

### Dados de Acesso
|Campo|Valor|
|-----|------|
|Ip do conteiner|192.168.10.11|
|Usuario|Root|

## Banco de Dados

Dados: Isolados que não dizem muita coisa

- Ex: Platini, futebol, chuteira

Informação: Dados estruturados

- Ex: O Platini comprou uma chuteira para jogar futebol

Conhecimento: O que podemos extrair à partir das informações

- Ex: Ele precisa comprar uma chuteira para jogar bola

---
### O fluxo normal de um Banco de Dados é mostrado em diferentes situações:

```mermaid
graph LR
A[Dado: Chuteira] --> B[Processamento] --> C[Informação: O cliente precisa de uma chuteira]
```
```mermaid
graph LR
    A[Usuario] --> B[Aplicação] --> C[(Banco de Dados)]

```
---
> Por qual razão, as empresas não salvam os dados em arquivos?

```mermaid
graph TD

A[Guardar Dados] --> B[Banco de Dados]
A[Guardar Dados] --> C[Arquivos/Planilhas]
B-->B1[Varios usuarios ao mesmo tempo]
B-->B2[Backup e Sincronização]
B-->B3[Colsultas otimizadas/rapidas]
C-->C1[Um arquivo por vez]
C-->C2[Backup ineficiente]

```

## SPBD


Primeiro, começamos atualizando os pacotes:
```bash
sudo apt update && upgrade

