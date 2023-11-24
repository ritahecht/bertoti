Observer

![observer drawio](https://github.com/ritahecht/bertoti/assets/89950512/be6a2471-6103-43f7-b9c8-5f7ae53135ed)

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

public void addObserver(Observer observer){
    this.observers.add(observer);
    }	

public void setEmpresa (String ){
    this.empresa = nome
    }

public void notify(String){
    this.observers.stream().forEach(item -> {
           item.update(nome) ;
	});
    }
```
```java
Classe Assistente Administrativo

public class AssistenteAdministrativo implements Observer {

    public void update(String ){
        System.out.println("Registro de funçao do funcionário: " +evento);
    }
}
```

```java
Classe Projetista

public class Projetista implements Observer {

    public void update(String ){
        System.out.println("Registro de funçao do funcionário: " +evento);
    }
}
```









