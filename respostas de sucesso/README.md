## Respostas de sucesso
```

```

* GET: O recurso foi buscado e transmitido no corpo da mensagem.
* HEAD: Os cabeçalhos da entidade estão no corpo da mensagem.
* PUT ou POST: O recurso descrevendo o resultado da ação é transmitido no corpo da mensagem.
* TRACE: O corpo da mensagem contém a mensagem de requisição recebida pelo servidor.

### 200 OK

Estas requisição foi bem sucedida. O significado do sucesso varia de acordo com o método HTTP:

### 201 Created

A requisição foi bem sucedida e um novo recurso foi criado como resultado. Esta é uma tipica resposta enviada após uma requisição POST.

### 202 Accepted

A requisição foi recebida mas nenhuma ação foi tomada sobre ela. Isto é uma requisição não-comprometedora, o que significa que não há nenhuma maneira no HTTP para enviar uma resposta assíncrona indicando o resultado do processamento da solicitação. Isto é indicado para casos onde outro processo ou servidor lida com a requisição, ou para processamento em lote.

#### 203 Non-Authoritative Information

Esse código de resposta significa que o conjunto de meta-informações retornadas não é o conjunto exato disponível no servidor de origem, mas coletado de uma cópia local ou de terceiros. Exceto essa condição, a resposta de 200 OK deve ser preferida em vez dessa resposta.