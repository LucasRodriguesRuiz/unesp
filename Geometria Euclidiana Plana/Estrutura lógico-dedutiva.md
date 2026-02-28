Princípios da lógica clássica:

| Principio                   | Representação |
| --------------------------- | :-----------: |
| Não Contradição             |    ¬(A∧¬A)    |
| 3ª excluído                 |     A∨¬A      |
| Reflexividade da Identidade |   (∀x)(x=x)   |

## Conectivos Lógicos (Operadores):

| Símbolo | Significado |
| :-----: | :---------: |
|    ¬    |     Não     |
|    ∧    |      E      |
|    ∨    |     Ou      |
|    →    |  Se, Então  |

# Sistema Axiomático
Axiomas são verdade aceitas em um certo cenário.
## Axiomas do Calculo Proporcional Clássico

|       Axioma        |          Nome          |
| :-----------------: | :--------------------: |
|       A→(B→A)       |   **Monotonicidade**   |
| ((A→B)∧(B→C))→(A→C) |   **Trasitividade**    |
| ((¬A→¬B)∧(¬A→B))→A  | **Redução ao Absurdo** |
## Regra de inferência "Modus Ponens"
A→B, A⊢B

> [!NOTE] Nota
> Calculo proporcional clássico (**CPC**) também podem ser conhecidos como Lógica proporcional clássica (**LPC**)


# Fato Matemático
Axiomas e Postulados são demonstrados por si próprios.
Fatos matemáticos devem ser demonstrados.

- Preposição
	- Fato simplório
- Lema
	- Fato usado para demonstrar um Teorema
- Teorema
	- Fato importante para a teoria
- Corolário
	- Fato demonstrado a partir de outro fato já demonstrado

## Técnicas de demonstração

Se **A**, então **B**
Aonde **A** é a nossa hipótese/premissa e **B** é nossa tese/conclusão.

|              | Forma Direta | Forma Indireta |
| ------------ | :----------: | :------------: |
| Hipótese     |      A       |      A∧¬B      |
| Tese         |      B       |      C∧¬C      |
| Demonstração |     A⊢B      | (A∧¬B)⊢(C∧¬C)  |
