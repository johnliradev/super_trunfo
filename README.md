# Super Trunfo de Cidades - Projeto em Linguagem C

Este projeto é uma implementação simples do jogo **Super Trunfo**, adaptado para comparar **cidades brasileiras** com base em atributos geográficos e econômicos. O sistema foi desenvolvido em linguagem C para fins educacionais, como parte de um trabalho de faculdade.

---

## 💡 Objetivo

Criar um programa em C que:

1. Cadastre duas cartas de cidades.
2. Calcule métricas como **densidade populacional** e **PIB per capita**.
3. Compare as cartas com base em seus atributos.
4. Determine qual cidade vence em cada categoria.
5. Calcule o **Super Poder** de cada carta e determine a vencedora geral.

---

## 📋 Informações Coletadas por Carta

- **Estado** (char): Letra de `A` a `H`
- **Código da Carta** (string): Ex: `A01`
- **Nome da Cidade** (string)
- **População** (`unsigned long int`)
- **Área (km²)** (`float`)
- **PIB (bilhões de reais)** (`float`)
- **Número de Pontos Turísticos** (`int`)

---

## 📈 Cálculos Realizados

- **Densidade Populacional** = população / área
- **PIB per Capita** = PIB / população
- **Super Poder** =  
  `população + área + PIB + pontos_turisticos + pib_per_capita + (1 / densidade_populacional)`

> Os valores são convertidos corretamente para `float` onde necessário.

---

## 🏆 Comparações Realizadas

Para cada atributo numérico, o programa indica se a **Carta 1 venceu (1)** ou **Carta 2 venceu (0)**.  
**Atenção**: na densidade populacional, **menor valor vence**; nos demais, vence o **maior valor**.

---

## 🖥️ Exemplo de Entrada

Cadastro da Carta 1:

Estado (A-H): A
Código (ex: A01): A01
Nome da Cidade: Alpha City
População: 2000000
Área (km²): 500.5
PIB (em bilhões): 25.3

Número de Pontos Turísticos: 15

Cadastro da Carta 2:
Estado (A-H): B
Código (ex: B02): B02
Nome da Cidade: Beta Town
População: 1500000
Área (km²): 700.7
PIB (em bilhões): 20.1
Número de Pontos Turísticos: 18

---

## 🧮 Exemplo de Saída (parcial)

Comparação de Cartas:

População: Carta 1 venceu (1)
Área: Carta 2 venceu (0)
PIB: Carta 1 venceu (1)
Pontos Turísticos: Carta 2 venceu (0)
Densidade Populacional: Carta 2 venceu (0)
PIB per Capita: Carta 1 venceu (1)
Super Poder: Carta 1 venceu (1)

---

## 🛠️ Requisitos Técnicos

- Compilador C compatível com o padrão C99 ou superior.
- Sistema com terminal para entrada e saída padrão.

---

## 🧾 Licença

Uso acadêmico apenas.
