Perfeito, Daniel 😎
Aqui está um **README.md** completo e bem formatado para o seu repositório desse projeto de **Árvore Binária de Busca (BST)** em Java:

---

# 🌳 Árvore Binária de Busca (Binary Search Tree - BST)

Este projeto implementa uma **Árvore Binária de Busca (BST)** em Java, com funcionalidades para **inserção de valores**, **exibição em diferentes formatos**, **cálculo de altura**, **exibição de folhas** e **construção automática a partir de um RA (Registro Acadêmico)**.

---

## 🧩 Estrutura do Projeto

O código é dividido em três classes principais:

### 🔹 `No`

Representa cada **nó** da árvore binária.

```java
class No {
    int valor;
    No esquerda, direita;

    public No(int valor) {
        this.valor = valor;
        esquerda = direita = null;
    }
}
```

---

### 🔹 `ArvoreBinariaDeBusca`

Classe responsável por toda a **lógica da BST**, incluindo inserções, percursos e exibição.

Principais métodos:

* `inserir(int valor)` → adiciona um novo valor na árvore sem permitir duplicados.
* `emOrdem()` → exibe os valores em **ordem crescente**.
* `exibirArvoreEmPe()` → imprime a árvore **de forma vertical**, como um diagrama.
* `altura(No no)` → calcula a **altura da árvore**.
* `exibirFolhas(No no)` → mostra apenas os **nós folha** (sem filhos).
* `construirComRA(String ra)` → cria automaticamente a árvore a partir dos **números de um RA**.

---

### 🔹 `Main`

Classe principal que demonstra o uso da árvore.
O código constrói uma árvore com base no **RA de exemplo** e exibe as informações principais.

```java
public class Main {
    public static void main(String[] args) {
        ArvoreBinariaDeBusca bst = new ArvoreBinariaDeBusca();

        // RA de exemplo (Daniel)
        String ra = "2403844";

        bst.construirComRA(ra);

        System.out.println("\n=== Árvore Binária de Busca (BST) ===");
        System.out.println("Raiz: " + bst.raiz.valor);

        System.out.print("Folhas: ");
        bst.exibirFolhas(bst.raiz);
        System.out.println();

        System.out.println("Altura da árvore: " + bst.altura(bst.raiz));
        bst.emOrdem();

        bst.exibirArvoreEmPe();
    }
}
```

---

## 🧠 Exemplo de Saída

Ao executar o programa com o RA `"2403844"`, a saída será semelhante a:

```
RA usado: 2403844

=== Árvore Binária de Busca (BST) ===
Raiz: 2
Folhas: 0 4 8 
Altura da árvore: 4

Percurso em ordem (ordenado): 0 2 3 4 8 

=== Estrutura da Árvore (Vertical) ===
└── 2
    ├── 0
    └── 4
        ├── 3
        └── 8
```

---

## ⚙️ Como Executar

1. Certifique-se de ter o **Java JDK** instalado (versão 8+).
2. Salve o código em um arquivo chamado `Main.java`.
3. Compile e execute no terminal:

```bash
javac Main.java
java Main
```

---

## 💡 Conceitos Envolvidos

* Estruturas de Dados: Árvores Binárias de Busca
* Recursão
* Percursos em ordem
* Cálculo de altura
* Impressão hierárquica de dados

---

## ✍️ Autor

**Daniel Fernandes Santos**
🎓 Estudante de Ciências da Computação
💻 Foco em Backend e apaixonado por lógica de programação.

---

Quer que eu adicione um campo de **licença** (por exemplo, MIT) e uma **seção “Próximos Passos”** (como balanceamento AVL, remoção de nós etc.) no final para deixar o README mais profissional?
