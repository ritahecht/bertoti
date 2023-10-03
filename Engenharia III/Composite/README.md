Composit

![composit](https://github.com/ritahecht/bertoti/assets/89950512/27acc4ac-c102-45b7-ab52-785546b13609)

> Código

#  Classe Compras
```java
import java.util.ArrayList;
import java.util.List;

public class Compras implements Produto {
  private List<Produto> Produto;
  private double valorTotal;

  public Compras() {
    this.produto= new ArrayList<>();
    this.valorTotal = 0.00;
  }

  public void comprar() {
    System.out.println("Valor da sua compra R$"+this.valorTotal);
  }

   public double getValorTotal(){
    return this.valorTotal;
  }

  public void addProduto(Produto produto) {
    produto.add(produto);
    this.valorTotal += produto.getValorTotal();
  }

  public void delProduto(Produto produto) {
    produto.remove(produto);
    this.valorTotal -= produto.getValorTotal();
  }

  public List<Produto> getProduto() {
    return produto;
  }
}
```

# Interface Produto

```java

public interface Produto {
     void comprar()
    double getValorProduto();
}

```
# Classe Refrigerante

```java

public class Refrigerante {
    private String nome;
    private char tamanho;
    private Double valor;

    public Produto(String nome, char tamanho, Double valor) {
        this.nome = nome;
        this.tamanho = tamanho;
        this.valor = valor;
    }

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public char getTamanho() {
        return tamanho;
    }

    public void setTamanho(char tamanho) {
        this.tamanho = tamanho;
    }

    public Double getValor() {
        return valor;
    }

    public void setValor(Double valor) {
        this.valor = valor;
    }
}


```
# Classe Hamburguer

```java
public class Hamburguer {
    private String nome;
    private char tamanho;
    private Double valor;

    public Produto(String nome, char tamanho, Double valor) {
        this.nome = nome;
        this.tamanho = tamanho;
        this.valor = valor;
    }

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public char getTamanho() {
        return tamanho;
    }

    public void setTamanho(char tamanho) {
        this.tamanho = tamanho;
    }

    public Double getValor() {
        return valor;
    }

    public void setValor(Double valor) {
        this.valor = valor;
    }
}


```









