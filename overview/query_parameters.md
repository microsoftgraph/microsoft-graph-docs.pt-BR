# <a name="microsoft-graph-optional-query-parameters"></a>Parâmetros de consulta opcional do Microsoft Graph
O Microsoft Graph fornece vários parâmetros de consulta opcional que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. O Microsoft Graph dá suporte às opções de consulta a seguir. 

|Nome|Valor|Descrição|
|:---------------|:--------|:-------|
|$search|cadeia de caracteres|Um par de propriedade e valor separado por dois-pontos. | 
|$select|cadeia de caracteres|Lista separada por vírgulas de propriedades para incluir na resposta.|
|$expand|cadeia de caracteres|Lista separada por vírgulas de relações para expandir e incluir na resposta.  |
|$orderby|string|Lista separada por vírgula de propriedades que são usadas para classificar a ordem dos itens na coleção de resposta.|
|$filter|string|Filtra a resposta baseado em um conjunto de critérios.|
|$top|int|O número de itens a serem retornados em um conjunto de resultados.|
|$skip|int|O número de itens que devem ser ignorados em um conjunto de resultados.|
|$skipToken|string|Token de paginação usado para obter o conjunto seguinte de resultados.|
|$count|nenhuma|Uma coleção e o número de itens na coleção.|

Esses parâmetros são compatíveis com a [linguagem de consulta OData V4](http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356).

>  **Observação**: No ponto de extremidade **beta** do Microsoft Graph, você pode omitir o prefixo **$** para ter uma experiência mais simples. Por exemplo, em vez de **$expand**, você pode usar **expand**. Para obter mais detalhes e exemplos, confira [Suporte a parâmetros da consulta sem prefixos $ no Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).  

**Codificação de parâmetros da consulta**

- Se você estiver experimentando parâmetros de consulta no [Microsoft Graph Explorer](https://graph.microsoft.io/en-us/graph-explorer#), é possível apenas copiar e colar os exemplos abaixo sem aplicar nenhuma codificação de URL à cadeia de caracteres de consulta. O exemplo a seguir funciona bem _no Graph Explorer_ sem a codificação de caracteres de espaço e aspas:
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'jon@contoso.com'
``` 
- Em geral, ao especificar parâmetros de consulta _no seu aplicativo_, codifique adequadamente os caracteres que estiverem [reservados para significados especiais em um URI](https://tools.ietf.org/html/rfc3986#section-2.2). Por exemplo, codifique os caracteres de espaço e aspas no último exemplo, conforme mostrado abaixo:
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address%20eq%20%27jon@contoso.com%27
```


### <a name="search"></a>$search
Para restringir os resultados de uma solicitação que correspondam a um critério de pesquisa, use o parâmetro de consulta **$search**. 

>  **Observação**: No momento, é possível usar **$search** em coleções de [message](../api-reference/v1.0/resources/message.md) e [person](../api-reference/beta/resources/person.md), mas não em [contact](../api-reference/v1.0/resources/contact.md) ou [event](../api-reference/v1.0/resources/event.md). Uma solicitação de **$search** retorna até 250 resultados. Não é possível usar **$filter **ou **$orderby** em uma solicitação de **$search**.

Os critérios de pesquisa são expressos usando a sintaxe de consulta avançada (AQS). 

**Aplicação de $search a mensagens**

Os resultados da pesquisa são classificados pela data e hora em que a mensagem foi enviada.

Você pode especificar as propriedades a seguir em uma **message** em um critério **$search**: **attachments**, **bccRecipients**, **body**, **category**, **ccRecipients**, **content**, **from**, **hasAttachments**, **participants**, **receivedDateTime**, **sender**, **subject**, **toRecipients**

Se você realizar uma pesquisa em mensagens e especificar apenas um valor, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.

O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenha "pizza" em qualquer uma das três propriedades de pesquisa padrão: 

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

O próximo exemplo procura todas as mensagens na Caixa de Entrada do usuário que foram enviadas de um endereço de email específico:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```



### <a name="select"></a>$select
Para especificar um conjunto diferente de propriedades para retornar além do conjunto padrão fornecido pelo Graph, use a opção de consulta **$select**. A opção **$select** permite escolher um subconjunto do conjunto padrão retornado. Por exemplo, ao recuperar suas mensagens, selecione que apenas as propriedades **from** e **subject** das mensagens sejam retornadas.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

<!--For example, when retrieving the children of an item on a drive, you want to select that only the **name** and **size** properties of items are returned.

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

## <a name="expand"></a>$expand

Em solicitações da API do Microsoft Graph, as navegações para um objeto ou coleção do item referenciado não são expandidas automaticamente. Isso ocorre por design porque reduz o tráfego de rede e o tempo necessário para gerar uma resposta do serviço. No entanto, em alguns casos pode ser ideal incluir esses resultados em uma resposta.

Você pode usar o parâmetro da cadeia de caracteres de consulta **$expand** para instruir a API para expandir uma coleção ou objeto filho e incluir aqueles resultados.

Por exemplo, para recuperar as informações da unidade raiz e os itens filho de nível superior em uma unidade, use o parâmetro **$expand**. Esse exemplo também usa uma instrução **$select** para retornar apenas as propriedades _id_ e _name_ dos itens filhos.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

>  **Observação**: o número máximo de objetos expandidos em uma solicitação é 20. 

> Além disso, se você consultar no recurso [user](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user), é possível usar **$expand** para obter as propriedades de apenas um conjunto ou objeto filho de cada vez. 

O exemplo a seguir obtém objetos **user**, cada um com até 20 objetos **directReport** na coleção **directReports** expandida:
```http
GET https://graph.microsoft.com/v1.0/users?$expand=directReports
```
Alguns outros recursos também podem ter um limite, portanto, verifique sempre possíveis erros.


<!---The following shows a sample result that is returned in the response body.-->


## <a name="orderby"></a>$orderby

Para especificar a ordem de classificação de itens retornados da API do Microsoft Graph, use a opção de consulta **$orderby**. 

Por exemplo, para retornar os usuários na organização classificados por seu nome de exibição, a sintaxe é a seguinte:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
``` 

Você também pode classificar por entidades de tipo complexo. O exemplo abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
``` 

Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.

 >  **Observação**: Se você consultar o recurso [user](../api-reference/v1.0/resources/user.md), **$orderby** não poderá ser combinado com expressões de filtro.

## <a name="filter"></a>$filter
Para filtrar os dados de resposta baseado em um conjunto de critérios, use a opção de consulta **$filter**. Por exemplo, para retornar usuários na organização classificados por nome para exibição iniciado por “Donato”, a sintaxe é a seguinte:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'Garth')
```

Você também pode filtrar por entidades de tipo complexo. O exemplo a seguir retorna mensagens que tenham o campo **address** da propriedade **from** propriedade igual a "matheus@contoso.com". A propriedade **from** é do tipo complexo **emailAddress**.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'jon@contoso.com'
``` 

## <a name="top"></a>$top
Para especificar o número máximo de itens para retornar em um conjunto de resultados, use a opção de consulta **$top**. A opção **$top** identifica um subconjunto na coleção. Esse subconjunto é formado selecionando-se apenas os primeiros N itens do conjunto, em que N é um inteiro positivo especificado por essa opção de consulta. Por exemplo, para retornar as cinco primeiras mensagens na caixa de correio do usuário, a sintaxe é a seguinte:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

## <a name="skip"></a>$skip
Para definir o número de itens que devem ser ignorados antes de recuperar itens em uma coleção, use a opção de consulta **$skip**. Por exemplo, para retornar eventos classificados por data de criação e começando do 21º evento, a sintaxe é a seguinte:

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```

## <a name="skiptoken"></a>$skipToken
Para solicitar a segunda página e as páginas subsequentes dos dados do Graph, use a opção de consulta **$skipToken**. A opção de consulta **$skipToken** é uma opção fornecida em Urls retornadas do Graph quando ele tiver retornado um subconjunto parcial de resultados, geralmente devido à paginação no servidor. Ela identifica o ponto em um conjunto onde o servidor terminou de enviar resultados e volta para o Graph para indicar de onde ele deve recomeçar o envio dos resultados. Por exemplo, o valor de uma opção de consulta **$skipToken** poderia identificar o décimo item em uma coleção ou o vigésimo item em uma coleção contendo 50 itens, ou qualquer outra posição nela.

Você verá um valor `@odata.nextLink` em algumas respostas. Alguns deles incluem um valor **$skipToken**. O valor **$skipToken** é como um marcador que informa ao serviço onde retomar no próximo conjunto de resultados. A seguir está um exemplo de um valor `@odata.nextLink` de uma resposta onde os usuários foram solicitados ordenados por `displayName`: 

```
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27"
```

Para retornar para a próxima página de usuários em sua organização, a sintaxe é a seguinte.

```http
GET  https://graph.microsoft.com/v1.0/users?$orderby=displayName&$skiptoken=X%2783630372100000000000000000000%27
```

## <a name="count"></a>$count
Use **$count** como um parâmetro de consulta para incluir uma contagem do número total de itens em um conjunto junto com a página de valores de dados retornados do Graph, como no exemplo a seguir:
```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```
Isso retornaria ambas as coleções **contacts** e o número de itens na coleção **contacts** na propriedade `@odata.count`.

>**Observação:** Isso não é suportado pelas coleções [directoryObject](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/directoryobject).
