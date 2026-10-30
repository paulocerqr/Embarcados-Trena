# Artigos científicos — seleção inicial para a trena ultrassônica

Pesquisa realizada em 29/10/2026. Foram selecionados **quatro artigos sobre tecnologias e quatro sobre aplicações da medição ultrassônica**. Todos são de revistas; não foram incluídos trabalhos de congresso como parte dos oito.

Esta é uma seleção comentada, não oito fichamentos finais de leitura integral. Os resumos abaixo se apoiam nos resumos publicados e nos trechos acessíveis das fontes indicadas. O acesso integral não foi possível para todos os PDFs; a situação está indicada em cada entrada. Nenhum PDF foi adicionado ao repositório.

**Limite da seleção:** nenhum desses trabalhos foi identificado como estudo ou aplicação do Velleman VTUSD3 especificamente. Os de aplicação tratam de instrumentos e sistemas relacionados à medição de distância. O enunciado pede aplicações/uso do produto; a adequação desse recorte à categoria do produto precisa ser confirmada com o professor antes de fechar a bibliografia. Não descrever essas pesquisas como ensaios do VTUSD3.

## 1. Visão geral e divisão da leitura

| Código | Assunto | Relação com o projeto | Leitura sugerida |
| --- | --- | --- | --- |
| T1 | Revisão de medição ultrassônica | Fundamentos, sensores e limites | Integrante 1 |
| T2 | Influência do ambiente | Erros de temperatura, umidade e vento | Integrante 2 |
| T3 | Rejeição de interferência | Ecos de outros sensores e validação | Integrante 3 |
| T4 | Alternativa ao tempo de voo | Comparação de técnicas e justificativa do recorte simples | Integrante 4 |
| A1 | Instrumento de distância com microcontrolador | Aplicação mais próxima da trena proposta | Integrante 1 |
| A2 | Medições em investigação de cena | Uso de um medidor e registro de distâncias | Integrante 2 |
| A3 | Instrumento de medição de altura | Uso de distância para medir uma dimensão | Integrante 3 |
| A4 | Localização em ambiente interno | Aplicação ampliada de medidas de distância | Integrante 4 |

Começar por T1 e A1. T3, T4 e A4 são mais avançados e servem à discussão bibliográfica; não exigem implementar suas técnicas no protótipo.

## 2. Tecnologias que viabilizam a medição

### T1 — Princípios e métodos de medição

**Referência:** QIU, Zurong; LU, Yaohuan; QIU, Zhen. Review of Ultrasonic Ranging Methods and Their Current Challenges. *Micromachines*, v. 13, n. 4, art. 520, 2022.

- DOI: [10.3390/mi13040520](https://doi.org/10.3390/mi13040520).
- [Página da revista](https://www.mdpi.com/2072-666X/13/4/520).
- [Texto integral no PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC9025471/).
- [PDF publicado no repositório da Liverpool John Moores University](https://researchonline.ljmu.ac.uk/id/eprint/18696/1/Review%20of%20Ultrasonic%20Ranging%20Methods%20and%20Their%20Current%20Challenges.pdf).
- Idioma: inglês. Texto integral consultado em versão HTML; PDF identificado no repositório institucional.

**Resumo inicial:** A revisão organiza transdutores, métodos de cálculo da distância e processamento de sinais. Explica o papel da detecção do eco, da velocidade do som e das condições ambientais nos limites da medição.

**Aplicação no relatório:** fundamentar o percurso de ida e volta e as limitações do sensor. Não atribuir ao módulo simples o desempenho de todas as técnicas revisadas.

### T2 — Erros provocados pelo ambiente

**Referência:** RUDYK, Andrii et al. Influence of Environmental Factors on the Accuracy of the Ultrasonic Rangefinder in a Mobile Robotic Technical Vision System. *Electronics*, v. 14, n. 7, art. 1393, 2025.

- DOI: [10.3390/electronics14071393](https://doi.org/10.3390/electronics14071393).
- [Página da revista](https://www.mdpi.com/2079-9292/14/7/1393).
- [PDF oficial](https://www.mdpi.com/2079-9292/14/7/1393/pdf).
- [Registro editorial do PDF](https://www.mdpi.com/2079-9292/14/7/1393/notes).
- Idioma: inglês. Resumo e trechos indexados consultados; o servidor limitou o acesso direto ao texto/PDF durante a pesquisa. O registro editorial confirma o endereço do arquivo; falta leitura integral.

**Resumo inicial:** O estudo combina análise e experimentação para investigar temperatura, umidade, pressão e vento na resposta de um sistema ultrassônico. A temperatura aparece como influência importante nas condições estudadas.

**Aplicação no relatório:** justificar registro das condições dos ensaios e cautela com velocidade do som fixa. Não exige adicionar sensores ambientais ao escopo mínimo.

### T3 — Interferência entre sensores

**Referência:** SHIN, Seungin; KIM, Min Hyun; CHOI, Seibum B. Ultrasonic Distance Measurement Method With Crosstalk Rejection at High Measurement Rate. *IEEE Transactions on Instrumentation and Measurement*, v. 68, n. 4, p. 972–979, 2019.

- DOI: [10.1109/TIM.2018.2863999](https://doi.org/10.1109/TIM.2018.2863999).
- [Registro institucional da KAIST](https://pure.kaist.ac.kr/en/publications/ultrasonic-distance-measurement-method-with-crosstalk-rejection-a/).
- [PDF no laboratório dos autores](https://acl.kaist.ac.kr/wp-content/uploads/2021/10/2018_TIM_SSI.pdf).
- Idioma: inglês. Referência e resumo confirmados no registro institucional; trechos do PDF estavam indexados, mas sua abertura direta terminou em timeout. Conferir o acesso antes da entrega.

**Resumo inicial:** Os autores estudam sinais codificados e processamento para medir distância e rejeitar interferência de outros sistemas ultrassônicos. A técnica busca conciliar velocidade de medição e custo computacional.

**Aplicação no relatório:** explicar por que nem todo retorno detectado é confiável. A codificação proposta não será implementada no módulo didático; o protótipo deve registrar essa limitação.

### T4 — Uma alternativa ao tempo de voo

**Referência:** CAROTENUTO, Riccardo; PEZZIMENTI, Fortunato; DELLA CORTE, Francesco G.; IERO, Demetrio; MERENDA, Massimo. Ranging with Frequency Dependent Ultrasound Air Attenuation. *Sensors*, v. 21, n. 15, art. 4963, 2021.

- DOI: [10.3390/s21154963](https://doi.org/10.3390/s21154963).
- [Página da revista](https://www.mdpi.com/1424-8220/21/15/4963).
- [PDF publicado em repositório institucional](https://iris.unirc.it/retrieve/e2047589-0489-7e24-e053-6605fe0afb29/Carotenuto2021_sensors-21-04963.pdf).
- Idioma: inglês. PDF aberto e conteúdo consultado.

**Resumo inicial:** O artigo propõe estimar a distância pela atenuação de sinais de diferentes frequências, sem depender da sincronização necessária em certas configurações de tempo de voo. Apresenta formulação e avaliação por simulação.

**Aplicação no relatório:** comparar caminhos tecnológicos e explicar por que a reprodução usa medição simples de eco. Não é evidência de que o VTUSD3 ou o HC-SR04 empreguem o método do artigo. É a referência de relação menos direta com a implementação e pode ser substituída por estudo experimental de tempo de voo após a leitura do grupo.

## 3. Aplicações de instrumentos e sistemas relacionados

### A1 — Instrumento de distância com microcontrolador e display

**Referência:** TITLEE, Rokhsana; BHUYAN, Muhibul Haque. Design, Implementation and Testing of Ultrasonic High Precision Contactless Distance Measurement System Using Microcontroller. *SEU Journal of Science and Engineering*, v. 10, n. 2, dez. 2016.

- [PDF original no domínio da universidade](https://old.seu.edu.bd/seujse/downloads/vol_10_no_2_dec_2016/02_Vol10No2Dec2016.pdf).
- DOI: não identificado no documento consultado; não inventar um identificador.
- Idioma: inglês. PDF aberto; conferir a paginação bibliográfica ao preparar a versão final.

**Resumo inicial:** Apresenta um instrumento com PIC16F877A, HC-SR04 e LCD. O microcontrolador processa o retorno ultrassônico e apresenta a distância; o estudo compara medições com valores de referência.

**Aplicação no relatório:** é a entrada mais próxima do fluxo sensor → processamento → display da nossa trena. A ESP32 substitui o controlador; desempenho e código não devem ser transplantados sem análise.

### A2 — Medir e registrar distâncias em uma cena

**Referência:** SUNGKANGWAN, Thosaporn; PRAIHIRUNKIT, Pairoa. Smartphone Application with an Ultrasonic Sensor for Measuring and Recording Distance in Crime Scene Investigation. *The Journal of King Mongkut’s University of Technology North Bangkok*, v. 32, n. 1, p. 177–188, 2022.

- DOI: [10.14416/j.kmutnb.2021.05.039](https://doi.org/10.14416/j.kmutnb.2021.05.039).
- [Página da revista](https://ph01.tci-thaijo.org/index.php/kmutnb-journal/article/view/247198).
- [Link de download disponibilizado pela revista](https://ph01.tci-thaijo.org/index.php/kmutnb-journal/article/download/247198/167963).
- Idioma: tailandês, com título e resumo em inglês. A página e o resumo foram consultados; o download oficial não abriu nesta pesquisa. Ano da referência segue o fascículo de 2022, apesar das datas de publicação online anteriores.

**Resumo inicial:** O trabalho integra um sensor ultrassônico a um aplicativo para medir e registrar distâncias em cenários simulados de investigação. Também avalia o uso da interface por profissionais.

**Aplicação no relatório:** mostra que apresentar, registrar e interpretar a distância é parte da utilidade do instrumento. Nosso escopo não inclui aplicativo nem finalidade pericial. A leitura do texto completo exigirá tradução cuidadosa.

### A3 — Medição de altura a partir da distância

**Referência:** WONGKE, Thunyarat; AWIKUNPRASERT, Panatsada; AWIKUNPRASERT, Chayanon. Digital height meter using ultrasonic sensor. *Journal of Associated Medical Sciences*, v. 50, n. 3, p. 435–441, 2017.

- DOI: [10.14456/jams.2017.60](https://doi.org/10.14456/jams.2017.60).
- [Página da revista](https://he01.tci-thaijo.org/index.php/bulletinAMS/article/view/85156).
- [PDF original](https://he01.tci-thaijo.org/index.php/bulletinAMS/article/download/85156/74346).
- Idioma: tailandês, com resumo em inglês e ilustrações. PDF aberto; a síntese inicial usa o resumo em inglês e os elementos técnicos identificáveis, não uma tradução integral.

**Resumo inicial:** Um instrumento usa ultrassom, Arduino, sensor de temperatura e LCD para calcular altura. Os autores comparam resultados com método convencional e discutem o efeito da superfície de reflexão.

**Aplicação no relatório:** relacionar medida de distância, referência geométrica e validação experimental. A trena não será apresentada como instrumento clínico; não se deve repetir uma equação extraída do texto sem conferir unidades e coerência física.

### A4 — Uso de distâncias para localização interna

**Referência:** CHEW, Moi Tin; ALAM, Fakhrul; LEGG, Mathew; SEN GUPTA, Gourab. Accurate Ultrasound Indoor Localization Using Spring-Relaxation Technique. *Electronics*, v. 10, n. 11, art. 1290, 2021.

- DOI: [10.3390/electronics10111290](https://doi.org/10.3390/electronics10111290).
- [Página da revista](https://www.mdpi.com/2079-9292/10/11/1290).
- [PDF oficial](https://www.mdpi.com/2079-9292/10/11/1290/pdf).
- [Registro institucional da Massey University](https://mro.massey.ac.nz/items/67e42f3c-71fa-43a8-98fc-a86a852d0c18).
- Idioma: inglês. Conteúdo da página e registro institucional consultados; a abertura direta do PDF oficial falhou nesta pesquisa. O repositório confirma esse endereço como acesso aberto.

**Resumo inicial:** O estudo mede tempos de propagação ultrassônica para estimar a posição de um receptor em uma área interna. Compara estratégias de posicionamento e avalia experimentalmente o erro.

**Aplicação no relatório:** mostrar como medidas individuais de distância sustentam uma aplicação espacial mais ampla. O sistema exige múltiplas referências e processamento além da trena, portanto é aplicação da tecnologia, não reprodução do mesmo instrumento.

## 4. Como transformar a seleção em entrega

1. Confirmar o recorte de aplicação do produto/categoria exigido pelo professor. A1 é o mais próximo de um instrumento equivalente; A4 é mais distante.
2. Cada integrante abre os textos completos de suas duas entradas. Resolver os acessos pendentes antes de tratá-las como bibliografia final.
3. Para A2 e A3, usar tradução com conferência das figuras, unidades e método. Se o idioma impedir a compreensão, substituir o artigo; não entregar um resumo que ninguém do grupo consiga explicar.
4. Registrar problema, método, resultado principal, limitações e relação com o projeto. Os resumos iniciais deste arquivo não substituem essa leitura.
5. Anotar páginas/seções que sustentam cada afirmação. Completar metadados e incluir data real de acesso na versão final.
6. Verificar os links dos PDFs no navegador da equipe. Usar o acesso institucional quando necessário; não fazer upload de PDFs ao repositório.
7. Reescrever a seção acadêmica com palavras próprias e referências. Não copiar resumos de trabalhos anteriores do acervo.

## 5. Situação da pesquisa

Há oito referências de revistas identificadas e relacionadas à medição ultrassônica, com links de texto/PDF. A seleção demonstra disponibilidade de bibliografia, mas **não está encerrada**: restam leitura integral, resolução de acessos, decisão sobre os dois textos em tailandês e confirmação do recorte de aplicação. A existência de uma referência não comprova sozinha sua adequação ao critério do professor.

Alternativa a pesquisar se for necessário substituir aplicações: [Room measurement tool combining ultrasonic and inertial sensors in smartphones](https://kyushu-u.elsevierpure.com/en/publications/room-measurement-tool-combining-ultrasonic-and-inertial-sensors-i/), de Kashimoto, Arakawa e Yasumoto, *International Journal of Ad Hoc and Ubiquitous Computing*, 31(3), 189–199, 2019, DOI [10.1504/IJAHUC.2019.100779](https://doi.org/10.1504/IJAHUC.2019.100779). O resumo é próximo da medição de ambientes, mas não foi localizado um PDF independente do artigo nesta consulta; uma tese ou versão de congresso não deve substituí-lo silenciosamente.
