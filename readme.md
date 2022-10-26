
#### Clean Architecture

A `clean architucture` é a forma em que vamos estruturas as camadas do software dentro da aplicação. 
O objetivo principal é eliminar o máximo de dependências dentro do código e ampliar o escopo de 
testes idependentes para agilizar no desenvolvimento. A seguir uma imagem que representa o `clean architecture`
de uma forma simples, onde fatores externos depende de entidades internas porém uma entidade interna nunca poderá
depender de uma externa. 

![alt text](/images/CleanArchitecture.jpg)


### Caso de uso desta aplicação

Existe um concessionária de veículos que além de vender veículos por um preço x ela também 
pode alugar o veículo. Um veículo pode ser alugado e vendido, no momento em que está 
alugado então ele não poderá ser vendido enquanto seja devolvido em boas condições.
Todo aluguel e compra tem um vendedor e um comprador onde precisa ser armazenado seus dados, os 
dados obrigatórios para cada um é nome e CPF, para o veículo: ano, modelo, marca, tipo, data de devolução etc...