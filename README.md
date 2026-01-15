# 📚 Dia 1: Pesquisa Binária (Binary Search)

**Livro:** Entendendo Algoritmos (Aditya Y. Bhargava)
**Status:** ✅ Concluído

## 🔍 O que é?
A Pesquisa Binária é um algoritmo eficiente para encontrar um item em uma **lista ordenada**. Diferente da pesquisa simples (que verifica um por um), a binária elimina **metade** das possibilidades a cada tentativa.

---

## 🧠 Como funciona (A Lógica)

Imagine que buscamos o número **3** em uma lista `[1, 3, 5, 7, 9]`.

1.  **Define limites:** Começamos olhando a lista inteira (Baixo=0, Alto=4).
2.  **Chute no Meio:** O meio é o número 5.
3.  **Analisa:**
    * 5 é igual a 3? ❌ Não.
    * 5 é maior que 3? ✅ Sim (Chute foi alto).
4.  **Corta:** Ignoramos tudo do 5 para cima. Nova busca apenas entre `[1, 3]`.
5.  **Repete:** Novo meio é 3. Achou! 🏆

### 📉 Comparativo de Desempenho
Para uma lista de **240.000** itens:
* 🐢 **Pesquisa Simples:** Pode levar até 240.000 etapas.
* 🐇 **Pesquisa Binária:** Leva no máximo **18 etapas** ($\log_2 n$).

---



## 🐍 Código
Veja o arquivo `pesquisa_binaria.py` neste repositório para a implementação prática.