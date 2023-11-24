|nome do padrão|anti-padrão|definição do padrão|problema que ele resolve|Exemplo|
|---|---|---|---|---|
|Strategy |Herança|	encapsula uma familia de algoritmos usando composição e os torna intercambiaveis usando polimorfismo|Encapsulamento      |perguntar qual pessoa tem o sobrenome, em vez de perguntar individualmente o nome completo pra descobrir de qual familia pertence. Outro exemplo Comparable no Java|
|Observer |Alto Acoplamento|Notificar objetos separados, em um mesmo evento/método|utilizamos o polimorfismo mas sem ocorrer o alto-acoplamento|saldo em conta bancária, precisa atualizar o saldo nas contas envolvidas na transação ao mesmo tempo. Outro exemplo é Observable no Java|
|Composite|herança & alto-acoplamento|utilizamos o polimorfismo mas sem ocorrer o alto-acoplamento|Tratar objetos individuais e grupos de objetos de forma uniforme|utilizamos por exemplo no Java Swing, para construir interfaces gráficas|
