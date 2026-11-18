# Sisdeve Agro — Guia em português

O Sisdeve Agro é um monólito modular para a gestão de fazendas de grãos.

## Situação atual

O projeto está na fase inicial de preparação do backend em Go.
Os cadastros e a persistência serão implementados progressivamente.

## Requisitos

- Go 1.27.4
- Git
- GNU Make

## Executar na raiz do projeto

```bash
make -C back run
make -C back test
make -C back build
```

## Organização planejada

- `back/`: aplicação em Go e automação do desenvolvimento.
- `infra/`: infraestrutura, quando necessária.
- `front/`: aplicação React, após o MVP do backend.

## Princípios

O sistema será um monólito modular, com regras de negócio independentes
do banco utilizado, testes e versionamento com Git Flow.

As mensagens destinadas às pessoas usuárias serão em português brasileiro.