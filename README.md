# marketplace-payments

Serviço de pagamentos de um marketplace. Recebe pedidos de cobrança, registra a transação e aciona o gateway de pagamento parceiro.

## Stack

- Java 21
- Spring Boot 3.5
- Maven
- MySQL (persistência dos pagamentos)

## Pré-requisitos

- JDK 21
- Maven 3.9+

## Como executar

```bash
mvn spring-boot:run
```

A aplicação sobe na porta `8080`.

## Testes

```bash
mvn verify
```

## Estrutura do projeto

```
src/
  main/
    java/com/marketplace/payments/   código da aplicação
    resources/                       configurações
  test/
    java/com/marketplace/payments/   testes automatizados
.github/workflows/                   pipeline de integração contínua
```

## Fluxo de contribuição

1. Crie uma branch a partir da `main` (`feature/<descrição>` ou `fix/<descrição>`).
2. Faça commits pequenos, seguindo o padrão Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`, `ci:`).
3. Abra um Pull Request para a `main`.
4. O PR precisa de revisão e de CI verde antes do merge.

## Contexto

Projeto acadêmico do módulo de Arquitetura de Software.
