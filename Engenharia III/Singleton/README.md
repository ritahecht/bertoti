Singleton

![singleton drawio](https://github.com/ritahecht/bertoti/assets/89950512/6e3355a5-441d-4f1a-8617-145be4c8e576)

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
