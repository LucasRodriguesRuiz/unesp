# 🧠 Lógica Clássica e Demonstrações Matemáticas

---

## 🏛️ Princípios da Lógica Clássica

| Princípio                       | Representação Lógica |
| :------------------------------ | :------------------: |
| **Não Contradição**             |     `¬(A ∧ ¬A)`      |
| **Terceiro Excluído**           |       `A ∨ ¬A`       |
| **Reflexividade da Identidade** |    `(∀x)(x = x)`     |

---

## 🔗 Conectivos Lógicos (Operadores)

| Símbolo | Significado                   |
| :-----: | :---------------------------- |
|   `¬`   | Não (Negação)                 |
|   `∧`   | E (Conjunção)                 |
|   `∨`   | Ou (Disjunção)                |
|   `→`   | Se..., Então... (Condicional) |

---

## 📐 Sistema Axiomático

> **Axiomas** são verdades aceitas de forma universal dentro de um certo cenário ou teoria, sem a necessidade de demonstração.

### Axiomas do Cálculo Proposicional Clássico

| Axioma | Nome |
| :--- | :---: |
| `A → (B → A)` | **Monotonicidade** |
| `((A → B) ∧ (B → C)) → (A → C)` | **Transitividade** |
| `((¬A → ¬B) ∧ (¬A → B)) → A` | **Redução ao Absurdo** |

### Regra de Inferência: *Modus Ponens*
Se temos a premissa de que **A implica B** e sabemos que **A é verdade**, logo **B também é verdade**.
> **Notação:** `A → B, A ⊢ B`

> [!NOTE] Terminologia
> O **Cálculo Proposicional Clássico (CPC)** também pode ser conhecido como **Lógica Proposicional Clássica (LPC)**.

---

## 📖 Fatos Matemáticos

Enquanto *Axiomas* e *Postulados* são demonstrados por si próprios (verdades assumidas), **Fatos Matemáticos devem ser demonstrados**. Eles são classificados hierarquicamente na matemática:

- **Proposição:** Um fato simplório ou afirmação básica que pode ser classificada como verdadeira ou falsa.
- **Lema:** Um fato (teorema auxiliar) usado especificamente como degrau/ferramenta para demonstrar um Teorema maior.
- **Teorema:** Um fato de grande importância para a teoria, que exige demonstração formal.
- **Corolário:** Uma consequência direta ou fato demonstrado a partir de um Teorema que já foi previamente provado.

---

## 🛠️ Técnicas de Demonstração

A estrutura básica de uma demonstração segue o formato:
> **Se `A`, então `B`**  *( `A → B` )*

Onde **`A`** é a nossa **Hipótese/Premissa** (aquilo que assumimos como verdade inicial) e **`B`** é a nossa **Tese/Conclusão** (o destino, onde queremos chegar).

### Comparativo de Formas de Demonstração

|                                    | 🎯 Forma Direta | 🔄 Forma Indireta (Absurdo)  |
| :--------------------------------- | :-------------: | :--------------------------: |
| **Hipótese** (Ponto de partida)    |       `A`       |           `A ∧ ¬B`           |
| **Tese** (Onde queremos chegar)    |       `B`       | `C ∧ ¬C` *(Uma contradição)* |
| **Demonstração** (Processo lógico) |     `A ⊢ B`     |    `(A ∧ ¬B) ⊢ (C ∧ ¬C)`     |
