# Usar parâmetros de consulta para personalizar respostas
<a id="use-query-parameters-to-customize-responses" class="xliff"></a>

O Microsoft Graph fornece parâmetros de consulta opcional que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. Há suporte para os seguintes parâmetros de consulta.

|Name|Descrição|Exemplo (clique nos exemplos para experimentar no [Explorador do Graph][graph-explorer])
|:---------------|:--------|:-------|
|[$filter](#filter)|Filtra os resultados (linhas).|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)
|[$select](#select)|Filtra as propriedades (colunas).|[`/users?$select=givenName,surname`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)
|[$expand](#expand)|Recupera os recursos relacionados.|[`/groups/{id}?$expand=members`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/22be6ccb-15a5-459f-94ac-d1393bdd9e66?$expand=members&method=GET&version=v1.0)
|[$orderby](#orderby)|Ordena os resultados.|[`/users?$orderby=displayName,userPrincipalName desc`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$orderby=displayName,userPrincipalName%20DESC&method=GET&version=v1.0)
|[$top](#top)|Limita os resultados. Normalmente é usado com `$skipToken`.|[`/users?$top=2`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)
|[$skipToken](#skiptoken)|Usado com `$top` para recuperar uma página de resultados.|Confira `nextLink` da consulta $top para obter um exemplo.
|[$count](#count)|Recupera a contagem total de recursos correspondentes.|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)
<!-- TODO: figure out whether $search is actually used
|[`$search`](#search)|A property and value pair separated by a colon.|
-->

Esses parâmetros são compatíveis com a [linguagem de consulta OData V4][odata-query].

> **Observação:** No ponto de extremidade `beta`, o prefixo `$` é opcional. Por exemplo, em vez de `$filter`, você pode usar `filter`. Para obter mais detalhes e exemplos, confira [Suporte a parâmetros da consulta sem prefixos $ no Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).

**Codificação de parâmetros da consulta:**

Os valores dos parâmetros da consulta devem ser codificados por porcentagem. Muitas ferramentas, navegadores e clientes HTTP (por exemplo, o [Explorador do Graph][graph-explorer]) vão ajudar você com isso. Se uma consulta está falhando, um motivo possível é a falha na codificação adequada dos valores dos parâmetros da consulta.

Uma URL descodificada é semelhante a esta:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

Uma URL codificada adequadamente é semelhante a esta:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## filtro
<a id="filter" class="xliff"></a>

`$filter` pode ser usado para recuperar apenas um subconjunto de uma coleção. Por exemplo, para encontrar usuários cujo nome de exibição comece com `J`, use `startswith`.

[Experimentar no Explorador do Graph](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)

**Solicitação:**

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

**Resposta:**

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users",
    "value": [
        {
            "id": "e013b9f3-a1ab-48d1-907b-e716c39d6363",
            "businessPhones": [
                "4255550100"
            ],
            "displayName": "Jan Madden",
            "givenName": "Jan",
            "jobTitle": null,
            "mail": "demo32@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": null,
            "preferredLanguage": null,
            "surname": "Madden",
            "userPrincipalName": "demo32@a830edad9050849NDA1.onmicrosoft.com"
        },
        {
            "id": "89efe8ed-d141-4151-a3e4-570a70022dff",
            "businessPhones": [
                "+1 425 555 0109"
            ],
            "displayName": "Janet Schorr",
            "givenName": "Janet",
            "jobTitle": "Product Marketing Manager",
            "mail": "janets@a830edad9050849NDA1.onmicrosoft.com",
            "mobilePhone": null,
            "officeLocation": "18/2111",
            "preferredLanguage": null,
            "surname": "Schorr",
            "userPrincipalName": "janets@a830edad9050849NDA1.onmicrosoft.com"
        },
        ...
    ]
}
```

`$filter` tem uma sintaxe muito rica e expressiva com muitos operadores internos. Os operadores lógicos incluem é igual a (`eq`), não é igual a (`ne`), maior (`gt`), maior ou igual a (`gte`), e (`and`), ou (`or`), não (`not`) etc. Os operadores aritméticos incluem somar (`add`), subtrair (`sub`) etc. Os operadores de cadeia de caracteres incluem contém (`contains`), começa com (`startswith`) etc. Os operadores lambda incluem qualquer (`any`) e tudo (`all`). Para obter outros detalhes sobre a sintaxe `$filter`, veja o [protocolo OData][odata-filter].


## select
<a id="select" class="xliff"></a>

Em uma coleção ou uma entidade individual, para especificar um conjunto diferente de propriedades para retornar em vez do conjunto padrão, use o parâmetro de consulta `$select`. O parâmetro `$select` permite escolher um subconjunto ou superconjunto do conjunto padrão retornado. Por exemplo, ao recuperar suas mensagens, selecione que apenas as propriedades `from` e `subject` das mensagens sejam retornadas.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<!--For example, when retrieving the children of an item on a drive, you want to select that only the `name` and `size` properties of items are returned.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name,size
```

By submitting the request with the `$select=name,size` query string, the objects
in the response will only have those property values included.

```json
{
  "value": [
    {
      "id": "13140a9sd9aba",
      "name": "Documents",
      "size": 1024
    },
    {
      "id": "123901909124a",
      "name": "Pictures",
      "size": 1012010210
    }
  ]
}
```-->

## expandir
<a id="expand" class="xliff"></a>

Em solicitações da API do Microsoft Graph, as navegações para um objeto ou coleção do item referenciado não são expandidas automaticamente. Isso ocorre por design porque reduz o tráfego de rede e o tempo necessário para gerar uma resposta do serviço. No entanto, em alguns casos pode ser ideal incluir esses resultados em uma resposta.

Você pode usar o parâmetro da cadeia de caracteres de consulta `$expand` para instruir a API a expandir uma coleção ou objeto filho e incluir os resultados.

Por exemplo, para recuperar as informações da unidade raiz e os itens filho de nível superior em uma unidade, use o parâmetro `$expand`. Esse exemplo também usa uma instrução [`$select`](#select) para retornar apenas as propriedades `id` e `name` dos itens filhos.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> **Observação:** o número máximo de objetos expandidos em uma solicitação é 20. Além disso, se você consultar no recurso [`user`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user), é possível usar `$expand` para obter as propriedades de apenas uma coleção ou objeto filho de cada vez. O exemplo a seguir obtém objetos `user`, cada um com até 20 objetos `directReport` na coleção `directReports` expandida:

```http
GET https://graph.microsoft.com/v1.0/users?$expand=directReports
```

Alguns outros recursos também podem ter um limite, portanto, verifique sempre possíveis erros.

## orderby
<a id="orderby" class="xliff"></a>

Para especificar a ordem de classificação de itens retornados da API do Microsoft Graph, use o parâmetro de consulta `$orderby`.

Por exemplo, para retornar os usuários na organização classificados por seu nome de exibição, a sintaxe é a seguinte:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

Você também pode classificar por entidades de tipo complexo. O exemplo abaixo obtém mensagens e as classifica pelo campo `address` da propriedade `from`, que é do tipo complexo `emailAddress`:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.

 > **Observação:** Se você consultar o recurso [`user`](../api-reference/v1.0/resources/user.md), `$orderby` não poderá ser combinado com expressões de filtro.

## top
<a id="top" class="xliff"></a>

Para especificar o número máximo de itens para retornar em um conjunto de resultados, use o parâmetro de consulta `$top`. O parâmetro de consulta `$top` identifica um subconjunto na coleção. Esse subconjunto é formado selecionando-se apenas os primeiros N itens do conjunto, em que N é um inteiro positivo especificado por esse parâmetro de consulta. Por exemplo, para retornar as cinco primeiras mensagens na caixa de correio do usuário, a sintaxe é a seguinte:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

## ignorar
<a id="skip" class="xliff"></a>

Para definir o número de itens que devem ser ignorados antes de recuperar itens em uma coleção, use o parâmetro de consulta `$skip`. Por exemplo, para retornar eventos classificados por data de criação e começando do 21º evento, a sintaxe é a seguinte:

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```

## skipToken
<a id="skiptoken" class="xliff"></a>

Para solicitar a segunda página e as páginas subsequentes dos dados do Graph use o parâmetro de consulta `$skipToken`. O parâmetro de consulta `$skipToken` é fornecido em Urls retornados do Graph quando o Graph retorna um subconjunto parcial de resultados, normalmente devido à paginação do servidor. Ela identifica o ponto em uma coleção onde o servidor terminou de enviar resultados e volta para o Graph para indicar de onde ele deve recomeçar o envio dos resultados. Por exemplo, o valor de um parâmetro de consulta `$skipToken` poderia identificar o décimo item em uma coleção ou o vigésimo item em uma coleção com 50 itens, ou qualquer outra posição nela.

Em algumas respostas, você verá o valor `@odata.nextLink`. Algumas incluem um valor `$skipToken`. O valor `$skipToken` é como um marcador que informa ao serviço onde retomar no próximo conjunto de resultados. A seguir está um exemplo de um valor `@odata.nextLink` de uma resposta em que os usuários foram solicitados ordenados por `displayName`:

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27"
```

Para retornar para a próxima página de usuários em sua organização, a sintaxe é a seguinte.

```http
GET  https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27
```

## count
<a id="count" class="xliff"></a>

Use `$count` como um parâmetro de consulta para incluir uma contagem do número total de itens em uma coleção junto com a página de valores de dados retornados do Graph, como no exemplo a seguir:

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

Isso retornaria ambas as coleções `contacts` e o número de itens na coleção `contacts` na propriedade `@odata.count`.

>**Observação:** Isso não tem suporte das coleções [`directoryObject`](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/directoryobject).

## pesquisar
<a id="search" class="xliff"></a>

Para restringir os resultados de uma solicitação que correspondam a um critério de pesquisa, use o parâmetro de consulta `$search`.

> **Observação:** Atualmente, é possível pesquisar **somente** coleções de [mensagens](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/message) e [pessoas](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/person). Uma solicitação de `$search` retorna até 250 resultados. Não é possível usar [`$filter`](#filter) ou [`$orderby`](#orderby) em uma solicitação de pesquisa.

Os critérios de pesquisa são expressos usando a sintaxe de consulta avançada (AQS). Os resultados são classificados pela data e hora em que a mensagem foi enviada.

Você pode especificar as seguintes propriedades em uma `message` em um critério `$search`: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`,`toRecipients`

Se você realizar uma pesquisa em mensagens e especificar apenas um valor, a pesquisa será realizada nas propriedades de pesquisa padrão `from`, `subject` e `body`.

O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

O próximo exemplo procura todas as mensagens na Caixa de Entrada do usuário que foram enviadas de um endereço de email específico:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
