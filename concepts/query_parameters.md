# <a name="use-query-parameters-to-customize-responses"></a>Usar parâmetros de consulta para personalizar respostas

O Microsoft Graph fornece parâmetros de consulta opcional que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. Há suporte para os parâmetros de consulta a seguir.

>**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].

|Name|Descrição|Exemplo|
|:---------------|:--------|:-------|
|[$count](#count)|Recupera a contagem total de recursos correspondentes.|[`/me/messages?$top=2&$count=true`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0)|
|[$expand](#expand)|Recupera os recursos relacionados.|[`/groups?$expand=members`](https://developer.microsoft.com/graph/graph-explorer?request=groups$expand=members&method=GET&version=v1.0)|
|[$filter](#filter)|Filtra os resultados (linhas).|[`/users?$filter=startswith(givenName,'J')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)|
|[$format](#format)|Retorna os resultados no formato de mídia especificado.|[`/users?$format=json`](https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0)|
|[$orderby](#orderby)|Ordena os resultados.|[`/users?$orderby=displayName desc`](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0)|
|[$search](#search)| Retorna os resultados com base nos critérios de pesquisa. Atualmente com suporte em conjuntos de `messages` e `person`.|[`/me/messages?$search=pizza`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0)|
|[$select](#select)|Filtra as propriedades (colunas).|[`/users?$select=givenName,surname`](https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0)|
|[$skip](#skip)|Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente.  | [`/me/messages?$skip=11`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0)|
|[$skipToken](#skiptoken)|Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.) | `https://graph.microsoft.com/v1.0/users?$skiptoken=X%274453707402000100000017 ... 65612D643839392D343230372D613033662D306332623836633432363932B900000000000000000000%27`|
|[$top](#top)|Define o tamanho de página de resultados. |[`/users?$top=2`](https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0)|

Esses parâmetros são compatíveis com a [linguagem de consulta OData V4][odata-query]. Nem todos os parâmetros têm suporte em todas as APIs do Microsoft Graph, e o suporte pode diferir significativamente entre os pontos de extremidade `v1.0` e `beta`. 

> **Observação:** No ponto de extremidade `beta`, o prefixo `$` é opcional. Por exemplo, em vez de `$filter`, você pode usar `filter`. Para obter mais detalhes e exemplos, confira [Suporte a parâmetros da consulta sem prefixos $ no Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).

## <a name="encoding-query-parameters"></a>Codificação de parâmetros da consulta

Os valores dos parâmetros da consulta devem ser codificados por porcentagem. Muitas ferramentas, navegadores e clientes HTTP (como o [Explorador do Graph][graph-explorer]) ajudarão você com isso. Se uma consulta está falhando, uma causa possível é a falha na codificação adequada dos valores dos parâmetros da consulta.

Uma URL descodificada é semelhante a esta:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

Uma URL codificada adequadamente é semelhante a esta:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count"></a>Count

Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph. 

Por exemplo, a solicitação a seguir retornará o conjunto `contacts` do usuário atual e o número de itens no conjunto `contacts` na propriedade `@odata.count`.

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


>**Observação:**`$count` não há suporte para conjuntos de recursos derivados de [`directoryObject`](../api-reference/v1.0/resources/directoryobject.md), como conjuntos de [usuários](../api-reference/v1.0/resources/user.md) ou [grupos](../api-reference/v1.0/resources/group.md).

## <a name="expand"></a>expand

Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como suas relações com outros recursos. Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos. Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações. 

Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.

O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades `id` e `name`.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children($select=id,name)&method=GET&version=v1.0)

> **Observação:** Nem todas as relações e recursos de dão suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir as relações `directReports`, `manager` e `memberOf` em um usuário, mas não pode expandir suas relações `events`, `messages` ou `photo`. Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos. 
> 
> Com recursos do Azure AD derivados de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [user](../api-reference/v1.0/resources/user.md) e [group](../api-reference/v1.0/resources/group.md), `$expand` só há suporte para `beta`, e normalmente são retornados no máximo 20 itens para a relação expandida.

## <a name="filter"></a>filtro

Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto. 

Por exemplo, para localizar os usuários cujo nome de exibição se inicia com a letra "J", use `startswith`.

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0)

O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph. Os seguintes operadores lógicos geralmente são suportados: 

- igual a (`eq`)
- não é igual a (`ne`)
- maior que (`gt`)
- maior ou igual a (`ge`)
- menor que (`lt`), menor ou igual a (`le`)
- e (`and`)
- ou (`or`)
- não (`not`)
 
O operador de cadeia de caracteres `startswith` geralmente é suportado. O operador lambda `any` tem suporte em algumas APIs. Para ver alguns exemplos de uso, confira a tabela a seguir. Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].  

A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.

>**Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].

|Descrição|Exemplo|
|:--------|:-------|
|  Pesquisar por usuários com o nome Clara entre várias propriedades. | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| Obter todos os eventos do usuário conectado que começaram após 1/7/2017. | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| Obter todos os emails de um endereço específico recebidos pelo usuário conectado. | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| Obter todos os emails recebidos pelo usuário conectado em abril de 2017. | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| Obter todos os emails não lidos na caixa de entrada do usuário conectado. | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| Listar todos os grupos do Office 365 em uma organização. | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |

> **Observação:** Os seguintes operadores `$filter` não têm suporte para recursos do Azure AD: `ne`, `gt`, `ge`, `lt`, `le` e `not`. O operador de cadeia de caracteres `contains` atualmente não tem suporte em nenhum recurso do Microsoft Graph.

## <a name="format"></a>formato

Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.

Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0)

> **Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.

## <a name="orderby"></a>orderby

Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.

Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName&method=GET&version=v1.0)

Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo `address` da propriedade `from`, que é do tipo complexo `emailAddress`:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.

Com algumas APIs, você pode ordenar os resultados em várias propriedades. Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z - A) e, em seguida, por assunto, em ordem ascendente (padrão).

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```
[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)


 > **Observação:** Com os recursos do Azure AD derivados de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [user](../api-reference/v1.0/resources/user.md) e [group](../api-reference/v1.0/resources/group.md), você não pode combinar `$orderby` a expressões `$filter`. 

## <a name="search"></a>pesquisar

Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.

> **Observação:** Atualmente, é possível pesquisar **somente** coleções de [mensagens](../api-reference/v1.0/resources/message.md) e [pessoas](../api-reference/v1.0/resources/person.md). Uma solicitação de `$search` retorna até 250 resultados. Não é possível usar [`$filter`](#filter) ou [`$orderby`](#orderby) em uma solicitação de pesquisa.

### <a name="using-search-on-message-collections"></a>Usando $search em conjuntos de `message`

Critérios de pesquisa em mensagens são expressos usando [AQS (Sintaxe de Consulta Avançada)](https://support.office.com/article/Search-Mail-and-People-in-Outlook-com-and-Outlook-on-the-web-for-business-88108edf-028e-4306-b87e-7400bbb40aa7). Os resultados são classificados pela data e hora em que a mensagem foi enviada.

Você pode especificar as seguintes propriedades em uma `message` em um critério `$search`: 

- `attachments`
- `bccRecipients`
- `body`
- `category`
- `ccRecipients`
- `content`
- `from`
- `hasAttachments`
- `participants`
- `receivedDateTime`
- `sender`
- `subject`
- `toRecipients`

Se você realizar uma pesquisa em mensagens e especificar apenas um valor, a pesquisa será realizada nas propriedades de pesquisa padrão `from`, `subject` e `body`.

O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

O próximo exemplo procura todas as mensagens na Caixa de Entrada do usuário que foram enviadas de um endereço de email específico:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

### <a name="using-search-on-person-collections"></a>Usando $search em conjuntos de `person`

Você pode usar a API de Pessoas do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. A API de Pessoas dá suporte ao parâmetro de consulta `$search`.

As pesquisas de pessoas ocorrem nas propriedades `displayName` e `emailAddress` do recurso [pessoa](../api-reference/v1.0/resources/person.md). As pesquisas implementam um algoritmo de correspondência difusa. Retornarão resultados com base em uma correspondência exata e também em Inferências sobre a intenção da pesquisa. Por exemplo, imagine que um usuário com o nome de exibição "Carlos Lima" e o endereço de email carloslim@example.com que esteja no conjunto `people` do usuário conectado. Todas as pesquisas a seguintes retornarão resultados que contêm Carlos.

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

Você também pode executar pesquisas de pessoas que estão interessadas em determinado tópico. As pesquisas são executadas com base nas inferências derivadas das conversas de email do usuário. Por exemplo, a pesquisa a seguir retornará um conjunto de pessoas relevantes para o usuário conectado que tenham expressado interesse por pizza nas comunicações com o usuário. Observe que a frase de pesquisa está entre aspas.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

Finalmente, você pode combinar pesquisas de pessoas e pesquisas de tópicos na mesma solicitação combinando os dois tipos de expressão de pesquisa.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```
Essa solicitação realiza basicamente duas pesquisas: uma pesquisa difusa em relação às propriedades `displayName` e `emailAddress` de pessoas relevantes ao usuário conectado e uma pesquisa pontual por "pizza" em relação às pessoas relevantes ao usuário. Os resultados são classificados, ordenados e retornados. A pesquisa não é restritiva. Você pode obter resultados que contenham pessoas com correspondência difusa "car", que estejam interessadas em "pizza" ou ambos.

Para saber mais sobre a API de Pessoas, confira [Obter informações sobre pessoas relevantes](./people_example.md).  

## <a name="select"></a>select

Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos. Com $select, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.

Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades `from` e `subject` sejam retornadas:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$select=from,subject&method=GET&version=v1.0)

> **Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo. Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo. Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.
>
> No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](../api-reference/v1.0/resources/directoryobject.md), como [usuário](../api-reference/v1.0/resources/user.md) e [grupo](../api-reference/v1.0/resources/group.md), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.  

## <a name="skip"></a>ignorar

Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$orderby=createdDateTime&$skip=20&method=GET&version=v1.0)

> **Observação:** Algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (`message`, `event` e `calendar`), usam `$skip` para implementar a paginação. Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`. Você pode usar essa URL para retornar a próxima página de resultados. Para saber mais, confira [Paginação](./paging.md).

## <a name="skiptoken"></a>skipToken

Algumas solicitações retornam várias páginas de dados devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top) para limitar o tamanho da página da resposta. Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado. O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta. Para saber mais, confira [paginação](./paging.md).


## <a name="top"></a>top

Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados. 

Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`. Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados. Para saber mais, confira [Paginação](./paging.md). 

Por exemplo, a solicitação a seguir retorna as primeiras cinco mensagens na caixa de correio do usuário:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=5&method=GET&version=v1.0)


## <a name="error-handling-for-query-parameters"></a>Tratamento de erro para parâmetros de consulta

Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`. 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente. Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte. Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado. 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356