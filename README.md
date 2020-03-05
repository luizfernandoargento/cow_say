# README

Execute o server
$ rails server

Abra outro terminal e digite

$ curl localhost:3000/say -H 'Content-Type: application/json' -d '{"message": "Hello from RapidAPI"}'
| ruby -r json -e "print JSON.parse(STDIN.read)['message']"

Aqui estamos canalizando a saída do nosso comando curl para o ruby, onde exigimos o módulo json e o usamos para analisar a resposta, pegar a propriedade e imprimi-la, o que garante que a resposta seja apresentada corretamente. Agora você deve ver uma vaca dizendo sua frase:

"Hello from RapidAPI"
