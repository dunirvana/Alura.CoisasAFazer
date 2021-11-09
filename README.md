# Alura.CoisasAFazer
Revisando testes de integração

## Testes de integração
- conceito de testes de integração, injeção de dependência e inversão de controle
- principal estratégia para aplicar injeção de dependência em suas classes, que é através de argumentos no construtor
- criar objetos leves que simulam recursos caros e lentos como por exemplo um banco de dados

## Dependências mais leves e mais rápidas
- o EF Core disponibiliza uma estratégia para realizar testes que dependam de banco de dados;
- criar massas de dados que materializem cenários complexos e ao mesmo tempo garantem testes isolados e independentes;
- repositório fake;
- testes com classes de produção, com uma configuração específica para usar o InMemoryDatabase;
- padrão **dummy object**;
- padrão **fake object**;

## Injetando dados em cenários complexos
- o que fazer quando seus cenários de testes exigem recursos que injetem informações específicas, exceções ou falhas;
- o framework Moq;
- padrão **Stub** (injetar informações específicas nos cenários de testes);

## Testando comportamentos do sistema
- usar bibiloteca Moq para testar comportamento;
- padrão **Mock**;

## Verificando efeitos colaterais
- testar se determinada ação gerou um determinado resultado indireto no nosso sistema (como geração de log);
- padrão **Spy** (com o framework Moq);

## Aplicando em controladores AspNet Core
- testes em método que representa um endpoint de uma API AspNet Core;
