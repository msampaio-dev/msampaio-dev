# Marcelo Sampaio

Sou desenvolvedor backend Java e procuro uma vaga júnior, em backend ou full stack.

Trabalho principalmente com Java e Spring Boot, e uso React quando o projeto precisa de uma interface. Gosto de sistemas com regras que não podem falhar. No meu projeto principal, dois clientes nunca conseguem reservar o mesmo horário, nem clicando no mesmo instante.

## Projeto em destaque: AgendaPro

![Demonstração do AgendaPro: escolha da barbearia, do profissional, do serviço e do horário, até a confirmação](https://raw.githubusercontent.com/msampaio-dev/AgendaPro/main/docs/screenshots/agendamento.gif)

O AgendaPro é uma plataforma de agendamento para barbearias, publicada e funcionando. Você pode [testar a demonstração](https://agenda-pro-web-agendapro2.vercel.app/) sem se cadastrar: na tela de login tem um botão para entrar com uma conta de teste.

A API é em Java 21 e Spring Boot, com PostgreSQL, Flyway e mais de 160 testes. Um deles dispara duas reservas ao mesmo tempo contra um banco real e confirma que só uma passa. O frontend é em React e TypeScript, com testes de componente e testes ponta a ponta no computador e no celular.

O sistema roda no Render, na Vercel e no Neon. Quando a API ficou lenta, medi antes de mexer e descobri que o banco estava em outro continente. Depois de mudar a região, cada consulta caiu de 320 ms para 4 ms.

[Código da API](https://github.com/msampaio-dev/AgendaPro) · [Código do frontend](https://github.com/msampaio-dev/AgendaPro-Web) · [Demonstração](https://agenda-pro-web-agendapro2.vercel.app/)

## Como eu trabalho

Escrevo teste antes de dizer que algo está pronto. Nas mensagens de commit, registro por que tomei cada decisão, então o histórico dos meus projetos mostra o que eu pensei, inclusive os erros e como corrigi.

## Ferramentas

Java · Spring Boot · Spring Security · JPA/Hibernate · PostgreSQL · Flyway · JUnit · Mockito · Testcontainers · Docker · React · TypeScript · Vitest · Playwright · GitHub Actions

## Contato

[LinkedIn](https://www.linkedin.com/in/marcelo-sampaio-8a23b0439/) · [marcelosampaio.dev@gmail.com](mailto:marcelosampaio.dev@gmail.com)
