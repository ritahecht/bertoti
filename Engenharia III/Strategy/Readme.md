# Strategy

![strategy drawio](https://github.com/ritahecht/bertoti/assets/89950512/5c2701c1-28f8-4625-8a63-5a08cf85b706)

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
