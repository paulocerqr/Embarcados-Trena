# Resumo — Velleman VTUSD3 e reprodução com ESP32

O grupo estuda o VTUSD3, medidor de distância por ultrassom com apontador laser, e propõe reproduzir sua função principal com uma ESP32, sensor ultrassônico, botão, OLED I2C e buzzer ativo. Um toque solicita uma leitura; o sistema captura o eco, calcula a distância e apresenta resultado ou erro. A alimentação inicial será por USB e a montagem futura, em protoboard.

A proposta exclui laser, rádio, bateria própria, histórico persistente e cálculo de área/volume. Os modelos da placa e dos módulos serão confirmados antes da ligação; o HC-SR04 é somente referência condicional. Não houve montagem ou ensaio, e as metas de teste não são desempenho medido.

O estudo comercial cobre as doze categorias do enunciado, registrando informações não identificadas e suas fontes. A bibliografia contém quatro artigos tecnológicos e quatro de aplicação de instrumentos dimensionais, sem afirmar uso do VTUSD3 pelos autores. O comparativo inclui VTUSD2, Stanley IntelliMeasure, CEM DM-01, Bosch GLM 40 e Extech DT100M.

- [Relatório completo, identificação e proposta](../README.md).
- [Oito artigos, referências, PDFs e resumos críticos](ARTIGOS.md).

Equipe: Paula Lima (211062713), Cristiano Borges (222033952), Isaac Lucas (211031735) e Paulo Cerqueira (211030630).
