Singleton

![Diagrama sem nome drawio](https://github.com/ritahecht/bertoti/assets/89950512/30060288-9632-4d13-a794-2d0754a3a04b)

> Código

```java

public static class Bilhete {
	private static Ingresso Bilhete;
	private Bilhete(){}
	public void Ingresso getInstance(){
		if(bilhete==null){
			bilhete = new Bilhete;
		}
		return bilhete;
	}

	public comprar(String documento) {
        System.out.println("Comprando: " + documento);
    }
}

```