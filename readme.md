# Fonte de 5V com Regulador 7805

Este projeto apresenta uma fonte de alimentação linear capaz de fornecer 5V DC a partir da rede elétrica. Utilizando o regulador de tensão 7805, o circuito é ideal para alimentar microcontroladores como Arduino, sensores e qualquer outro dispositivo que funcione com 5V.

---

## Visão Geral

### Modelo 3D
Visualização do projeto em 3D feita no Proteus. Serve como referência para montagem e disposição dos componentes.

![3D](Portofolio/3D/3.png)

---

### Esquemático
Diagrama elétrico com todos os componentes conectados, representando o funcionamento completo da fonte.

![Esquemático](Portofolio/Esquematico/2.png)

---

### PCB
Layout da placa de circuito impresso. Aqui é possível ver a distribuição das trilhas, pads e a organização geral do circuito.

![PCB](Portofolio/PCB/1.png)

---

### Protótipo
Versão montada em protoboard para testes e validação prática do circuito.

![Prática](Portofolio/Pratica/5.png)

---

## Componentes Utilizados

- **TR1** – Transformador que reduz a tensão da rede (110/220V) para 12V AC.
- **BR1** – Ponte retificadora responsável por converter a tensão alternada em contínua pulsante.
- **C1 (1µF)** – Capacitor de filtragem primário, reduz a oscilação da tensão após a retificação.
- **U1 - 7805** – Regulador linear que estabiliza a tensão de saída em 5V.
- **C2 e C3 (22nF)** – Capacitores de desacoplamento que ajudam na estabilidade e redução de ruídos.
- **D1 (LED) + R1 (220Ω)** – Indicador visual de que a fonte está em funcionamento.

---

## Como o Circuito Funciona

1. O transformador reduz a tensão da rede elétrica para uma faixa segura (12V AC).
2. A ponte de diodos retifica essa tensão, convertendo-a para DC pulsante.
3. O capacitor C1 realiza a filtragem inicial, suavizando os picos da tensão retificada.
4. O regulador 7805 recebe essa tensão filtrada e entrega uma saída estabilizada de 5V.
5. Os capacitores C2 e C3 são posicionados próximos ao regulador para garantir que a tensão se mantenha estável e livre de ruídos.
6. O LED em série com o resistor funciona como um indicador visual: se estiver aceso, a fonte está operando corretamente.

---

## Aplicações

- Alimentação de microcontroladores (Arduino, ESP, PIC, etc.)
- Módulos de sensores e displays que operam com 5V
- Protótipos e testes em bancada
- Qualquer aplicação simples que demande 5V regulados

---

## Observações

- O regulador 7805 precisa de uma tensão de entrada mínima de aproximadamente 7V para funcionar corretamente.
- Se o consumo de corrente for alto, é recomendado o uso de um dissipador de calor no regulador para evitar sobreaquecimento.
- O capacitor de filtragem pode ser substituído por um de maior valor (ex: 100µF ou mais) para uma resposta melhor em cargas mais exigentes.

---

