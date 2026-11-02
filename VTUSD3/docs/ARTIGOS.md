# Pesquisa bibliográfica — trena ultrassônica
Esta pesquisa reúne **oito artigos distintos de revistas científicas**, quatro tecnológicos (T1–T4) e quatro de aplicação (A1–A4). Os PDFs originais são apenas vinculados, sem cópias no repositório.

**Recorte de aplicação.** A1 trata de instrumento equivalente; A2, de medição e registro de distâncias; A3, de medição dimensional derivada da distância; A4 documenta uso de medidor ultrassônico comercial. São aplicações da categoria funcional, não do modelo VTUSD3. Não foi localizado, nas consultas realizadas, estudo que utilizasse explicitamente esse modelo. Essa distinção é um limite de aderência ao termo “produto” do enunciado, sobretudo em A3.
## Método de pesquisa

Consulta e revisão em 02 nov. 2026, com busca por título, DOI e termos `ultrasonic ranging`, `ultrasonic distance measurement`, `distance meter application` e `ultrasonic height meter`. Foram utilizados PubMed/PMC, portais de revistas (MDPI, SEU e TCI-ThaiJO) e repositórios institucionais LJMU e KAIST. A referência de T3 também foi conferida no registro institucional que identifica sua publicação no periódico IEEE. Não se declara pesquisa autenticada no Portal Capes, Scopus ou IEEE Xplore.

Critérios: artigo de revista, identidade bibliográfica verificável, relação explícita com transdução/medição acústica ou uso de instrumento dimensional e link do PDF original. Foram excluídos da contagem trabalhos de congresso, manuais e textos apenas sobre navegação sem instrumento dimensional como foco de aplicação. A evidência consultada está declarada em cada entrada; não se atribui leitura integral ao grupo nem tradução integral dos artigos em tailandês.

## Seleção e contribuição

| Código | Eixo | Contribuição |
| --- | --- | --- |
| [T1](#t1) | Tecnologia | Fundamentos da medição ultrassônica |
| [T2](#t2) | Tecnologia | Influência das condições ambientais |
| [T3](#t3) | Tecnologia | Rejeição de interferência entre sensores |
| [T4](#t4) | Tecnologia | Estimação do tempo de voo com ecos sobrepostos |
| [A1](#a1) | Aplicação | Instrumento portátil de distância com microcontrolador |
| [A2](#a2) | Aplicação | Registro de distâncias em investigação de cenas |
| [A3](#a3) | Aplicação | Uso da distância ultrassônica para medir altura |
| [A4](#a4) | Aplicação | Levantamento de áreas com medidor ultrassônico comercial |

<a id="t1"></a>

## T1 — Fundamentos da medição ultrassônica

**Referência:** QIU, Zurong; LU, Yaohuan; QIU, Zhen. Review of Ultrasonic Ranging Methods and Their Current Challenges. *Micromachines*, v. 13, n. 4, art. 520, 2022.

**DOI:** [10.3390/mi13040520](https://doi.org/10.3390/mi13040520).

[Página/registro](<https://www.mdpi.com/2072-666X/13/4/520>) · [PDF original](<https://researchonline.ljmu.ac.uk/id/eprint/18696/1/Review%20of%20Ultrasonic%20Ranging%20Methods%20and%20Their%20Current%20Challenges.pdf>). Consulta em: 02 nov. 2026.

**Evidência consultada:** Revisão consultada no PDF institucional e no conteúdo indexado do PMC; seções 2, 4 e 5.

**Problema, método e resultado:** A revisão compara transdutores, técnicas de tempo de voo, fase e codificação e métodos de extração do eco. Identifica compromissos entre alcance, exatidão, consumo e processamento, além de erros de aquisição e de velocidade do som. Por reunir sistemas heterogêneos, não estabelece uma especificação única para todos os sensores.

**Relação com o produto e sistemas embarcados:** Fundamenta transdução, temporização e cálculo de distância. Na ESP32, sustenta captura temporal e validação de faixa; técnicas avançadas revisadas não são automaticamente recursos do módulo didático.

<a id="t2"></a>

## T2 — Influência das condições ambientais

**Referência:** RUDYK, Andrii; SEMENOV, Andriy; BARABAN, Serhii; SEMENOVA, Olena; KULAKOV, Pavlo; KUSTOVSKYJ, Oleksandr; BRYCH, Lesia. Influence of Environmental Factors on the Accuracy of the Ultrasonic Rangefinder in a Mobile Robotic Technical Vision System. *Electronics*, v. 14, n. 7, art. 1393, 2025.

**DOI:** [10.3390/electronics14071393](https://doi.org/10.3390/electronics14071393).

[Página/registro](<https://www.mdpi.com/2079-9292/14/7/1393>) · [PDF original](<https://res.mdpi.com/electronics/electronics-14-01393/article_deploy/electronics-14-01393.pdf>). Consulta em: 02 nov. 2026.

**Evidência consultada:** PDF da editora consultado, obtido pelo servidor de conteúdo; seções 3–5 e tabela 5. A rota principal pode bloquear acesso automatizado.

**Problema, método e resultado:** O estudo combina modelagem, sensores ambientais e ensaios de um telémetro embarcado em robô. A análise de 256 medições aponta temperatura como influência dominante nas condições estudadas; material refletor e vento também importam. A tabela experimental mostra alcance estável diferente para vidro e tecido. Esses resultados dependem do arranjo e não caracterizam o VTUSD3.

**Relação com o produto e sistemas embarcados:** Justifica declarar a hipótese de velocidade do som fixa e registrar condições e superfície nos ensaios. Compensação ambiental seria uma evolução do firmware, sem exigir rede neural ou sensores adicionais no escopo mínimo.

<a id="t3"></a>

## T3 — Rejeição de interferência entre sensores

**Referência:** SHIN, Seungin; KIM, Min-Hyun; CHOI, Seibum B. Ultrasonic Distance Measurement Method With Crosstalk Rejection at High Measurement Rate. *IEEE Transactions on Instrumentation and Measurement*, v. 68, n. 4, p. 972–979, 2019.

**DOI:** [10.1109/TIM.2018.2863999](https://doi.org/10.1109/TIM.2018.2863999).

[Página/registro](<https://pure.kaist.ac.kr/en/publications/ultrasonic-distance-measurement-method-with-crosstalk-rejection-a/>) · [PDF original](<https://acl.kaist.ac.kr/wp-content/uploads/2021/10/2018_TIM_SSI.pdf>). Consulta em: 02 nov. 2026.

**Evidência consultada:** PDF dos autores consultado; seções V–VII, especialmente experimento da seção VI. Metadados conferidos no registro institucional KAIST.

**Problema, método e resultado:** Os autores codificam pulsos por modulação caótica de posição e usam processamento de um bit e correlação para estimar o tempo de voo. Simulações avaliam interferência; um ensaio em veículo contra parede apresenta erro RMS de 29 mm. Parte do processamento experimental foi feita offline, portanto o artigo não demonstra essa cadeia completa em tempo real em uma ESP32.

**Relação com o produto e sistemas embarcados:** Mostra que selecionar ecos confiáveis exige processamento e memória. Apoia os intervalos entre disparos e a discussão de interferência; a reprodução não implementa codificação nem acesso ao sinal acústico bruto.

<a id="t4"></a>

## T4 — Estimação do tempo de voo com ecos sobrepostos

**Referência:** SARABIA, Esther G.; LLATA, Jose R.; ROBLA, Sandra; TORRE, Carlos; ORIA, Juan P. Accurate Estimation of Airborne Ultrasonic Time-of-Flight for Overlapping Echoes. *Sensors*, v. 13, n. 11, p. 15465–15488, 2013.

**DOI:** [10.3390/s131115465](https://doi.org/10.3390/s131115465).

[Página/registro](<https://www.mdpi.com/1424-8220/13/11/15465>) · [PDF original](<https://mdpi-res.com/d_attachment/sensors/sensors-13-15465/article_deploy/sensors-13-15465.pdf>). Consulta em: 02 nov. 2026.

**Evidência consultada:** PDF da editora consultado; análise de detecção, figuras 26–31 e seção 5.

**Problema, método e resultado:** O trabalho modela a resposta transitória de sensores piezoelétricos, considerando excitação, diretividade e atenuação. Compara limiar e correlação com uma estimativa baseada nos máximos do sinal. Os exemplos experimentais mostram a identificação de tempos iniciais de subecos parcialmente sobrepostos. O resultado depende do modelo e da aquisição do sinal, não somente de medir a largura de um pulso digital.

**Relação com o produto e sistemas embarcados:** Detalha a tecnologia de detecção necessária à medição por eco. Explica por que um módulo TRIG/ECHO oculta decisões do receptor e por que alvos múltiplos podem limitar a reprodução simples.

<a id="a1"></a>

## A1 — Instrumento portátil de distância com microcontrolador

**Referência:** TITLEE, Rokhsana; BHUYAN, Muhibul Haque. Design, Implementation and Testing of Ultrasonic High Precision Contactless Distance Measurement System Using Microcontroller. *SEU Journal of Science and Engineering*, v. 10, n. 2, p. 6–11, 2016.

**DOI:** não identificado no documento.

[Página/registro](<https://old.seu.edu.bd/seujse/downloads/vol_10_no_2_dec_2016/02_Vol10No2Dec2016.pdf>) · [PDF original](<https://old.seu.edu.bd/seujse/downloads/vol_10_no_2_dec_2016/02_Vol10No2Dec2016.pdf>). Consulta em: 02 nov. 2026.

**Evidência consultada:** PDF original consultado; seções II–VI e tabela I.

**Problema, método e resultado:** O instrumento integra PIC16F877A, HC-SR04, temporizador e LCD. Os autores comparam 22 distâncias com uma escala de aço e relatam boa concordância. A tabela apresenta inconsistência aritmética: 2,00 cm e 2,02 cm correspondem a 1%, mas a linha informa 0,500%. Assim, a média de erro publicada não é adotada como garantia de desempenho.

**Relação com o produto e sistemas embarcados:** É uso de um instrumento funcionalmente próximo da trena. Orienta integração e comparação com referência física; na ESP32, temporização e interface serão próprias. O intervalo de disparos seguirá o datasheet do módulo, não valores conflitantes do artigo.

<a id="a2"></a>

## A2 — Registro de distâncias em investigação de cenas

**Referência:** SUNGKANGWAN, Thosaporn; PRAIHIRUNKIT, Pairoa. Smartphone Application with an Ultrasonic Sensor for Measuring and Recording Distance in Crime Scene Investigation. *The Journal of King Mongkut’s University of Technology North Bangkok*, v. 32, n. 1, p. 177–188, 2022.

**DOI:** [10.14416/j.kmutnb.2021.05.039](https://doi.org/10.14416/j.kmutnb.2021.05.039).

[Página/registro](<https://ph01.tci-thaijo.org/index.php/kmutnb-journal/article/view/247198>) · [PDF original](<https://ph01.tci-thaijo.org/index.php/kmutnb-journal/article/download/247198/167963>). Consulta em: 02 nov. 2026.

**Evidência consultada:** Resumo em inglês na página da revista e no PDF, p. 178. Corpo em tailandês; não se declara tradução integral.

**Problema, método e resultado:** O sistema associa sensor ultrassônico a aplicativo para medir distâncias e gerar registros de uma cena simulada. O resumo relata erro de distância de ±7 cm e avaliação de uso por vinte policiais. A comparação com medidor laser e a satisfação dos usuários não equivalem a calibração metrológica nem validam qualquer aparelho comercial.

**Relação com o produto e sistemas embarcados:** Demonstra medição dimensional aplicada a documentação de campo. Relaciona aquisição embarcada, apresentação e registro; a proposta mantém apenas medição e interface locais, sem aplicativo ou alegação de aptidão pericial.

<a id="a3"></a>

## A3 — Uso da distância ultrassônica para medir altura

**Referência:** WONGKE, Thunyarat; AWIKUNPRASERT, Panatsada; AWIKUNPRASERT, Chayanon. Digital height meter using ultrasonic sensor. *Journal of Associated Medical Sciences*, v. 50, n. 3, p. 435–441, 2017.

**DOI:** [10.14456/jams.2017.60](https://doi.org/10.14456/jams.2017.60).

[Página/registro](<https://he01.tci-thaijo.org/index.php/bulletinAMS/article/view/85156>) · [PDF original](<https://he01.tci-thaijo.org/index.php/bulletinAMS/article/download/85156/74346>). Consulta em: 02 nov. 2026.

**Evidência consultada:** Resumo em inglês da revista e do PDF, p. 435. Corpo em tailandês; a síntese se limita ao resumo publicado.

**Problema, método e resultado:** O instrumento combina Arduino, ultrassom, sensor de temperatura e LCD para medir altura. O resumo informa erro de 0,6–1,0% nos ensaios de distância de 2–200 cm. Na comparação de altura, relata erro de 4% sem anteparo e 1% com cartão plano sobre o alvo. A geometria de reflexão limita a transferência desses resultados a outros usos.

**Relação com o produto e sistemas embarcados:** É aplicação de medição dimensional derivada da distância, não ensaio de uma trena portátil. Relaciona referência geométrica, compensação e interface embarcada; sustenta o uso de alvo plano no teste, sem conferir finalidade clínica ao protótipo.

<a id="a4"></a>

## A4 — Levantamento de áreas com medidor ultrassônico comercial

**Referência:** YU, Sol; YANG, Wonho; LEE, Kiyoung; KIM, Sungcheon; HA, Kwonchul; KIM, Sungroul. Short-Term Impact of a Comprehensive Smoke-Free Law Following a Partial Smoke-Free Law on PM2.5 Concentration Levels at Hospitality Venues on the Peripheries of College Campuses. *International Journal of Environmental Research and Public Health*, v. 12, n. 11, p. 14034–14042, 2015.

**DOI:** [10.3390/ijerph121114034](https://doi.org/10.3390/ijerph121114034).

[Página/registro](<https://pmc.ncbi.nlm.nih.gov/articles/PMC4661630/>) · [PDF original](<https://res.mdpi.com/ijerph/ijerph-12-14034/article_deploy/ijerph-12-14034.pdf>). Consulta em: 02 nov. 2026.

**Evidência consultada:** PDF da editora consultado; seção 2.1 para uso do instrumento, resumo e resultados para contexto do estudo.

**Problema, método e resultado:** O estudo compara concentrações de partículas em estabelecimentos antes e depois de uma restrição ao fumo. A seção 2.1 documenta medidor ultrassônico comercial Zircon para levantar a área interna. Os autores relatam redução da mediana de PM2.5, sem diferença estatisticamente significativa no resumo. O artigo não avalia erro ou arquitetura do medidor.

**Relação com o produto e sistemas embarcados:** É uso real de produto da mesma categoria para obter dimensões de ambientes, próximo da função de área do VTUSD3. O sistema embarcado fornece dado geométrico auxiliar; partículas são medidas por outro instrumento, não pela trena.

## Síntese para a proposta

T1 e T4 fundamentam a aquisição de ecos; T2 explica as limitações ambientais; T3 evidencia os custos de rejeitar interferência. A1 orienta uma integração simples e a leitura crítica dos resultados; A2–A4 demonstram finalidades de medições dimensionais. A proposta permanece com um sensor, uma solicitação por botão e apresentação local. Nenhum resultado dos artigos é declarado resultado do grupo, e nenhum artigo comprova o circuito interno do VTUSD3.
