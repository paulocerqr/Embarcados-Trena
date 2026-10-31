# Velleman VTUSD3 — estudo técnico e proposta de reprodução com ESP32

**Trabalho 2 — 2026/2**  
**Produto selecionado:** Velleman VTUSD3, medidor ultrassônico de distância com apontador laser.  
**Situação:** relatório em elaboração; proposta de reprodução preenchida, demais seções a completar.  
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

A proposta consiste em reproduzir parcialmente a função de medição de distância do Velleman VTUSD3 com uma placa ESP32, um sensor de ultrassom, um botão, um display OLED I2C e um buzzer ativo. Ao pressionar o botão, o usuário solicitará uma leitura; o sistema calculará a distância, mostrará o resultado em centímetros e emitirá uma confirmação sonora curta. Se a tentativa falhar, apresentará uma mensagem de erro e permitirá uma nova medição.

A operação por tecla e a apresentação local de medidas tomam como referência o manual do produto [R2](#r2). A seleção de componentes, os parâmetros de software e os critérios de teste a seguir são decisões de projeto do grupo, não especificações internas do VTUSD3. Trata-se de uma proposta conceitual para o Trabalho 2: a montagem, o firmware e os ensaios ainda não foram executados.

O recorte foi escolhido para uma equipe de quatro estudantes com pouca experiência em eletrônica. A montagem em protoboard utiliza um sensor principal e interfaces locais, sem mecânica ou circuitos de potência. O buzzer fornece atuação sonora, e o display apresenta o resultado. A reprodução não exige comprar ou desmontar o produto comercial.

| Função do produto original | Reprodução proposta | Integral, simplificada ou não reproduzida | Justificativa |
| --- | --- | --- | --- |
| Medição de distância por ultrassom | Sensor do laboratório e processamento na ESP32 | Simplificada | Preservar a função principal sem prometer alcance ou exatidão equivalentes |
| Solicitação pela tecla READ | Um botão físico | Simplificada | Um toque produz uma tentativa de medição |
| Apresentação em LCD | Distância e mensagens em OLED I2C | Simplificada | Aproveitar um display da lista da disciplina |
| Indicação de leitura incorreta | Mensagem de erro e aviso pelo buzzer | Simplificada | Tornar explícitas as tentativas inválidas; padrões sonoros definidos pelo grupo |
| Unidades e referências de medição selecionáveis | Centímetros, a partir da face dos transdutores | Simplificada | Usar uma unidade e uma referência física únicas |
| Apontador laser | Não previsto | Não reproduzida | Não é necessário à emissão e recepção do ultrassom |
| Cálculo de área/volume e armazenamento de medidas | Apenas último resultado em RAM | Não reproduzidas as funções adicionais | Concentrar o trabalho no caminho sensor → processamento → interface |

O resultado deverá permanecer identificado como **última leitura** até a próxima solicitação. Durante uma nova tentativa, a tela mostrará “Medindo”; em caso de falha, substituirá o valor por uma mensagem, sem reapresentar a medida antiga como resultado atual.

#### 3.3.2 Componentes e recursos equivalentes

| Característica da seção 3.2 | Recurso da ESP32 ou módulo equivalente | Conexão/recurso utilizado | Fonte e situação |
| --- | --- | --- | --- |
| Processamento | Placa ESP32 fornecida pelo professor | Executar controle, cálculo e interface | Modelo, arquitetura, clock e número de núcleos dependem da placa a confirmar |
| Memória | RAM para estado, tempo de eco e resultado; Flash para firmware | Sem histórico persistente ou EEPROM adicional | Capacidades dependem da placa; uso definido nesta proposta |
| Sistema operacional | ESP-IDF com FreeRTOS | Uma tarefa de aplicação coordena o ciclo de medição | FreeRTOS integra o ESP-IDF [R4](#r4); versão será registrada na implementação |
| Sensores e atuadores | Sensor de ultrassom, OLED I2C e buzzer ativo | Sensor adquire a distância; display e buzzer apresentam o resultado | Módulos constam na lista da disciplina; modelo do sensor ainda não confirmado |
| Comunicação com fio | Interface de comando/eco, se compatível com o sensor; I2C no display | GPIO/temporização e linhas SDA/SCL; serial para diagnóstico | HC-SR04 como referência condicional [R3](#r3); I2C [R5](#r5) |
| Comunicação sem fio | Não utilizada | Controle e apresentação locais | Não depende de rede, conta ou servidor; capacidade de rádio não implica uso |
| I/O | Entradas para botão e eco; saídas para comando e buzzer | Captura temporizada; RMT como opção para o eco na placa compatível | RMT registra níveis e durações de pulsos [R6](#r6); ADC/DAC não necessários ao fluxo proposto |
| Energia | USB da placa e alimentação adequada a cada módulo | GND comum; adequação dos níveis de sinal | Confirmar regulador, corrente disponível e requisitos dos módulos antes da montagem |
| Firmware e atualização | Programa em C com ESP-IDF | Gravação por cabo; sem OTA | Escolha de projeto; fixar versão do ambiente e dos drivers |
| Segurança | Operação local, sem credenciais ou serviços de rede | Tratar leituras inválidas, falhas e tempo máximo de espera | Não afirmar habilitação de secure boot ou criptografia sem configuração e verificação |
| Armazenamento externo | Não previsto | Nenhum cartão SD ou memória externa adicional | O histórico não faz parte da reprodução |
| Interface com o usuário | Botão, OLED e buzzer ativo | Comando único, leitura em centímetros e avisos de sucesso/erro | Controlador do OLED, endereço I2C e acionamento do buzzer dependem dos módulos reais |

**Disponibilidade:** a [lista da disciplina](../Lista_de_Sensores.md) contém “Sensor Ultrasom”, mas não especifica o modelo. Confirmar módulos, alimentação, níveis lógicos e componentes auxiliares antes de detalhar o circuito.

Serão necessários uma placa, uma protoboard, um sensor, um botão, um display, um buzzer, cabo USB de dados, jumpers e resistores conforme a ligação. Para os ensaios, utilizar régua ou fita métrica e um alvo plano fixo. Nenhum número de GPIO será definido antes da identificação da placa e de seus pinos reservados.

Como referência de viabilidade, o HC-SR04 documentado em [R3](#r3) usa alimentação de 5 V e sinais de comando/eco. Se esse modelo for disponibilizado, adequar a saída ECHO ao nível admitido pela entrada da ESP32; não ligar um sinal de 5 V diretamente a um GPIO de 3,3 V. Verificar também os resistores de pull-up do OLED e o nível das linhas I2C. O buzzer deverá ter acionamento compatível com a corrente da saída, usando driver quando necessário. O esquema elétrico definitivo depende dessas confirmações.

#### 3.3.3 Diagrama conceitual

```mermaid
flowchart LR
    USB["Alimentação USB"] --> PLACA["Placa ESP32 e alimentação dos módulos"]
    BTN["Botão de medição"] -->|Entrada GPIO| ESP["ESP32: aquisição, validação e cálculo"]
    PLACA --> ESP
    PLACA --> US["Sensor de ultrassom"]
    ESP -->|Comando de emissão| US
    US -->|Eco| NIVEL["Adequação de nível, quando necessária"]
    NIVEL -->|Captura temporizada| ESP
    ESP -->|I2C| OLED["OLED: distância ou erro"]
    ESP -->|Acionamento compatível| BZ["Buzzer ativo"]
    ESP -->|Diagnóstico serial| PC["Computador de desenvolvimento"]
```

**Figura — Diagrama funcional da reprodução, elaborado pelo grupo.** A emissão sonora atinge o alvo e o retorno é convertido em uma medida pela ESP32. Display e buzzer apresentam o resultado ao usuário. O computador serve ao desenvolvimento e ao diagnóstico, sem participar do cálculo durante a operação normal.

O desenho não representa pinagem, polaridades ou todas as ligações de alimentação. Display e buzzer também receberão alimentação apropriada e os circuitos compartilharão GND. A distribuição de energia e os eventuais divisores ou drivers serão detalhados no esquema elétrico após identificar os módulos.

#### 3.3.4 Funcionamento e organização do software

O firmware será desenvolvido em C no ESP-IDF, utilizando FreeRTOS [R4](#r4). Uma tarefa de aplicação tratará o botão, solicitará a aquisição e atualizará a interface. A temporização do eco ficará a cargo do driver do sensor e de recurso compatível da placa, como o RMT, que registra a duração de níveis digitais [R6](#r6). Não será utilizada uma espera de tarefa para contar microssegundos. O driver I2C do ESP-IDF será combinado com um driver do controlador real do OLED [R5](#r5).

O fluxo será o seguinte:

```mermaid
flowchart TD
    INICIO["Ligar: manter buzzer desligado e invalidar resultado"] --> INIT["Inicializar GPIO, captura e display"]
    INIT --> OK{"Inicialização concluída?"}
    OK -->|Não| FATAL["Indicar falha pelo recurso disponível e registrar diagnóstico"]
    OK -->|Sim| ESPERA["Aguardar novo toque com botão liberado"]
    ESPERA --> TOQUE["Confirmar pressionamento estável e mostrar Medindo"]
    TOQUE --> CAP["Respeitar intervalo mínimo, preparar captura e disparar sensor"]
    CAP --> ECO{"Pulso completo dentro do timeout?"}
    ECO -->|Não| ERRO["Invalidar leitura, mostrar erro e emitir dois avisos curtos"]
    ECO -->|Sim| CALC["Converter tempo para distância e verificar faixa"]
    CALC --> VALIDO{"Resultado válido?"}
    VALIDO -->|Não| ERRO
    VALIDO -->|Sim| RESULTADO["Mostrar última leitura em cm e emitir um aviso curto"]
    ERRO --> LIBERA["Aguardar liberação estável do botão"]
    RESULTADO --> LIBERA
    LIBERA --> ESPERA
```

**Figura — Fluxo proposto do software, elaborado pelo grupo.** Novos comandos durante a aquisição serão ignorados. Um botão mantido pressionado não iniciará outras medições; será necessária a liberação estável antes de reconhecer outro toque. O tratamento de repiques do contato, chamado *debounce*, evita transformar um toque em vários comandos.

**Cálculo.** Para o eco de ida e volta, usar `distancia_m = velocidade_som_m_s × tempo_eco_s / 2`. A implementação converterá microssegundos em segundos explicitamente. Como hipótese inicial de bancada, adotar 340 m/s, valor usado no exemplo do datasheet [R3](#r3). Assim, 1.000 µs correspondem a 0,17 m, ou 17 cm. Essa escolha não representa compensação ambiental nem comprova exatidão do instrumento.

**Parâmetros propostos.** Os valores abaixo são escolhas iniciais para o cenário HC-SR04, não parâmetros já testados nem especificações do VTUSD3. Devem ser revistos se o módulo fornecido for diferente.

| Parâmetro | Valor inicial proposto | Finalidade |
| --- | --- | --- |
| Estabilidade do botão | 30 ms no pressionamento e na liberação | Filtrar repiques sem repetição por botão mantido |
| Comando TRIG | Pulso alto de 10 µs | Atender ao mínimo documentado para o HC-SR04 [R3](#r3) |
| Intervalo entre disparos | Pelo menos 100 ms | Superar o intervalo recomendado de mais de 60 ms do datasheet [R3](#r3) |
| Timeout de aquisição | Até 30 ms a partir do disparo | Limitar a espera tanto pela subida quanto pela descida do eco |
| Resolução temporal desejada | 1 µs | Converter o pulso com unidade conhecida; não equivale à resolução real de distância |
| Faixa nominal de referência | 2 a 400 cm, se confirmado o HC-SR04 | Rejeitar valores fora dos limites documentados [R3](#r3) |
| Faixa inicial de avaliação | 20, 50 e 100 cm | Concentrar a validação em distâncias reproduzíveis em bancada |
| Aviso de sucesso | Um pulso de 100 ms no buzzer | Confirmar a leitura |
| Aviso de erro | Dois pulsos de 100 ms, separados por 100 ms | Diferenciar falha e sucesso sem som contínuo |

Será necessário garantir que a captura cubra a janela escolhida e seja preparada antes da emissão, sem perder o início do eco. Resultado abaixo/acima da faixa, ausência de pulso, ECHO preso em nível alto ou aquisição incompleta produzirão erro. O timeout não será convertido em distância. O display mostrará centímetros inteiros, sem confundir a resolução de apresentação com a exatidão da medida.

Falhas do display ou de inicialização serão registradas pelo diagnóstico serial; o dispositivo não anunciará operação normal se a interface não estiver disponível. Todas as esperas de periféricos terão tempo limite, o buzzer será desligado ao concluir cada aviso e uma falha de medição retornará à espera de um novo toque. O driver do sensor deverá retornar um estado de sucesso/erro separado do valor numérico.

#### 3.3.5 Limitações e desafios esperados

| Limitação/desafio | Impacto na reprodução | Tratamento proposto |
| --- | --- | --- |
| Modelo dos módulos ainda desconhecido | Pinagem, alimentação e drivers não podem ser fechados | Identificar placa, sensor, controlador do OLED e buzzer antes da montagem |
| Alcance e exatidão diferentes do produto comercial | Uma reprodução funcional não demonstra desempenho equivalente | Publicar somente a faixa ensaiada e os erros observados |
| Alvo inclinado, pequeno, irregular ou absorvente | O retorno pode ser fraco, desviado ou corresponder a outra superfície | Usar alvo plano fixo no ensaio básico e registrar ensaios de limitações |
| Temperatura e condições ambientais | A velocidade do som adotada pode diferir da real | Registrar condições e declarar uso de velocidade fixa, sem compensação automática |
| Reflexões e outros emissores ultrassônicos | Um eco aceito pode não pertencer ao alvo desejado | Ensaiar um sensor por vez e declarar ausência de identificação/codificação de ecos |
| Adaptação elétrica e acionamento das saídas | Tensão ou corrente inadequadas podem danificar os componentes | Revisar esquema, níveis e alimentação; usar adaptação/driver conforme os módulos |
| Laser e referências frontal/traseira | Não há auxílio óptico nem compensação pelo comprimento de um gabinete | Adotar e registrar uma referência na face dos transdutores |
| Área, volume, memória e conversão de unidades | Essas funções do produto não serão reproduzidas | Restringir a implementação a distância em centímetros e última leitura em RAM |
| Alimentação USB e montagem aberta | Sem autonomia, gabinete ou proteção de produto comercial | Limitar a demonstração à bancada e não alegar certificação ou robustez equivalente |
| Disponibilidade do hardware | Resultados físicos podem não existir na entrega teórica | Apresentar procedimento e critérios de teste, sem inventar medições |

O tratamento de timeout detecta falhas de aquisição, mas não identifica todo eco incorreto. Uma leitura numericamente dentro da faixa ainda pode conter erro. Filtros, sensores ambientais e técnicas de codificação não fazem parte desta reprodução; sua necessidade será discutida a partir dos resultados. O instrumento será didático, sem uso previsto para decisões clínicas, periciais ou outras que dependam de exatidão certificada.

#### 3.3.6 Plano de validação

| Verificação | Procedimento proposto | Resultado esperado/critério |
| --- | --- | --- |
| Conversão matemática | Fornecer tempos sintéticos de 1.000 e 2.000 µs com 340 m/s | Obter 17 e 34 cm antes do arredondamento de apresentação |
| Validação de entrada | Simular timeout, pulso ausente/incompleto, duração zero e valor fora da faixa | Retornar erro separado do resultado numérico |
| Limites da faixa | Simular valores nos limites e imediatamente fora deles | Aceitar os limites definidos e rejeitar os valores externos |
| Botão | Simular repiques e manter pressionado por 2 s | Gerar uma tentativa; nova tentativa somente após liberação estável e novo toque |
| Inicialização | Ligar/reiniciar sem leitura anterior | Mostrar “Pronto” somente após inicialização; buzzer desligado e nenhuma distância fictícia |
| Medição em bancada | Realizar dez tentativas em cada posição de 20, 50 e 100 cm | Registrar todas as tentativas, inclusive falhas, e comparar com a referência |
| Sensor ausente ou eco travado | Simular o sinal no software; em bancada, alterar ligações somente com alimentação desligada | Aquisição encerra no timeout configurado, apresenta erro e não mantém valor antigo como atual |
| Recuperação | Após falha, disponibilizar novamente um alvo válido e pressionar o botão | Medir novamente sem reiniciar o firmware |
| Display e buzzer | Executar sucesso, erro e falha de inicialização/comunicação | Unidade e mensagens coerentes, avisos distintos e diagnóstico quando a tela falhar |
| Influência do alvo | Repetir observações com alvo inclinado ou material diferente | Documentar alteração e falhas sem excluir resultados inconvenientes |

**Montagem do ensaio.** Fixar o sensor e um alvo plano de dimensões adequadas ao módulo. Medir com régua ou fita a separação entre a referência dos transdutores e o plano do alvo, mantendo alinhamento e registrando material, dimensão do alvo e condições ambientais disponíveis. Respeitar o intervalo entre disparos. A ficha conterá referência, número da tentativa, leitura ou erro, e observações; serão 30 tentativas no ensaio básico.

**Análise.** Para cada posição, informar quantas das dez tentativas foram válidas, média, mínimo e máximo das leituras válidas, erro médio com sinal (`media_cm − referencia_cm`) e erro absoluto da média. Não substituir falhas por zero e não calcular média quando não houver leitura válida. A comparação com régua é uma verificação didática, não uma calibração rastreável.

**Critério proposto para o primeiro protótipo.** Em cada uma das três posições, buscar pelo menos nove leituras válidas em dez e erro absoluto da média de até 2 cm. Esses limites são metas do grupo para a bancada, não desempenho medido nem especificação garantida pelo fabricante. Se não forem alcançados, registrar o insucesso e investigar alinhamento, captura, alimentação e condições do alvo; qualquer revisão da meta deverá ser justificada e declarada antes de um novo ensaio.

As verificações matemáticas e de estados serão automatizadas quando o firmware existir. Testes físicos serão executados após revisão das ligações. Nesta etapa, nenhum dos testes foi realizado e não há resultados experimentais a apresentar.

### 3.4 Pesquisa bibliográfica e tecnológica

Esta seção organiza **oito artigos distintos de revistas científicas**: quatro sobre tecnologias e quatro sobre uso de instrumentos de medição de distância. As referências completas e a situação de acesso estão no [arquivo bibliográfico de apoio](../TrenaUltrassonica/ARTIGOS.md). Nenhum PDF foi enviado ao repositório.

**Situação da redação:** os resumos são preliminares, baseados no conteúdo acessível; não representam leitura integral dos oito artigos. As aplicações demonstram uso de instrumentos da categoria, não do VTUSD3 especificamente. A3 usa laser, enquanto o VTUSD3 mede por ultrassom. Resolver acessos, registrar consultas em bases acadêmicas e confirmar esse recorte antes de consolidar a entrega. A2 e A3 ainda não tiveram seus PDFs obtidos.

#### 3.4.1 Artigos sobre tecnologias

##### T1 — Fundamentos da medição ultrassônica

- **Referência:** Qiu, Lu e Qiu, *Micromachines*, 13(4), 520, 2022. [Referência completa](../TrenaUltrassonica/ARTIGOS.md#t1).
- **DOI e PDF:** [10.3390/mi13040520](https://doi.org/10.3390/mi13040520) · [PDF publicado](https://researchonline.ljmu.ac.uk/id/eprint/18696/1/Review%20of%20Ultrasonic%20Ranging%20Methods%20and%20Their%20Current%20Challenges.pdf).
- **Resumo e relação:** a revisão explica transdutores, detecção do eco e erros de medição. Fundamenta aquisição e cálculo embarcado da distância, sem comprovar os componentes internos do VTUSD3.

##### T2 — Influência das condições ambientais

- **Referência:** Rudyk et al., *Electronics*, 14(7), 1393, 2025. [Referência completa](../TrenaUltrassonica/ARTIGOS.md#t2).
- **DOI e PDF:** [10.3390/electronics14071393](https://doi.org/10.3390/electronics14071393) · [PDF oficial](https://www.mdpi.com/2079-9292/14/7/1393/pdf).
- **Resumo e relação:** o estudo avalia efeitos ambientais na medição ultrassônica. Apoia a discussão da velocidade do som adotada no firmware e das condições dos ensaios. Leitura integral pendente por limitação de acesso automatizado.

##### T3 — Processamento de ecos e interferência

- **Referência:** Shin, Kim e Choi, *IEEE Transactions on Instrumentation and Measurement*, 68(4), 972–979, 2019. [Referência completa](../TrenaUltrassonica/ARTIGOS.md#t3).
- **DOI e PDF:** [10.1109/TIM.2018.2863999](https://doi.org/10.1109/TIM.2018.2863999) · [PDF dos autores](https://acl.kaist.ac.kr/wp-content/uploads/2021/10/2018_TIM_SSI.pdf).
- **Resumo e relação:** apresenta processamento e codificação para rejeitar interferência ultrassônica. Relaciona confiabilidade e custo computacional; não há evidência de adoção dessa técnica no VTUSD3, nem previsão de implementá-la na reprodução. Abertura integral do PDF pendente.

##### T4 — Integração entre sensor, temporizador e display

- **Referência:** Titlee e Bhuyan, *SEU Journal of Science and Engineering*, 10(2), 6–11, 2016. [Referência completa](../TrenaUltrassonica/ARTIGOS.md#t4).
- **PDF original:** [artigo no domínio da universidade](https://old.seu.edu.bd/seujse/downloads/vol_10_no_2_dec_2016/02_Vol10No2Dec2016.pdf). DOI não identificado.
- **Resumo e relação:** desenvolve um instrumento com PIC, HC-SR04 e LCD. A temporização do retorno viabiliza cálculo e apresentação da distância. É referência de arquitetura de medição, não evidência do controlador do produto comercial.

#### 3.4.2 Artigos sobre aplicação/uso

##### A1 — Registro de distâncias em investigação de cenas

- **Referência:** Sungkangwan e Praihirunkit, *The Journal of KMUTNB*, 32(1), 177–188, 2022. [Referência completa](../TrenaUltrassonica/ARTIGOS.md#a1).
- **DOI e PDF:** [10.14416/j.kmutnb.2021.05.039](https://doi.org/10.14416/j.kmutnb.2021.05.039) · [download da revista](https://ph01.tci-thaijo.org/index.php/kmutnb-journal/article/download/247198/167963).
- **Resumo e aplicação:** utiliza medição ultrassônica e aplicativo para documentar distâncias de uma cena simulada. Demonstra finalidade concreta da saída de um instrumento embarcado; nosso protótipo não inclui aplicativo. Texto em tailandês, com resumo em inglês; leitura integral pendente.

##### A2 — Levantamento de cômodos

- **Referência:** Kashimoto, Arakawa e Yasumoto, *International Journal of Ad Hoc and Ubiquitous Computing*, 31(3), 189–199, 2019. [Referência completa](../TrenaUltrassonica/ARTIGOS.md#a2).
- **DOI e rota de PDF:** [10.1504/IJAHUC.2019.100779](https://doi.org/10.1504/IJAHUC.2019.100779) · [editora, acesso não confirmado](https://www.inderscienceonline.com/doi/pdf/10.1504/IJAHUC.2019.100779).
- **Resumo e aplicação:** combina distâncias ultrassônicas às paredes com sensores inerciais para obter dimensões e forma de cômodos. Demonstra o uso das leituras em levantamento espacial. Texto integral não obtido; a reprodução não terá geração automática de plantas.

##### A3 — Dimensionamento de fachadas

- **Referência:** Ordóñez et al., *Automation in Construction*, 19(6), 742–749, 2010. [Referência completa](../TrenaUltrassonica/ARTIGOS.md#a3).
- **DOI e rota de PDF:** [10.1016/j.autcon.2010.03.002](https://doi.org/10.1016/j.autcon.2010.03.002) · [editora, pode exigir acesso institucional](https://www.sciencedirect.com/science/article/pii/S0926580510000464/pdfft).
- **Resumo e aplicação:** usa câmera e Leica Disto Plus para dimensionar fachadas e aberturas. O medidor fornece distância ao processamento geométrico. A tecnologia é laser, diferente do VTUSD3; o caso sustenta uso da categoria funcional, sem equivalência de desempenho. Leitura integral pendente.

##### A4 — Levantamento da área de estabelecimentos

- **Referência:** Yu et al., *International Journal of Environmental Research and Public Health*, 12(11), 14034–14042, 2015. [Referência e identificação do uso na seção 2.1](../TrenaUltrassonica/ARTIGOS.md#a4).
- **DOI e PDF:** [10.3390/ijerph121114034](https://doi.org/10.3390/ijerph121114034) · [PDF oficial](https://www.mdpi.com/1660-4601/12/11/14034/pdf).
- **Resumo e aplicação:** emprega medidor ultrassônico comercial da Zircon no levantamento de área interna dos locais de um estudo ambiental. A trena fornece dados dimensionais, não mede partículas. O exemplo demonstra utilização de um instrumento da categoria sem descrever sua eletrônica; leitura integral pendente.

### 3.5 Comparativo com produtos similares

Foram selecionados **cinco outros medidores comerciais**: Velleman VTUSD2, Stanley IntelliMeasure 0-77-018, CEM DM-01, Bosch GLM 40 e Extech DT100M. O enunciado admite produtos de gerações distintas; esta comparação documental não pressupõe disponibilidade atual para compra.

Os três primeiros medem por ultrassom, assim como o VTUSD3. Bosch e Extech utilizam laser para a própria medição, permitindo contrastar tecnologias na mesma categoria funcional. Um apontador laser em um medidor ultrassônico não transforma sua medição em óptica.

#### 3.5.1 Tecnologia e desempenho declarado

As especificações abaixo são dos fabricantes, não resultados obtidos pelo grupo. Foram preservados os termos percentuais e adicionais das fontes, sem reduzir expressões diferentes a um único número de erro.

| Produto | Tecnologia de medição | Faixa declarada | Exatidão/precisão declarada na fonte | Fonte |
| --- | --- | --- | --- | --- |
| **VTUSD3 — produto estudado** | Ultrassom; laser como apontador | 0,50–16 m | ±1% + 1 dígito | [R2](#r2), seção 8 |
| **Velleman VTUSD2** | Ultrassom; laser como apontador | 0,91–18,288 m | 0,5% (±1 dígito), conforme a notação do manual | [P1](#p1), seção 13 |
| **Stanley IntelliMeasure 0-77-018** | Ultrassom | 0,60–12 m | ±0,5% da leitura, com percurso sem obstruções | [P2](#p2) |
| **CEM DM-01** | Ultrassom; laser como apontador | 0,50–16 m | ±1% + 1 da leitura; termo adicional não explicado na ficha | [P3](#p3) |
| **Bosch GLM 40 — código 0 601 072 900** | Laser | 0,15–40 m | ±1,5 mm, valor típico | [P4](#p4) |
| **Extech DT100M** | Laser | 0,05–100 m | ±2 mm, exatidão básica | [P5](#p5) |

**Condições.** O VTUSD3 informa operação de 0 a 40 °C e 45–91% de umidade relativa, com restrições de superfície e alinhamento. O VTUSD2 indica 0 a 43 °C; o Stanley, 10 a 49 °C e uso interno. O CEM associa a exatidão a 25 ±5 °C e 45–90% de umidade relativa. Os valores típicos/básicos dos modelos a laser não representam erro máximo garantido em qualquer ambiente; verificar as condições no manual da variante antes de ensaios comparativos. [R2](#r2), [P1](#p1), [P2](#p2), [P3](#p3), [P4](#p4), [P5](#p5).

O termo adicional da ficha CEM é ambíguo e não foi interpretado como um dígito ou convertido em centímetros. Dígitos de uma expressão de erro não são bits de processamento. Resolução de apresentação e exatidão são características diferentes.

#### 3.5.2 Interface, funções, memória de resultados e alimentação

| Produto | Interface e funções documentadas | Memória de resultados | Alimentação | Fonte |
| --- | --- | --- | --- | --- |
| **VTUSD3** | LCD e teclas; área, volume, soma e referência frontal/traseira | Cinco conjuntos | Uma bateria de 9 V | [R2](#r2), seções 4–6 e 8 |
| **VTUSD2** | LCD iluminável e teclas; área, volume, soma/subtração e unidades | Três posições M1–M3; apagadas ao desligar | Uma bateria alcalina de 9 V | [P1](#p1), seções 5 e 8–13 |
| **Stanley 0-77-018** | LCD e teclas; área, volume, soma e conversão de unidades | Exibe as três últimas medidas; persistência não comprovada | Uma bateria de 9 V | [P2](#p2) |
| **CEM DM-01** | LCD iluminado, teclas e avisos sonoros; área, volume, soma e referência frontal/traseira | Cinco grupos; retenção após desligamento declarada | Uma bateria de 9 V | [P3](#p3) |
| **Bosch GLM 40** | Display iluminado; distância, área, volume e altura indireta | Dez valores; mostra os três últimos resultados | Duas pilhas AAA de 1,5 V | [P4](#p4) |
| **Extech DT100M** | LCD iluminado de quatro linhas e nível de bolha; área, volume, medição indireta, contínua, mínimo/máximo e soma/subtração | Vinte valores | Duas pilhas AAA de 1,5 V | [P5](#p5) |

Essas quantidades descrevem **leituras armazenadas ou apresentadas**, não capacidades de RAM, Flash ou EEPROM. Nas fontes consultadas para os seis aparelhos, não foram identificados fabricante/modelo do MCU, arquitetura/clock, capacidade de memória de programa/dados ou SO. Também não foram identificados, para este comparativo, barramentos internos, ADC/DAC, PWM, interfaces de dados externas/rádios, protocolos, mecanismos de atualização, criptografia, armazenamento externo, PMIC, watchdog e supervisão de energia. Isso registra lacunas documentais, não ausência dos recursos. As fontes de cada linha delimitam as consultas realizadas.

#### 3.5.3 Análise comparativa e relação com a reprodução

**Proximidade funcional.** VTUSD2 e CEM DM-01 se aproximam do VTUSD3 pela medição ultrassônica e pelas funções dimensionais locais. A semelhança entre VTUSD3 e CEM não comprova placa, firmware ou fabricante original comuns. O Stanley tem menor alcance máximo declarado e seu manual caracteriza o instrumento como estimador para interiores, recomendando outras soluções para exigências maiores. [R2](#r2), [P1](#p1), [P2](#p2), [P3](#p3).

**Diferença tecnológica.** As versões documentadas de Bosch e Extech declaram alcances máximos maiores e erros típicos/básicos expressos em milímetros. Essa comparação de especificações não demonstra superioridade universal de qualquer produto a laser. O código completo do Bosch evita misturar variantes. O **DT100M** comparado é a laser e não deve ser confundido com o antigo **DT100**, ultrassônico. [P4](#p4), [P5](#p5).

**Decisão de projeto.** A reprodução com ESP32 manterá botão, aquisição ultrassônica, display e aviso sonoro. Área/volume, memória persistente, apontador laser e desempenho comercial ficam fora do escopo mínimo da seção 3.3. Alcance e erro serão avaliados na montagem real, sem herdar as especificações desses produtos.

## 4. Referências bibliográficas

Listar aqui todas as fontes efetivamente utilizadas, inclusive as das imagens, características técnicas, artigos e similares. Os identificadores devem corresponder às citações no texto. Não inventar DOI para documentos que não tenham um identificador confirmado.

### R1

VELLEMAN. **VTUSD3: Ultrasonic Distance Meter + Laser**. Disponível em: https://www.velleman.eu/products/view/ultrasonic-distance-meter-laser-vtusd3/?id=372828&lang=en. Acesso em: [PREENCHER: data da consulta pelo grupo].

### R2

VELLEMAN. **VTUSD3 — User Manual**. Versão 03, 25 out. 2018. Disponível em: https://cdn.velleman.eu/downloads/1/vtusd3a6v03.pdf. Consulta documental em: 31 out. 2026.

### R3

ELECFREAKS. **Ultrasonic Ranging Module HC-SR04**. Datasheet disponibilizado pela SparkFun, p. 1–3. Disponível em: https://cdn.sparkfun.com/datasheets/Sensors/Proximity/HCSR04.pdf. Acesso em: 30 out. 2026. Referência condicional para o sensor da reprodução; não identifica componentes internos do VTUSD3.

### R4

ESPRESSIF SYSTEMS. **FreeRTOS Overview — ESP-IDF Programming Guide, ESP32**. Disponível em: https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-reference/system/freertos.html. Acesso em: 30 out. 2026. Confirmar documentação correspondente à versão e ao alvo usados na implementação.

### R5

ESPRESSIF SYSTEMS. **Inter-Integrated Circuit (I2C) — ESP-IDF Programming Guide, ESP32**. Disponível em: https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-reference/peripherals/i2c.html. Acesso em: 30 out. 2026. Confirmar documentação correspondente à versão e ao alvo usados na implementação.

### R6

ESPRESSIF SYSTEMS. **Remote Control Transceiver (RMT) — ESP-IDF Programming Guide, ESP32**. Disponível em: https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-reference/peripherals/rmt.html. Acesso em: 30 out. 2026. Recurso proposto para temporização, sujeito à compatibilidade da placa e do driver escolhidos.

### P1

VELLEMAN. **VTUSD2 — Ultrasonic Distance Meter with Laser: manual, versão 3**. Seções 5 e 8–13. Disponível em: https://cdn.velleman.eu/downloads/1/vtusd2gbnlfresd.pdf. Consulta documental em: 31 out. 2026.

### P2

STANLEY. **0-77-018 IntelliMeasure Ultrasonic Estimator — User Manual**. Especificações e operação, p. 2–5 da seção em inglês. Disponível em: https://www.stanley.eu/uploads/it/downloads/manuals/0-77-018%20Intellimeasure%20manual.pdf. Página oficial complementar: https://www.stanleytools.co.nz/product/77-018/stanley-ultrasonic-distance-measure. Consulta documental em: 31 out. 2026.

### P3

CEM. **DM-01 — Ultrasonic Digital Distance Meter**. Ficha técnica de uma página, portal CEM Instruments India. Disponível em: https://www.cem-instruments.in/pdf/DM-01.pdf. Consulta documental em: 31 out. 2026. Notação de exatidão com termo adicional não definido explicitamente, conforme registrado no comparativo.

### P4

BOSCH PROFESSIONAL. **PRO GLM 40 — Medidor de distâncias laser, número de pedido 0 601 072 900**. Dados técnicos e funções. Disponível em: https://www.bosch-professional.com/pt/pt/products/glm-40-0601072900. Consulta documental em: 31 out. 2026.

### P5

EXTECH. **DT100M — Laser Distance Meter**. Especificações e funções. Disponível em: https://www.extech.com/products/dt100m/. Consulta documental em: 31 out. 2026.

### Demais referências

As referências acadêmicas completas T1–T4 e A1–A4 estão no [arquivo bibliográfico](../TrenaUltrassonica/ARTIGOS.md), parte desta documentação. Revisão da seleção em 31 out. 2026; as pendências de consulta integral estão registradas individualmente.

[PREENCHER: outras fontes técnicas e referências das imagens, com identificadores próprios e datas de acesso. As fontes dos similares estão em P1–P5.]

## Checklist de revisão antes da entrega

- [ ] Preencher identificação dos quatro integrantes.
- [ ] Completar descrição, fotos e fontes do produto.
- [ ] Cobrir todos os subitens das 12 categorias técnicas.
- [ ] Justificar informações não identificadas ou não aplicáveis.
- [ ] Destacar tecnologias críticas.
- [x] Redigir proposta, equivalências ESP32, diagramas, fluxo, plano de testes e limitações.
- [ ] Confirmar os módulos reais e revisar a proposta elétrica e os parâmetros antes da montagem.
- [x] Organizar quatro artigos tecnológicos e quatro de uso de instrumentos, com resumos iniciais e links de texto/PDF.
- [ ] Obter os textos integrais pendentes, concluir fichamentos e confirmar o recorte de aplicações da categoria, incluindo o caso a laser.
- [x] Comparar cinco outros produtos e citar suas fontes.
- [ ] Conferir referências completas e correspondência das citações.
- [ ] Remover campos `[PREENCHER]` e instruções editoriais após concluir as seções.
- [ ] Conferir renderização, imagens e links no GitLab.
- [ ] Manter o relatório principal como `VTUSD3/README.md` e submeter conforme a disciplina.
