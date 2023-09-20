Composit

![composit](https://github.com/ritahecht/bertoti/assets/89950512/27acc4ac-c102-45b7-ab52-785546b13609)

> Código

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


```java


```
```java

```

```java

```









