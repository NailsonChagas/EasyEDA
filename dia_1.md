Aqui está o texto revisado, formatado em **markdown** e com pequenas correções e complementos técnicos:

---

# Montagem de PCB usando EasyEDA — Dia 1

> **Observação:** o projeto do circuito eletrônico **não será abordado neste curso**. O foco será o processo de **criação, roteamento e montagem** da placa de circuito impresso (PCB).

---

## Etapas do curso

1. **Criação do esquemático** do circuito no EasyEDA
2. **Roteamento (routes)** da PCB
3. **Confecção da placa** (transferência térmica + corrosão)
4. **Montagem e teste** dos componentes na PCB

> ⚙️ **Dica:** Antes de passar do esquemático (etapa 1) para o roteamento (etapa 2), **verifique o DRC** (*Design Rule Check*) no menu **Design**, para evitar erros de ligação e sobreposição.

---

## Conceitos importantes

* **Footprint:** representa **como o componente é montado fisicamente na placa** (a disposição de seus terminais e dimensões).
  Exemplos de tipos de encapsulamento:

  * **SOP** — Small Outline Package
  * **SO** — Small Outline
  * **PDIP** — Plastic Dual Inline Package
  * **DIP** — Dual Inline Package
  * **SOIC** — Small Outline Integrated Circuit

* **TH (Through-Hole):** componentes **com terminais furados**, que atravessam a placa.

  * Mais fáceis de soldar manualmente.
  * Costumam exigir o uso de **soquetes (sockets)** ou **perfuração** da placa.

* **SMD (Surface-Mount Device):** tecnologia de **montagem superficial**, em que os componentes ficam “sentados” sobre a placa.

  * Menores e mais baratos que os TH.
  * Mais difíceis de manusear e soldar manualmente.

---

## Circuito a ser montado

O circuito escolhido para este curso será um **VU Meter** (indicador de nível de sinal).

**Componentes principais:**

* **TL082CP** (amplificador operacional duplo)
* **Versão TH (Through-Hole)** dos componentes

> Um esquemático pode conter **mais de uma folha (sheet)**. Em projetos complexos, isso facilita a organização.
> Neste curso, utilizaremos **apenas uma folha**.

---

## Comandos importantes no EasyEDA

* **P → Place:** abre o menu de **inserção de componentes padrões**.
* **P + P:** abre a **interface de busca de componentes** em fornecedores integrados (ex.: LCSC).

---

## Dicas ao inserir componentes

* **X.1, X.2, X.3…** → indicam **instâncias diferentes** de um mesmo componente (por exemplo, canais distintos de um mesmo CI).
* Os **números nos pinos** indicam **qual porta ou terminal** corresponde àquele sinal no componente.

> 🧩 Exemplo: O TL082 tem dois amplificadores internos (A e B). Assim, os símbolos **U1A** e **U1B** representam os dois canais do mesmo CI físico.
