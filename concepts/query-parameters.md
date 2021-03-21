---
title: Usar parâmetros de consulta para personalizar respostas
description: O Microsoft Graph fornece parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 51bf43360c3580011ab39e2c385b4c23d3bfc5a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962410"
---
# <a name="use-query-parameters-to-customize-responses"></a>Usar parâmetros de consulta para personalizar respostas

O Microsoft Graph fornece suporte a parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. O suporte para os parâmetros de consulta exatos variam de uma operação de API para outra e, dependendo da API, podem diferir entre os pontos de extremidade v1.0 e beta. 

> [!TIP] 
> No ponto de extremidade beta, o prefixo `$` é opcional. Por exemplo, em vez de `$filter`, você pode usar `filter`. No ponto de extremidade v1, o prefixo `$` é opcional apenas para um subconjunto de APIs. Para simplificar, inclua sempre `$` se estiver usando o ponto de extremidade v1.

Os parâmetros de consulta podem ser opções de consulta de sistema OData ou outros parâmetros de consulta. 

> [!VIDEO https://www.youtube-nocookie.com/embed/7BuFv3yETi4]

## <a name="odata-system-query-options"></a>Opções de consulta de sistema OData
Uma operação de API do Microsoft Graph pode oferecer suporte a uma ou mais das seguintes opções de consulta de sistema OData. Essas opções de consulta são compatíveis com a [linguagem de consulta OData V4][odata-query].

>**Observação:** o OData 4.0 oferece suporte às opções de consulta do sistema apenas em operações GET.

Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].

| Nome                     | Descrição | Exemplo
|:-------------------------|:------------|:---------|
| [$count](#count-parameter)         | Recupera a contagem total de recursos correspondentes. | [`/me/messages?$top=2&$count=true`][count-example]
| [$expand](#expand-parameter)       | Recupera os recursos relacionados.|[`/groups?$expand=members`][expand-example]
| [$filter](#filter-parameter)       | Filtra os resultados (linhas).|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [$format](#format-parameter)       | Retorna os resultados no formato de mídia especificado.|[`/users?$format=json`][format-example]
| [$orderby](#orderby-parameter)     | Ordena os resultados.|[`/users?$orderby=displayName desc`][orderby-example]
| [$search](#search-parameter)       | Retorna os resultados com base nos critérios de pesquisa. |[`/me/messages?$search=pizza`][search-example]
| [$select](#select-parameter)       | Filtra as propriedades (colunas).|[`/users?$select=givenName,surname`][select-example]
| [$skip](#skip-parameter)           | Índices em um conjunto de resultados. Também usado por algumas APIs para implementar a paginação e pode ser usado com `$top` para paginar resultados manualmente. | [`/me/messages?$skip=11`][skip-example]
| [$top](#top-parameter)             | Define o tamanho de página de resultados. |[`/users?$top=2`][top-example]


## <a name="other-query-parameters"></a>Outros parâmetros de consulta

| Nome                     | Descrição | Exemplo
|:-------------------------|:------------|:---------|
| [$skipToken](#skiptoken-parameter) | Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.) | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a>Outros recursos de URL OData

Os seguintes recursos OData 4.0 são segmentos de URL, não parâmetros de consulta.

| Nome                     | Descrição | Exemplo 
|:-------------------------|:------------|:---------|
| [$ref](/graph/api/group-post-members) | Atualiza a associação de entidades a uma coleção. | `POST /groups/{id}/members/$ref` |
| [$value](/graph/api/profilephoto-get) | Recupera ou atualiza o valor binário de um item. | `GET /me/photo/$value` |

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

### <a name="escaping-single-quotes"></a>Escape de aspas simples

Para pedidos que usem aspas simples, se os valores de qualquer parâmetro também contém aspas, elas devem ter escape duplo. Caso contrário, a solicitação falhará devido a sintaxe inválida. No exemplo, o valor de cadeia de caracteres `let''s meet for lunch?` tem o escape de aspas simples.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a>parâmetro count

Use o parâmetro de consulta `$count` para incluir uma contagem do número total de itens em um conjunto, juntamente com a página de valores de dados retornados do Microsoft Graph. 

Por exemplo, a solicitação a seguir retornará tanto o conjunto **contato** do usuário atual quanto o número de itens no conjunto **contato** na propriedade `@odata.count`.

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[Experimente o Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


O parâmetro de consulta `$count` é compatível com esses conjuntos de recursos e suas relações, derivadas do [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):
- [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
- [orgContact](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
- [device](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
- [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
- [users](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).

## <a name="expand-parameter"></a>parâmetro expand

Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos. Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos. Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações. 

Normalmente, você pode consultar as propriedades de um recurso ou uma de suas relações em uma única solicitação, mas não ambas. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou o conjunto referenciado por uma única relação (propriedade de navegação) nos resultados.

O seguinte exemplo obtém informações de unidade raiz juntamente com os itens filho de nível superior em uma unidade:

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

[Experimentar no Explorador do Graph][expand-example]

> **Observação:** nem todas as relações e recursos dão suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir as relações **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir suas relações **events**, **messages** ou **photo**. Nem todos os recursos ou relações dão suporte ao uso de `$select` em itens expandidos. 
> 
> Com recursos do Azure AD derivados de [directoryObject](/graph/api/resources/directoryobject), como [user](/graph/api/resources/user) e [group](/graph/api/resources/group), `$expand` só há suporte para `beta`, e normalmente são retornados no máximo 20 itens para a relação expandida.

## <a name="filter-parameter"></a>parâmetro filter

Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto. O parâmetro de consulta `$filter` também pode ser usado para recuperar relações como members, memberOf, transitiveMembers e transitiveMemberOf. Por exemplo, obter todos os grupos de segurança dos quais sou membro.

O exemplo a seguir pode ser usado para encontrar usuários cujo nome de exibição começa com a letra “J’: use `startsWith`.

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

[Experimentar no Explorador do Graph][filter-example]

O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph. Os seguintes operadores lógicos geralmente são suportados:

- é igual a `eq` / não é igual a `ne`
- menor que `lt` / maior que `gt`
- menor que ou igual a `le` / maior que ou igual a `ge`
- e `and` / ou `or`
- em `in`
- Negação `not`
- operador lambda qualquer `any`
- operador lambda todos `all`
- Começa com`startsWith`
- Termina com`endsWith`

> **Observação:** o suporte a esses operadores varia de acordo com a entidade. Confira a documentação específica da entidade para obter detalhes. 
>
> O operador da cadeia de caracteres `contains` atualmente não tem suporte em nenhum recurso do Microsoft Graph.

Para ver alguns exemplos de uso, consulte a tabela abaixo. Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].  
A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`.

> **Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].

| Descrição | Exemplo
|:------------|:--------|
| Pesquisar por usuários com o nome Clara entre várias propriedades. | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) |
| Obtenha todos os usuários com o domínio de email igual a 'hotmail.com' | [`https://graph.microsoft.com/v1.0/users?$count=true&$filter=endsWith(mail,'@hotmail.com')`](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) |
| Obter todos os eventos do usuário conectado que começaram após 01/07/2017. | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) |
| Obter todos os emails de um endereço específico recebidos pelo usuário conectado. | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) |
| Obter todos os emails recebidos pelo usuário conectado em abril de 2017. | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) |
| Obter todos os emails não lidos na caixa de entrada do usuário conectado. | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) |
| Listar todos os grupos do Microsoft 365 em uma organização. | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) |
| Use a conversão OData para obter uma participação transitória em grupos com um nome de exibição que comece com “a”, incluindo o número de objetos retornados. | [`https://graph.microsoft.com/beta/me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`](https://developer.microsoft.com/graph/graph-explorer?request=me/transitiveMemberOf/microsoft.graph.group?$count=true&$orderby=displayName&$filter=startswith(displayName,'a')&method=GET&version=v1.0) |

## <a name="format-parameter"></a>parâmetro format

Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.

Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

[Experimentar no Explorador do Graph][format-example]

> **Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.

## <a name="orderby-parameter"></a>parâmetro orderby

Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados pelo Microsoft Graph.

Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[Experimentar no Explorador do Graph][orderby-example]

Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`.

Com algumas APIs, você pode ordenar os resultados em várias propriedades. Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z – A) e, em seguida, por assunto, em ordem ascendente (padrão).

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[Experimentar no Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

> **Observação:** quando você especifica $filter, o servidor deduz uma ordem de classificação para os resultados. Se você usar `$orderby` e `$filter` juntos para receber mensagens, como o servidor sempre infere uma ordem de classificação para os resultados de `$filter`, você deve [especificar propriedades de determinadas maneiras](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).


O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[Experimente o Graph Explorer](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

> **Observação:** Combinar `$orderby` e parâmetros de consulta `$filter` é suportado no ponto de extremidade beta para os seguintes recursos do Microsoft Azure Active Directory e suas relações que derivam de [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta&preserve-view=true):
>
>- [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true)
>- [orgContact](/graph/api/resources/orgcontact?view=graph-rest-beta&preserve-view=true)
>- [device](/graph/api/resources/device?view=graph-rest-beta&preserve-view=true)
>- [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)
>- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true)
>- [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true)
>
> Para usar `$orderby` e `$filter` junto ou `$filter` com `endsWith` você precisa:
>
> - Adicionar `$count=true` aos parâmetros de consulta
> - Adicionar `ConsistencyLevel: eventual` ao cabeçalho de solicitação
>
> Confira [parâmetros opcionais de consulta de usuário](/graph/api/user-list?view=graph-rest-beta&preserve-view=true#optional-query-parameters) para obter mais informações.

## <a name="search-parameter"></a>parâmetro search

Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.

### <a name="using-search-on-message-collections"></a>Usando $search em conjuntos de mensagens

Você pode pesquisar mensagens com base em um valor nas propriedades de mensagens específicas. Os resultados da pesquisa são classificados pela data e hora em que a mensagem foi enviada. Uma solicitação de `$search` retorna até 250 resultados.

Se você realizar uma pesquisa em mensagens e especificar apenas um valor sem as propriedades de mensagens específicas, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.

O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

[Experimentar no Explorador do Graph][search-example]

Como alternativa, você pode pesquisar mensagens especificando os nomes de propriedade da mensagem na tabela a seguir, que são reconhecidos pela sintaxe da Linguagem de Consulta de Palavra-chave (KQL). Esses nomes de propriedades correspondem às propriedades definidas na entidade **mensagem** do Microsoft Graph. O Outlook e outros aplicativos do Microsoft 365 como o SharePoint são compatíveis com a sintaxe KQL, proporcionando a conveniência de um domínio de descoberta comum para seus repositórios de dados.


| Propriedades de emails pesquisáveis                | Descrição | Exemplo 
|:-------------------------|:------------|:---------|
| **attachment**           | Os nomes dos arquivos anexados a uma mensagem de email.|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| **bcc**           | O campo **Cco** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| **body**           | O corpo de uma mensagem de email.|[`me/messages?$search="body:excitement"`][search-body-example]
| **cc**           | O campo **Cc** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| **from**           | O remetente de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| **hasAttachment** | Verdadeiro se uma mensagem de email contiver um anexo que não seja um anexo embutido, caso contrário, falso. |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| **importance**           | A prioridade de uma mensagem de email, que um remetente pode especificar ao enviar uma mensagem. Os valores possíveis são `low`, `medium` ou `high`.|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| **kind**           | O tipo de mensagem. Os valores possíveis são `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` ou `voicemail`.|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| **participants**           | Os campos **de**, **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.|[`me/messages?$search="participants:danas"`][search-part-example]
| **received**           | A data em que uma mensagem de email foi recebida pelo destinatário.|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| **recipients**           | Os campos **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| **sent**           | A data em que uma mensagem de email foi enviada pelo remetente.|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| **size**           | O tamanho de um item em bytes.|[`me/messages?$search="size:1..500000"`][search-size-example]
| **subject**           | O texto na linha de assunto de uma mensagem de email. .|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| **to**           | O campo **para** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


Para saber mais sobre as propriedades de email pesquisáveis, KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:

- [Propriedades pesquisáveis no Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).

- [Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)

### <a name="using-search-on-person-collections"></a>Usando $search em conjuntos de pessoas

Você pode usar a API de Pessoas do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. A API de Pessoas é compatível com o parâmetro de consulta `$search`. Uma solicitação de `$search` retorna até 250 resultados.

As pesquisas de pessoas ocorrem nas propriedades **displayName** e **emailAddress** do recurso [person](/graph/api/resources/person).

A seguinte solicitação faz uma pesquisa por uma pessoa chamada "Clara Barbosa" nas propriedades **displayName** e **emailAddress** em todos os indivíduos no conjunto de **Pessoas** do usuário conectado. Como uma pessoa denominada "Clara Barbosa" é relevante para o usuário conectado, as informações para "Clara Barbosa" são retornadas.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

O exemplo a seguir mostra a resposta. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

Saiba mais sobre a API de Pessoas em [Obter informações sobre pessoas relevantes](./people-example.md#search-people).  

### <a name="using-search-on-directory-object-collections"></a>Como usar $search nos conjuntos de objetos do diretório

Você pode usar um parâmetro de consulta de `$search` para filtrar resultados usando a geração de tokens. A pesquisa tokenizada funciona extraindo palavras da cadeia de caracteres de entrada e de saída, usando espaços, números, uso de maiúsculas/minúsculas e símbolos para separar as palavras, da seguinte maneira:

* **Espaços**: `hello world` => `hello`, `world`
* **Caixa diferente**⁽¹⁾: `HelloWorld` ou `helloWORLD` => `hello`, `world`
* **Símbolos**⁽²⁾: `hello.world` => `hello`, `.`,`world`, `helloworld`
* **Números**: `hello123world` => `hello`,`123`, `world`

⁽¹⁾ Atualmente, a tokenização só funciona quando a caixa está mudando de minúsculas para maiúsculas, portanto, `HELLOworld` é considerada um único token: `helloworld`, e `HelloWORld` tem dois tokens: `hello`, `world`. ⁽²⁾ A lógica de tokenização também combina palavras que são separadas apenas por símbolos; por exemplo, pesquisar por `helloworld` irá localizar `hello-world` e `hello.world`.

> **Observação**: após a geração de tokens, os tokens são combinados independentemente da capitalização original e são combinados em qualquer ordem.
> O parâmetro de consulta de `$search` em coleções de objetos de diretório **requer** um cabeçalho de solicitação especial: `ConsistencyLevel: eventual`.

O suporte tokenizado à pesquisa funciona apenas nos campos **displayName** e **descrição**. Qualquer campo pode ser inserido em `$search`; campos diferentes de **displayName** e **descrição** padrão para `$filter` comportamento de startswith. Por exemplo:

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`

procurar todos os grupos com nomes de exibição que se pareçam com "OneVideo". O parâmetro `$search` também pode ser usado junto com o `$filter`. Por exemplo:

`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

procurar todos os grupos habilitados para email com nomes de exibição que se pareçam com "OneVideo". Os resultados são restringidos com base em uma conjunção lógica (um “AND”) do parâmetro `$filter` e na consulta inteira no parâmetro `$search`. O texto da pesquisa é tokenizado com base nas letras maiúsculas ou minúsculas, mas as equiparações são executadas de maneira insensível ao fato de a letra ser maiúscula ou minúscula. Por exemplo, "OneVideo" seria dividido em dois tokens de entrada "one" e "video", mas correspondendo a propriedades que não diferenciam maiúsculas de minúsculas.

A sintaxe da pesquisa segue as seguintes regras:

* Formato genérico: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.
* O número de cláusulas (clause) não é limitado. O uso de parênteses para a precedência também é suportado.
* A sintaxe para cada cláusula é: “\<property>:\<text to search>”.
* O nome da propriedade deve ser especificado na cláusula. Qualquer propriedade que possa ser usada em `$filter` também pode ser usada dentro de `$search`. Dependendo da propriedade, o comportamento da pesquisa será "search" ou, se “search” não for suportado na propriedade, "startswith".
* Todas as partes de cláusula devem ser colocadas entre aspas duplas.
* Os operadores lógicos “AND” e “OR” devem ser colocados fora das aspas duplas. Devem sempre ser grafados em maiúsculas.
* Considerando que toda a parte da cláusula precisa ser colocada entre aspas duplas, se contiver aspas duplas e barra invertida, as barras invertidas deverão ser usadas para escapar as aspas. Não é preciso escapar nenhum outro caractere.

A tabela a seguir mostra alguns exemplos.

| Classe de objeto | Descrição | Exemplo |
| ------------ | ----------- | ------- |
| Usuário | O caderno de endereços exibe o nome do usuário. | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr"` |
| Usuário | O caderno de endereços exibe o nome ou o email do usuário. | `https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"` |
| Grupo | O caderno de endereços exibe o nome ou a descrição de um grupo. | `https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")` |
| Grupo | Nome de exibição do catálogo de endereços em um grupo habilitado para email. | `https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"` |

Ambas as entradas da cadeia de caracteres fornecidas em `$search`, bem como as propriedades pesquisáveis, são divididas em partes por espaços, uso de maiúsculas/minúsculas e tipos de caracteres (números e caracteres especiais).

## <a name="select-parameter"></a>parâmetro select

Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos. Com $select, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.

Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[Experimentar no Explorador do Graph][select-example]

> **Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo. Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo. Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.
>
> No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](/graph/api/resources/directoryobject), como [usuário](/graph/api/resources/user) e [grupo](/graph/api/resources/group), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.  

## <a name="skip-parameter"></a>parâmetro skip

Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[Experimentar no Explorador do Graph][skip-example]

> **Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação. Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`. Você pode usar essa URL para retornar a próxima página de resultados. Para saber mais, confira [Paginação](./paging.md).

## <a name="skiptoken-parameter"></a>parâmetro skipToken

Algumas solicitações retornam várias páginas de dados, devido à paginação do lado do servidor ou devido ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta. Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência a páginas subsequentes do resultado.  
O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado na URL fornecida na propriedade `@odata.nextLink` na resposta. Para saber mais, confira [Paginação](./paging.md).
> **Observação:** se você estiver usando OData Count (adicionando `$count=true` na querystring), a propriedade `@odata.count` estará presente somente na primeira página.

## <a name="top-parameter"></a>parâmetro top

Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados. 

Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`. Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados. Para saber mais, confira [Paginação](./paging.md). 

O valor mínimo de $top é 1 e o máximo depende da API correspondente.  

Por exemplo, a seguinte solicitação de [lista de mensagens](/graph/api/user-list-messages) retorna as cinco primeiras mensagens na caixa de correio do usuário:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[Experimentar no Explorador do Graph][top-example]


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
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0



## <a name="see-also"></a>Confira também

- [Limitações de parâmetro de consulta](known-issues.md#query-parameter-limitations)
