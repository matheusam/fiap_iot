# Aula 10 - APIs e requests http.

## Conteúdo

Atualmente com essa onda de micro-serviços é impossivel não se falar de API's REST. Quando criamos uma comunicação por protocolo HTTP isso nos traz muitas vantagens, como por exemplo saber que todas nossas aplicações vão seguir um padrão para se comunicar, isso também facilita para ter um ambiente com muitas linguagens diferentes.
Quando falamos de requisições HTTP, tudo é baseado em algumas RFC's, como a [RFC7231](https://tools.ietf.org/html/rfc7231). Para definir o padrão de comunicação foi criado uma coisa chamada verbos, verbos nos dizem qual tipo de ação está sendo feita.
Você provavelmente já ouviu falar do GET ou POST, porém temos vários outros verbos também, mas os principais são:

* GET - Verbo usado para requisitar um recurso

* POST - Verbo usado para enviar um recurso

* DELETE - Verbo usado para apagar um recurso

* PUT - Verbo usado para editar vários atributos de um recurso de uma vez

* PATCH - Verbo usado para editar apenas um atributo de um recurso

Agora que entendemos os verbos temos que entender um pouco sobre endpoints, eles são caminhos na nossa aplicação e cada caminho tem um verbo associado a ele. Por exemplo, podemos pegar a posição atual do ISS(International Space Station) fazendo uma requisição GET para http://api.open-notify.org/iss-now.json.

Agora a parte importante, como fazer essas requisições? Caso seja uma requisição GET é só colocar no navegador o link que ele deve funcionar, porém quando usamos outros verbos isso não é possível. Podemos usar o Postman ou o Curl. Para que vocês se habituem melhor eu recomendo fortemente que usem o Curl.

Para fazer uma requisição GET com curl só precisamos fazer:

`curl http://api.open-notify.org/iss-now.json`

Caso queira fazer um POST ficaria algo assim:

`curl -d "name=fulado&senha=123" http://foo.bar/api/v1/user/new`

## Desafio

### User history


### Tasklist

* [ ]