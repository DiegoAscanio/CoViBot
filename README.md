# CoViBot

## Introdução:

Este projeto é uma ferramenta automatizada para auxílio aos órgãos de saúde pública no acompanhamento de prováveis casos do Covid-19.

Segundo questionamento realizado por jornalistas da imprensa brasileira a funcionários do ministério da saúde, descobriu-se que os acompanhamentos de prováveis casos (pessoas que tiveram contato com infectados pela doença) têm sido realizados por humanos através de ligações telefônicas.

Neste sentido, propõe-se a criação de um canal automatizado para realização de tais acompanhamentos, através de chatbots de questionários implementados nos principais apps de mensagens (Telegram, Whatsapp) e questionários telefônicos automatizados (URAs) através de APIs telefônicas como o Twilio.

## Produto Mínimo Viável (MVP):

Sete histórias de usuário (disponíveis no arquivo [historias_de_usuario.pdf](https://github.com/DiegoAscanio/CoViBot/blob/master/historias_de_usuario.pdf)) foram concebidas para construir um MVP do CoViBot. Entretanto, nem tudo que ali está especificado precisa ser desenvolvido.

A metodologia que inicialmente devo utilizar para a construção deste MVP está orientada para utilizar ferramentas que conheço de alguma forma. Entretanto, estou aberto a mudanças, a migrar este projeto para um grupo colaborativo no github e a delegar a tomada de decisões a respeito de tecnologias e implementação da ferramenta para desenvolvedores mais experientes que queiram colaborar com o projeto.

Desta forma, elenco as tecnologias que pretendo usar no desenvolvimento do produto mínimo viável:
- Ambiente de desenvolvimento virtualizado Vagrant (box será disponibilizada)
- GNU/Linux Ubuntu 18.04 LTS server edition.
- Servidor Web Apache2.
- Ambiente Virtual (virtualenv) em python.
- Framework de Desenvolvimento Web Python Django.
- Biblioteca de templates django-bootstrap para o framework Django.
- Fila de tarefas / mensagens assíncronas Python Celery.
- Broker AMQP RabbitMQ (para ser utilizado para troca de mensagens necessárias ao celery).
- Biblioteca de consumo de URLs Python Requests.
- Bot de envio de mensagens do Telegram.
- Controle de versionamento do código através de servidor git hospedado neste site github.
- Bibliotecas de testes pytest e django-pytest para desenvolvimento do produto segundo a metodologia TDD (estou aprendendo agora).
- Instância de produção AWS EC2 com GNU/Linux Ubuntu 18.04 LTS server edition.

## Observações:

Venho da administração de sistemas, não conheço separação de desenvolvimento em backend / frontend, por isso, vou desenvolver tudo acoplado. Entretanto, quero aprender e vou deixar que desenvolvedores que conheçam estas metodologias mudem a arquitetura do sistema se necessário.

Desta forma, como meus conhecimentos em metodologia backend / frontend são escassos e meu conhecimento sobre git é básico, desenvolvedores mais experientes são mais do que bem vindos, são demasiadamente necessários ao projeto! A contribuição é aberta a todos! Quem quiser colaborar, "forke" o repositório ou abra issues aqui emitindo sugestões, dúvidas e relatórios de bugs. Peço que deem star no projeto (para que o github mostre a outros desenvolvedores) e divulguem a possíveis interessados!

