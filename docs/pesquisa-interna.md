# Pesquisa sobre os componentes internos do VTUSD3

**Responsável:** Integrante 2 — análise de processamento, memória, SO, firmware e segurança
**Data da pesquisa:** 31/10/2026 e 01/11/2026
**Objetivo:** levantar dados verificáveis para a seção 3.2 do relatório e registrar, com transparência, o que não pôde ser identificado.

## 1. Resumo

O Velleman VTUSD3 é um medidor ultrassônico de distância com apontador laser, documentado por manual de operação e páginas de distribuidores. A documentação pública descreve funções, interface, alimentação e especificações de medição, mas **não identifica o microcontrolador, a memória, o sistema operacional, a versão de firmware ou mecanismos de segurança**. Não foi localizado service manual, esquema elétrico, teardown do modelo exato, patente específica ou certificação que revele esses componentes.

Por isso, os itens de 3.2.1 a 3.2.3, 3.2.9 a 3.2.11 foram redigidos como **"não identificado"** ou **"não documentado"**, com a fonte consultada e a justificativa. A ausência de dado não foi convertida em afirmação de inexistência, e nenhum componente foi atribuído por analogia com outros medidores.

## 2. Fontes consultadas

| Fonte | O que foi verificado | Resultado |
| --- | --- | --- |
| Manual VTUSD3 v03 (25/10/2018), R2 | Descrição, uso, funções e especificações | Documenta ultrassom, laser, LCD, teclas, área/volume, 5 memórias, auto-desligamento, 9 V e <60 mA. Não informa MCU, memória, SO, firmware ou segurança. |
| Manual VTUSD3 v02 (05/08/2014), R7 | Lista de características | Repete as funções e acrescenta "alarm function for wrong readings"; não acrescenta dados de hardware. |
| Manual INDC003/HMUSD2 | Versão de revenda do mesmo produto | Conteúdo técnico equivalente; sem dados internos. |
| Página oficial Velleman (R1) | Especificações e downloads | Em 01/11/2026 redirecionou para aviso de indisponibilidade da loja; sem dados técnicos acessíveis. |
| Distribuidores (EIO, All Spectrum) | Especificações e descrição | Confirmam faixa, exatidão, laser, alimentação e funções; não abrem o produto. |
| FCC ID (https://fccid.io/) | Certificação de rádio | Nenhum registro do VTUSD3 localizado; o manual não documenta rádio, o que é coerente. A base não revela o MCU. |
| Busca de patentes | Patente do modelo | Nenhuma patente atribuída ao VTUSD3 que descrevesse a eletrônica foi localizada. |
| Buscas de teardown | Desmontagem do modelo exato | Consultas em inglês, português, espanhol, neerlandês, alemão e polonês não localizaram desmontagem pública do VTUSD3. |

**Consultas de teardown realizadas:** "VTUSD3 teardown", "VTUSD3 PCB", "VTUSD3 chip", "VTUSD3 desmontagem", "VTUSD3 desmontaje", "VTUSD3 reparatie", "VTUSD3 zerlegen", "VTUSD3 demontage", "VTUSD3 service manual", "VTUSD3 schematic".

## 3. Resultados por item

| Item | Situação | Evidência | O que não se pode afirmar |
| --- | --- | --- | --- |
| 1.1 MCU/MPU | Não identificado | O manual descreve funções que exigem um controlador, mas não o nomeia | Fabricante/modelo |
| 1.2 Arquitetura/núcleos | Não identificado | Sem datasheet ou teardown | ARM, AVR, RISC-V etc. |
| 1.3 Clock | Não identificado | Nenhuma fonte consultada informa | Frequência |
| 1.4 Coprocessadores | Não identificado | Sem evidência documental | DSP/FPU/IA |
| 2.1 RAM | Não identificado | O manual não informa | Tipo/capacidade |
| 2.2 ROM/Flash | Não identificado | Há firmware, mas o manual não detalha a memória | Tipo/capacidade/localização |
| 2.3 EEPROM | Não identificado | O manual cita 5 conjuntos de memória, não a tecnologia | EEPROM/Flash/retenção |
| 3.1 SO | Não identificado | Sem evidência de GPOS/RTOS; bare-metal é hipótese | "Roda Linux/FreeRTOS" |
| 3.2 Versão | Não identificado | Nenhuma versão divulgada | Versão/distribuição |
| 9.1 Firmware | Não identificado | Funções documentadas; versão não divulgada | Versão/arquitetura |
| 9.2 OTA | Não documentado | Sem porta, rádio ou procedimento descrito | "Não é atualizável" |
| 10.1 Criptografia | Não documentado | Sem evidência | AES/SHA/etc. |
| 10.2 HSM/SE | Não documentado | Sem evidência | Presença/ausência |
| 10.3 Secure boot | Não documentado | Sem evidência | Presença/ausência |
| 10.4 Outras | Não documentado | Acesso físico por teclas; sem autenticação/rede descrita | "Sem nenhuma proteção interna" |
| 11.1 Armazenamento externo | Não documentado | Sem slot ou mídia descrita; 5 memórias internas | SD/NAND/eMMC |

## 4. O que não se pode concluir

- **Não** se pode dizer que o VTUSD3 usa o mesmo MCU de outro medidor (CEM, Stanley, Bosch etc.) só porque a função é parecida.
- **Não** se pode transportar a arquitetura da ESP32 para o produto comercial; a ESP32 é a plataforma da reprodução.
- **Não** se pode afirmar que o produto não tem memória não volátil, segurança ou boot protegido; apenas que o fabricante não documenta.
- **Não** se pode usar "5 memórias" como capacidade de RAM/Flash/EEPROM; é a quantidade de resultados armazenáveis.
- **Não** se pode inventar versão de firmware ou sistema operacional para preencher tabela.

## 5. Plano de identificação futura (não executado)

Se o grupo obtiver uma unidade e autorização:

1. Abrir o aparelho sem danificar, documentando cada etapa.
2. Fotografar a placa em alta resolução (frente e verso).
3. Ler as marcações dos chips e comparar com datasheets.
4. Identificar barramentos e pads de depuração (SWD/JTAG/UART).
5. Se possível, ler a memória de programa e verificar a proteção de leitura.
6. Registrar modelo, memória, clock e firmware observados, com foto e fonte.

Nada disso foi feito neste Trabalho 2; o escopo é teórico.

## 6. Referências

- [R1](../README.md#r1) — página oficial Velleman (redirecionou em 01/11/2026).
- [R2](../README.md#r2) — manual VTUSD3 v03.
- [R7](../README.md#r7) — manual VTUSD3 v02 (lista de características).
- [P1–P5](../README.md#p1) — manuais/páginas dos similares, usados apenas para comparação funcional.
- FCC ID: https://fccid.io/ (consulta em 01/11/2026).
- Busca de patentes em bases públicas (consulta em 01/11/2026).
