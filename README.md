# Velleman VTUSD3 — estudo técnico e proposta de reprodução com ESP32

**Trabalho 2 — 2026/2**  
**Produto selecionado:** Velleman VTUSD3, medidor ultrassônico de distância com apontador laser.  
**Situação:** esqueleto do relatório, a preencher.  
**Entrega indicada no enunciado:** 03/11/2026.

> Estrutura baseada no [enunciado em red/README.md](../red/README.md). Substituir os campos `[PREENCHER]` durante a pesquisa. Para características não identificadas, registrar as fontes consultadas; usar “não se aplica” somente com justificativa. Uma informação da ESP32 não descreve automaticamente o produto comercial.

## Identificação do grupo

| Integrante | Nome completo | Matrícula |
| --- | --- | --- |
| 1 | [PREENCHER] | [PREENCHER] |
| 2 | [PREENCHER] | [PREENCHER] |
| 3 | [PREENCHER] | [PREENCHER] |
| 4 | [PREENCHER] | [PREENCHER] |

## 1. Objetivos

[PREENCHER: objetivo do estudo do VTUSD3, análise de seu hardware/software e proposta de reprodução parcial com ESP32. Explicar o que o grupo pretende compreender e qual função será reproduzida.]

## 2. Seleção do sistema embarcado

[PREENCHER: justificar a escolha do produto comercial, seu enquadramento como sistema embarcado com sensores e atuadores, a disponibilidade de documentação e a viabilidade para o grupo.]

**Recorte previsto:** medição de distância por ultrassom sob comando de um botão, resultado em display e sinalização sonora. Detalhar e justificar na seção 3.3.

## 3. Estudo do produto e proposta

### 3.1 Descrição do produto selecionado

#### 3.1.1 Visão geral e funções principais

[PREENCHER: fabricante, modelo exato e funções, com referências junto às afirmações. Distinguir medição ultrassônica de apontamento laser. Fontes iniciais: [R1](#r1) e [R2](#r2).]

#### 3.1.2 Público-alvo, contexto de uso e segmento de mercado

[PREENCHER: quem utiliza, onde utiliza, aplicações e posição na categoria de instrumentos de medição. Citar fontes e distinguir aplicações documentadas de possibilidades propostas pelo grupo.]

#### 3.1.3 Fotos, ilustrações e diagramas do produto

[PREENCHER: inserir foto do VTUSD3 com legenda, autoria/origem e link. Acrescentar vista interna ou placa quando houver fonte verificável do modelo exato; se não encontrada, registrar essa limitação.]

| Figura prevista | Conteúdo | Fonte e identificação |
| --- | --- | --- |
| 1 | Vista externa do VTUSD3 | [PREENCHER] |
| 2 | Interface e elementos do produto | [PREENCHER] |
| 3, se disponível | Vista interna/placa | [PREENCHER] |

#### 3.1.4 Tecnologias de comunicação e controle embarcadas

[PREENCHER: como o produto adquire, processa e apresenta a medição. Informar interfaces documentadas; não presumir protocolos internos, conectividade ou sistema operacional.]

### 3.2 Análise técnica detalhada: listagem de características

Cada linha descreve **o VTUSD3 original**. Preencher informação, situação e fonte; incluir página/seção do manual quando possível. Se houver vários componentes ou interfaces, acrescentar linhas.

#### 3.2.1 Unidade de processamento

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 1.1 | Fabricante e modelo do MCU/MPU | [PREENCHER] | [PREENCHER] |
| 1.2 | Arquitetura e número de núcleos | [PREENCHER] | [PREENCHER] |
| 1.3 | Frequência de clock | [PREENCHER] | [PREENCHER] |
| 1.4 | Coprocessadores e unidades dedicadas | [PREENCHER] | [PREENCHER] |

#### 3.2.2 Memória

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 2.1 | RAM: tipo e capacidade | [PREENCHER] | [PREENCHER] |
| 2.2 | ROM/Flash: tipo, capacidade e localização interna/externa | [PREENCHER] | [PREENCHER] |
| 2.3 | EEPROM separada ou embutida | [PREENCHER] | [PREENCHER] |

#### 3.2.3 Sistema operacional

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 3.1 | GPOS, RTOS ou bare-metal | [PREENCHER] | [PREENCHER] |
| 3.2 | Versão/distribuição, quando identificável | [PREENCHER] | [PREENCHER] |

#### 3.2.4 Sensores e atuadores

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 4.1 | Sensores: variável, fabricante e modelo, quando identificáveis | [PREENCHER] | [PREENCHER] |
| 4.2 | Atuadores: função, fabricante e modelo, quando identificáveis | [PREENCHER] | [PREENCHER] |
| 4.3 | Conexão de cada sensor/atuador com o MCU/MPU | [PREENCHER] | [PREENCHER] |

#### 3.2.5 Interfaces de comunicação com fio

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 5.1 | Interfaces: I2C, SPI, UART, CAN, USB, Ethernet, RS-485 ou outras | [PREENCHER] | [PREENCHER] |

#### 3.2.6 Interfaces de comunicação sem fio

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 6.1 | Tecnologias e padrões sem fio | [PREENCHER] | [PREENCHER] |
| 6.2 | Chips/módulos de rádio e protocolos de aplicação | [PREENCHER] | [PREENCHER] |

#### 3.2.7 Unidades de entrada/saída (I/O)

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 7.1 | GPIO: funções de entrada e saída identificadas | [PREENCHER] | [PREENCHER] |
| 7.2 | ADC/DAC: presença, uso e resolução, quando identificáveis | [PREENCHER] | [PREENCHER] |
| 7.3 | PWM: presença e utilização | [PREENCHER] | [PREENCHER] |

#### 3.2.8 Fonte de energia e sistema de alimentação

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 8.1 | Fonte de energia, tensão e tipo de bateria/alimentação | [PREENCHER] | [PREENCHER] |
| 8.2 | Gerenciamento de energia, PMIC e regulação | [PREENCHER] | [PREENCHER] |
| 8.3 | Economia de energia, sleep e wake-up | [PREENCHER] | [PREENCHER] |
| 8.4 | Backup de energia | [PREENCHER] | [PREENCHER] |
| 8.5 | Reset e watchdog | [PREENCHER] | [PREENCHER] |
| 8.6 | Supervisão de energia e brown-out | [PREENCHER] | [PREENCHER] |

#### 3.2.9 Firmware e atualizações

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 9.1 | Firmware e funções documentadas | [PREENCHER] | [PREENCHER] |
| 9.2 | Atualizações remotas/OTA | [PREENCHER] | [PREENCHER] |

#### 3.2.10 Unidade de proteção e segurança

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 10.1 | Criptografia e aceleradores | [PREENCHER] | [PREENCHER] |
| 10.2 | HSM/Secure Element e armazenamento de credenciais | [PREENCHER] | [PREENCHER] |
| 10.3 | Secure boot e criptografia da Flash | [PREENCHER] | [PREENCHER] |
| 10.4 | Autenticação, controle de acesso, TLS/VPN e outras proteções | [PREENCHER] | [PREENCHER] |

#### 3.2.11 Armazenamento externo

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 11.1 | SD, NAND, eMMC, HDD/SSD ou outro armazenamento externo | [PREENCHER] | [PREENCHER] |

#### 3.2.12 Interface com o usuário (UI)

| Item do enunciado | Característica | Descrição no produto | Fonte |
| --- | --- | --- | --- |
| 12.1 | Displays e indicadores visuais | [PREENCHER] | [PREENCHER] |
| 12.2 | Botões e sensores de toque | [PREENCHER] | [PREENCHER] |
| 12.3 | Sinalização sonora e outras interfaces | [PREENCHER] | [PREENCHER] |

#### 3.2.13 Tecnologias críticas

| Tecnologia | Por que é necessária ao produto | Evidência/fonte |
| --- | --- | --- |
| [PREENCHER] | [PREENCHER] | [PREENCHER] |

[PREENCHER: explicar as tecnologias sem as quais o produto não seria viável, relacionando medição, processamento e apresentação. Distinguir funções essenciais de acessórios.]

### 3.3 Proposta de reprodução com ESP32

#### 3.3.1 Objetivo e funcionalidades reproduzidas

[PREENCHER: descrever a reprodução parcial e justificar sua adequação aos recursos e à experiência do grupo. Consultar o [plano de apoio](../TrenaUltrassonica/README.md), sem tratar funcionalidades planejadas como já implementadas.]

| Função do produto original | Reprodução proposta | Integral, simplificada ou não reproduzida | Justificativa |
| --- | --- | --- | --- |
| [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] |

#### 3.3.2 Componentes e recursos equivalentes

| Característica da seção 3.2 | Recurso da ESP32 ou módulo equivalente | Conexão/recurso utilizado | Fonte e situação |
| --- | --- | --- | --- |
| Processamento | [PREENCHER: modelo exato da ESP32] | [PREENCHER] | [PREENCHER] |
| Memória | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Sistema operacional | [PREENCHER: proposta com ESP-IDF/FreeRTOS] | [PREENCHER] | [PREENCHER] |
| Sensores e atuadores | [PREENCHER: sensor de ultrassom, display e buzzer reais] | [PREENCHER] | [PREENCHER] |
| Comunicação com fio | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Comunicação sem fio | [PREENCHER: justificar se não utilizada] | [PREENCHER] | [PREENCHER] |
| I/O | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Energia | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Firmware e atualização | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Segurança | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Armazenamento externo | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Interface com o usuário | [PREENCHER: botão e apresentação do resultado] | [PREENCHER] | [PREENCHER] |

**Disponibilidade:** a [lista da disciplina](../Lista_de_Sensores.md) contém “Sensor Ultrasom”, mas não especifica o modelo. Confirmar módulos, alimentação, níveis lógicos e componentes auxiliares antes de detalhar o circuito.

#### 3.3.3 Diagrama conceitual

[PREENCHER: inserir diagrama de blocos próprio, com ESP32, sensor, botão, display, buzzer, alimentação e interfaces. Explicar o fluxo e a diferença entre diagrama funcional e esquema elétrico.]

#### 3.3.4 Funcionamento e organização do software

[PREENCHER: sequência do botão até a apresentação da medida, cálculo com unidades, temporização, validação de eco, timeout e recuperação de falhas. Identificar ferramentas e drivers previstos para ESP-IDF.]

#### 3.3.5 Limitações e desafios esperados

| Limitação/desafio | Impacto na reprodução | Tratamento proposto |
| --- | --- | --- |
| [PREENCHER] | [PREENCHER] | [PREENCHER] |

[PREENCHER: indicar funcionalidades omitidas, diferença de alcance e precisão, dependência do alvo e condições ambientais. Não prometer características que não foram verificadas.]

#### 3.3.6 Plano de validação

| Verificação | Procedimento proposto | Resultado esperado/critério |
| --- | --- | --- |
| [PREENCHER] | [PREENCHER] | [PREENCHER] |

[PREENCHER: comparação com régua/fita métrica, medidas repetidas, falhas de eco e interface. Nesta entrega conceitual, não apresentar resultados de ensaios ainda não realizados.]

### 3.4 Pesquisa bibliográfica e tecnológica

Usar **oito artigos distintos de revistas científicas**: quatro sobre tecnologias e quatro sobre aplicação/uso. Cada entrada deve conter referência, link do PDF original, resumo próprio e relação com sistemas embarcados. Não enviar os PDFs ao repositório.

A [seleção inicial de apoio](../TrenaUltrassonica/ARTIGOS.md) inclui referências e pendências de acesso, idioma e adequação. Não foi identificada ali aplicação específica do VTUSD3; verificar a aceitação do recorte por categoria/tecnologia antes de consolidar as quatro aplicações.

#### 3.4.1 Artigos sobre tecnologias

##### T1 — [PREENCHER: título]

- **Referência completa:** [PREENCHER: autores, título, revista, volume, número, páginas/artigo e ano].
- **DOI e PDF original:** [PREENCHER: links].
- **Resumo:** [PREENCHER: problema, método e resultados após leitura].
- **Relação com o produto e sistemas embarcados:** [PREENCHER].

##### T2 — [PREENCHER: título]

- **Referência completa:** [PREENCHER].
- **DOI e PDF original:** [PREENCHER].
- **Resumo:** [PREENCHER].
- **Relação com o produto e sistemas embarcados:** [PREENCHER].

##### T3 — [PREENCHER: título]

- **Referência completa:** [PREENCHER].
- **DOI e PDF original:** [PREENCHER].
- **Resumo:** [PREENCHER].
- **Relação com o produto e sistemas embarcados:** [PREENCHER].

##### T4 — [PREENCHER: título]

- **Referência completa:** [PREENCHER].
- **DOI e PDF original:** [PREENCHER].
- **Resumo:** [PREENCHER].
- **Relação com o produto e sistemas embarcados:** [PREENCHER].

#### 3.4.2 Artigos sobre aplicação/uso

##### A1 — [PREENCHER: título]

- **Referência completa:** [PREENCHER].
- **DOI e PDF original:** [PREENCHER].
- **Resumo:** [PREENCHER].
- **Aplicação estudada e relação com o produto/sistemas embarcados:** [PREENCHER].

##### A2 — [PREENCHER: título]

- **Referência completa:** [PREENCHER].
- **DOI e PDF original:** [PREENCHER].
- **Resumo:** [PREENCHER].
- **Aplicação estudada e relação com o produto/sistemas embarcados:** [PREENCHER].

##### A3 — [PREENCHER: título]

- **Referência completa:** [PREENCHER].
- **DOI e PDF original:** [PREENCHER].
- **Resumo:** [PREENCHER].
- **Aplicação estudada e relação com o produto/sistemas embarcados:** [PREENCHER].

##### A4 — [PREENCHER: título]

- **Referência completa:** [PREENCHER].
- **DOI e PDF original:** [PREENCHER].
- **Resumo:** [PREENCHER].
- **Aplicação estudada e relação com o produto/sistemas embarcados:** [PREENCHER].

### 3.5 Comparativo com produtos similares

Selecionar pelo menos **cinco outros produtos comerciais** além do VTUSD3. Comparar os itens relevantes da seção 3.2, com fontes, unidades e condições de operação. Ampliar a tabela ou dividi-la por assunto para incluir características adicionais.

| Produto | Tecnologia de medição | Faixa e exatidão declaradas | Processamento/memória/SO | Interface e comunicação | Alimentação | Funções e limitações | Fontes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Velleman VTUSD3 | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Similar 1 — [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Similar 2 — [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Similar 3 — [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Similar 4 — [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] |
| Similar 5 — [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] | [PREENCHER] |

**Análise comparativa:** [PREENCHER: explicar diferenças e vantagens com base na tabela. Se incluir medidores a laser, explicitar a diferença em relação ao ultrassom. Não confundir resolução com exatidão.]

## 4. Referências bibliográficas

Listar aqui todas as fontes efetivamente utilizadas, inclusive as das imagens, características técnicas, artigos e similares. Os identificadores devem corresponder às citações no texto. Não inventar DOI para documentos que não tenham um identificador confirmado.

### R1

VELLEMAN. **VTUSD3: Ultrasonic Distance Meter + Laser**. Disponível em: https://www.velleman.eu/products/view/ultrasonic-distance-meter-laser-vtusd3/?id=372828&lang=en. Acesso em: [PREENCHER: data da consulta pelo grupo].

### R2

VELLEMAN. **VTUSD3 — User Manual**. Versão 03, 25 out. 2018. Disponível em: https://cdn.velleman.eu/downloads/1/vtusd3a6v03.pdf. Acesso em: [PREENCHER: data da consulta pelo grupo].

### Demais referências

[PREENCHER: referências completas das outras fontes técnicas, dos oito artigos, dos cinco similares e das imagens, com identificadores próprios e datas de acesso.]

## Checklist de revisão antes da entrega

- [ ] Preencher identificação dos quatro integrantes.
- [ ] Completar descrição, fotos e fontes do produto.
- [ ] Cobrir todos os subitens das 12 categorias técnicas.
- [ ] Justificar informações não identificadas ou não aplicáveis.
- [ ] Destacar tecnologias críticas.
- [ ] Completar proposta, equivalências ESP32, diagrama e limitações.
- [ ] Incluir quatro artigos tecnológicos e quatro de aplicação, com resumos e links de PDF.
- [ ] Comparar cinco outros produtos e citar suas fontes.
- [ ] Conferir referências completas e correspondência das citações.
- [ ] Remover campos `[PREENCHER]` e instruções editoriais após concluir as seções.
- [ ] Conferir renderização, imagens e links no GitLab.
- [ ] Manter o relatório principal como `VTUSD3/README.md` e submeter conforme a disciplina.
