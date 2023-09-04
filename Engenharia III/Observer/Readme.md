Observer

![diagramaObs](https://github.com/ritahecht/bertoti/assets/89950512/e2b6e04c-f934-4928-b910-1c9c6a7639d3)

> Código

```java

Classe Observer
 
public interface Observer {
	
	public void update(string);

}
```
```java

import java.util.ArrayList;
import java.util.List;

public class Funcionario {
    private List<Observer> observers = new ArrayList<>();
    private empresa: String

    public Funcionario( ){
        this.observers = new ArrayList<>();
        this.empresa = String
    }		

    public void setEmpresa (String ){
        this.empresa = nome
    }

    public void addObserver(Observer observer){
        this.observers.add(observer);
    }
    public void notify(String){
        this.observers.stream().forEach(item -> {
           item.update(nome) ;
        });
    }

    
}



