# Marcelo Sampaio

Sou desenvolvedor backend Java e estudo Engenharia de Software. Procuro minha primeira vaga em backend ou full stack.

Trabalho principalmente com Java e Spring Boot, e uso React com TypeScript quando o projeto precisa de uma interface. Gosto de sistemas com regras que não podem falhar. No meu projeto principal, dois clientes nunca conseguem reservar o mesmo horário, nem clicando no mesmo instante.

## AgendaPro

![Demonstração do AgendaPro: escolha da barbearia, do profissional, do serviço e do horário, até a confirmação](https://raw.githubusercontent.com/msampaio-dev/AgendaPro/main/docs/screenshots/agendamento.gif)

O AgendaPro é uma plataforma de agendamento para barbearias, publicada e funcionando. Dá para [testar a demonstração](https://agenda-pro-web-agendapro2.vercel.app/) sem se cadastrar: na tela de login tem um botão que entra com uma conta de teste.

A API é em Java 21 e Spring Boot, com PostgreSQL, Flyway e mais de 160 testes. Um deles dispara duas reservas ao mesmo tempo contra um banco real e confirma que só uma passa. O frontend é em React e TypeScript, com testes de componente e testes ponta a ponta no computador e no celular.

O sistema roda no Render, na Vercel e no Neon, e já me deu problemas de produção para resolver. As fotos sumiam a cada deploy porque o disco do servidor era apagado, então passei a guardá-las no banco. Quando a API ficou lenta, medi antes de mexer e descobri que o banco estava em outro continente. Depois de mudar a região, cada consulta caiu de 320 ms para 4 ms.

[Código da API](https://github.com/msampaio-dev/AgendaPro) · [Código do frontend](https://github.com/msampaio-dev/AgendaPro-Web) · [Demonstração](https://agenda-pro-web-agendapro2.vercel.app/)

## PedeJá

Uma versão simplificada do iFood, com backend em Java e Spring Boot e frontend em React. O cliente paga com Pix, e o gateway confirma o pagamento por um webhook assinado. Se o mesmo aviso chegar duas vezes, o pedido muda uma vez só.

Cada mudança de status é gravada no banco antes de ir para o RabbitMQ, no padrão outbox, então nada se perde se o broker cair. O restaurante vê o pedido pago aparecer na tela sem recarregar a página. Os 52 testes do backend rodam com PostgreSQL e RabbitMQ de verdade, em containers.

[Código do PedeJá](https://github.com/msampaio-dev/PedeJa)

## Como eu trabalho

Antes de corrigir um bug, procuro a causa, e só digo que algo está pronto quando um teste confirma. Uso Claude Code e Codex para ganhar produtividade, e leio, questiono e testo o que eles geram antes de integrar. Nas mensagens de commit, registro por que tomei cada decisão, então o histórico dos meus projetos mostra o que eu pensei, inclusive os erros e como corrigi.

Agora estou estudando AWS para a certificação Cloud Practitioner e fazendo um app em React Native para o AgendaPro.

## Ferramentas

Backend: Java, Spring Boot, Spring Security, JPA/Hibernate, PostgreSQL, Flyway e RabbitMQ

Frontend: React e TypeScript

Testes: JUnit, Mockito, Testcontainers, Vitest e Playwright

Entrega: Docker e GitHub Actions

## Contato

[LinkedIn](https://www.linkedin.com/in/marcelo-sampaio-8a23b0439/) · [marcelosampaio.dev@gmail.com](mailto:marcelosampaio.dev@gmail.com)
