# Strategy

![diagramaClasses](https://github.com/ritahecht/bertoti/assets/89950512/3826a286-8c05-470b-9dd1-9e0d81bc7c10)

>Código



```java

Classe Funcionário

public class Funcionario {

	private Cadastro cadastro; 
	
	public void setCadastro(Cadastro cadastro){//argumento polimorfico
		this.cadastro = cadastro;
	}
	
	public void Cadastrar() {
		this.cadastro.cadastrar();
	}
	
}
```
```java

Classe Cadastrar

public interface Cadstro {

	public void cadastrar();
	
}
```
```java
Classe Assistente Administrativo


public class AssistenteAdministrativo implements Cadastro{

	public void cadastrar() {
		
		System.out.println("Assistente Administrativo");
		
	}
	
}
```
```java
Classe Projetista


public class Projetista implements Cadastro{

	public void cadastrar() {
		
		System.out.println("Projetista");
		
	}
	
}
```
```java
Classe Montador


public class Montador implements Cadastro{

	public void cadastrar() {
		
		System.out.println("Montador");
		
	}
	
}
```
