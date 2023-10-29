Façade


![facade drawio (1)](https://github.com/ritahecht/bertoti/assets/89950512/fe690ccf-fbb2-4079-90e7-fc66c08cbcc2)

Código


```java

public class ClienteBanco {
    private String nome;

    public String lerNomeCliente(){
        return this.nome;
    }

    public ClienteBanco(){}

    public ClienteBanco (String nome){
        this.nome = nome;
    }

}

```
```java

#Classe Conta

public class Conta {
    private String conta;
    private double saldo;

    public double depositar(double valor){
        System.out.println("Depositando...");
        return this.setSaldo(this.getSaldo() + valor);
    }

    public String lerNumConta(){
        System.out.println("Obtendo número de conta...");
        return this.conta;
    }

    public double lerSaldo(){
        System.out.println("Obtendo saldo...");
        return this.getSaldo();
    }

    public Conta(){}

    public Conta(String conta){
        this.conta = conta;
    }

    public double getSaldo() {
        return saldo;
    }

    public double setSaldo(double saldo) {
        this.saldo = saldo;
        return saldo;
    }
}

```
```java

#Aplicação Cliente

public class AplicacaoCliente {

    public static void main(String[] args) {
        ClienteBanco cliente = new ClienteBanco("Rita Priante");
        Conta conta = new Conta("15983-7");

        Fachada facade = new Fachada();
        facade.fazerDeposito(250, cliente, conta);
    }
}
```
```java

#Classe Facade

public class Fachada {
    private ClienteDoBanco cliente;
    private ContaBancaria conta;

    public Fachada() {
        this.cliente = new ClienteBanco();
        this.conta = new Conta();
    }

    public void fazerDeposito(int quantidade, ClienteBanco cliente, ContaBancaria conta){
        System.out.printf("Olá, o beneficiário de seu depósito é o(a) cliente %s\n",cliente.lerNomeCliente());
        System.out.printf("Você escolheu a conta %s\n", conta.lerNumConta());
        System.out.printf("O saldo desta conta é: %d\n", conta.lerSaldo());
        System.out.printf("Você está depositando R$ %s\n", quantidade);
        conta.setSaldo(conta.getSaldo() + quantidade);
        System.out.printf("Depositado R$ %d na conta de %s\n",quantidade, cliente.lerCliente());
        System.out.printf("O saldo desta conta é: R$ %s\n", conta.lerSaldo());
    }

    public ClienteDoBanco getCliente() {
        return cliente;
    }

    public void setCliente(ClienteBanco cliente) {
        this.cliente = cliente;
    }

    public ContaBancaria getConta() {
        return conta;
    }

    public void setConta(ContaBancaria conta) {
        this.conta = conta;
    }
}

```





