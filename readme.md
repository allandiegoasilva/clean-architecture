
### O que é arquitetura de software? 

Resumidamente, a arquitetura de software é definir como todos os componentes dentro de uma aplicação vão se comunicar.
Separar o software em camadas proporciona algumas vantagens como: **desempenho, escalabilidade, interoperabilidade
compatibilidade e performace.**

### Alguns modelos de arquitetura de software

- Clean Architecture ***(essa que está sendo utilizada neste projeto)***
- Domain driven design 
- Hexagonal Architecture ou Ports and Adapters 

### Clean Architecture

A `clean architucture` é a forma em que vamos estruturas as camadas do software dentro da aplicação. 
O objetivo principal é eliminar o máximo de dependências dentro do código e ampliar o escopo de 
testes idependentes para agilizar no desenvolvimento. A seguir uma imagem que representa o `clean architecture`
de uma forma simples, onde fatores externos depende de entidades internas porém uma entidade interna nunca poderá
depender de uma externa. 

![alt text](/images/CleanArchitecture.jpg)



##### Entidades
*As entidades encapsulam as regras de negócios de toda a empresa. Uma entidade pode ser um objeto com métodos, ou pode ser um conjunto de estruturas de dados e funções. Não importa, desde que as entidades possam ser usadas por muitos aplicativos diferentes na empresa.* - Robert C. Martin 

#### Casos de uso 
*O software nesta camada contém regras de negócios específicas do aplicativo . Ele encapsula e implementa todos os casos de uso do sistema. Esses casos de uso orquestram o fluxo de dados de e para as entidades e direcionam essas entidades a usar suas regras de negócios em toda a empresa para atingir as metas do caso de uso.* - Robert C. Martin 

**Complemento:** Repare que nesta situação o caso de uso pode depender de uma entidade porém não pode acontecer vice 
versa. 

#### Adaptadores de interface 
A camada de `adaptadores de interface` é um conjunto de `interface` (contratos). (continuar...)



### Caso de uso desta aplicação

Existe um concessionária de veículos que além de vender veículos por um preço x ela também 
pode alugar o veículo. Um veículo pode ser alugado e vendido, no momento em que está 
alugado então ele não poderá ser vendido enquanto seja devolvido em boas condições.
Todo aluguel e compra tem um vendedor e um comprador onde precisa ser armazenado seus dados, os 
dados obrigatórios para cada um é nome e CPF, para o veículo: ano, modelo, marca, tipo, data de devolução etc...


### Referência

- [Entenda CLEAN ARCHITECTURE de uma vez por todas!](https://www.youtube.com/watch?v=HynTfTli4mw)
- [The Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)
- [Descompmlicando a clean architecture](https://medium.com/luizalabs/descomplicando-a-clean-architecture-cf4dfc4a1ac6)