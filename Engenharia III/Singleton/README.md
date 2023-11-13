Singleton

![singlton drawio](https://github.com/ritahecht/bertoti/assets/89950512/14a41c20-40cd-41dc-835c-87f23ecb2f8e)

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
