# Controle de Temperatura de Estufa de Secagem com CLP

Trabalho final da disciplina de **Controladores Lógicos Programáveis** — UFMS, 2025.

O projeto consiste em um sistema de controle de temperatura para uma estufa de secagem usada na cura de tinta em peças metálicas. Foi implementado em dois CLPs diferentes para poder comparar as plataformas.

## CLPs utilizados

- **Siemens LOGO! 12/24RCE** — programado em FBD (Diagrama de Blocos Funcionais) no LOGO!Soft Comfort
- **WEG TPW04-114BR-A** — programado em Ladder no TPW-PCLINK V1.12

## Como funciona

O sistema lê a temperatura da estufa e controla o aquecedor com lógica liga/desliga com histerese (115°C a 125°C, setpoint de 120°C). Quando a temperatura entra na faixa de cura, um timer de 30 min começa a contar. Depois da cura, liga o ventilador por 5 min para resfriar. Tem também alarme de sobretemperatura (150°C) e intertravamento de porta.

> Os tempos de cura e resfriamento estão reduzidos no programa (10s e 7s) para facilitar a demonstração em simulação.

## Arquivos

| Arquivo | Descrição |
|---------|-----------|
| `main.tex` | Relatório em LaTeX (abntex2) |
| `main.pdf` | Relatório compilado |
| `TRABALHO FINAL - JOSE VITOR CARDOZO AMARAL.lsc` | Projeto do LOGO!Soft Comfort |
| `estufa.tpc` | Projeto do TPW-PCLINK |
| `clp.pdf` | Diagrama FBD (LOGO!) |
| `IHM.png` | Tela da IHM do LOGO! |
| `tpw_ladder1.png` | Ladder parte 1 (Rungs 1–10) |
| `tpw_ladder2.png` | Ladder parte 2 (Rungs 11–16) |

## Softwares necessários

- [LOGO!Soft Comfort](https://www.siemens.com) — para abrir o arquivo `.lsc`
- [TPW-PCLINK V1.12](https://www.weg.net) — para abrir o arquivo `.tpc`
## Autor

**José Vítor Cardozo Amaral** — Engenharia Elétrica, UFMS

Professor: Valmir Machado Pereira
