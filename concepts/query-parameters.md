---
title: Usar parâmetros de consulta para personalizar respostas
description: O Microsoft Graph fornece parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta.
author: mumbi-o
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: e0af0692e89f0ea099fb480ecd57cd60e54bd798
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461370"
---
# <a name="use-query-parameters-to-customize-responses"></a>Usar parâmetros de consulta para personalizar respostas

O Microsoft Graph fornece suporte a parâmetros de consulta opcionais que você pode usar para especificar e controlar a quantidade de dados retornados em uma resposta. O suporte para os parâmetros de consulta exatos variam de uma operação de API para outra e, dependendo da API, podem diferir entre os pontos de extremidade v1.0 e beta.

> [!TIP] 
> No ponto de extremidade beta, o prefixo `$` é opcional. Por exemplo, em vez de `$filter`, você pode usar `filter`. No ponto de extremidade v1, o prefixo `$` é opcional apenas para um subconjunto de APIs. Para simplificar, inclua sempre `$` se estiver usando o ponto de extremidade v1.

Os parâmetros de consulta podem ser [opções de consulta de sistema OData](http://docs.oasis-open.org/odata/odata/v4.01/odata-v4.01-part2-url-conventions.html#_Toc31360955) ou outros parâmetros de consulta.

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

Para conhecer as opções de consulta do sistema OData que uma API e suas propriedades suportam, consulte a tabela **Propriedades** na página de recursos e a seção **Parâmetros de consulta opcionais** das operações LIST e GET para a API.

## <a name="other-query-parameters"></a>Outros parâmetros de consulta

| Nome                     | Descrição | Exemplo
|:-------------------------|:------------|:---------|
| [$skipToken](#skiptoken-parameter) | Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas. (Algumas APIs usam `$skip` em vez disso.) | `/users?$skiptoken=X%274453707402000100000017...`|

## <a name="other-odata-url-capabilities"></a>Outros recursos de URL OData

Os seguintes recursos OData 4.0 são segmentos de URL, não parâmetros de consulta.

| Nome                     | Descrição | Exemplo 
|:-------------------------|:------------|:---------|
| [$count](/graph/api/user-list#example-3-get-only-a-count-of-users)| Recupera o total inteiro da coleção. | `GET /users/$count` <br> `GET /groups/{id}/members/$count`|
| [$ref](/graph/api/group-post-members) | Atualiza a associação de entidades a uma coleção. | `POST /groups/{id}/members/$ref` |
| [$value](/graph/api/profilephoto-get) | Recupera ou atualiza o valor binário de um item. | `GET /me/photo/$value` |
| [&batch](/graph/json-batching) | Combina várias solicitações HTTP em uma solicitação em lote. | `POST /$batch` |

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

Para solicitações que usam aspas simples, se algum valor de parâmetro também contiver aspas simples, eles devem ter escape duplo; caso contrário, a solicitação falhará devido à sintaxe inválida. No exemplo, o valor da cadeia de caracteres `let''s meet for lunch?` tem a aspa simples com escape.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=subject eq 'let''s meet for lunch?'
```

## <a name="count-parameter"></a>parâmetro count

Use o `$count` parâmetro de consulta para recuperar a contagem do número total de itens em uma coleção ou correspondência de uma expressão. `$count` pode ser usado das seguintes maneiras:

1. Como um parâmetro de consulta de cadeia de caracteres `$count=true` para incluir uma contagem do número total de itens em uma coleção ao lado da página de valores de dados devolvidos do Microsoft Graph. Por exemplo, `users?$count=true`.
2. Como um [segmento de URL](#other-odata-url-capabilities) para recuperar somente o total inteiro da coleção. Por exemplo, `users/$count`.
3. Em uma `$filter` expressão com operadores de igualdade para recuperar uma coleção de dados onde a propriedade filtrada é uma coleção vazia. Consulte [os exemplos abaixo](#examples-using-the-filter-query-operator).

> [!NOTE]
> 1. Em recursos que derivam do [directoryObject](/graph/api/resources/directoryobject), `$count` só é suportado em uma consulta avançada. Consulte [Recursos avançados de consulta em objetos de diretório do Microsoft Azure Active Directory](/graph/aad-advanced-queries).
> 2. Não há suporte para o uso de `$count` em locatários do Microsoft Azure Active Directory B2C.

Por exemplo, a solicitação a seguir retornará tanto o conjunto **contato** do usuário atual quanto o número de itens no conjunto **contato** na propriedade `@odata.count`.

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

O parâmetro de consulta `$count` é suportado nas coleções dos seguintes recursos utilizados com frequência e suas relações que derivam do [directoryObject](/graph/api/resources/directoryobject) e somente em [consultas avançadas](/graph/aad-advanced-queries):
- [administrativeUnit](/graph/api/resources/administrativeunit)
- [application](/graph/api/resources/application)
- [orgContact](/graph/api/resources/orgcontact)
- [device](/graph/api/resources/device)
- [group](/graph/api/resources/group)
- [servicePrincipal](/graph/api/resources/serviceprincipal)
- [user](/graph/api/resources/user)

## <a name="expand-parameter"></a>parâmetro expand

Muitos recursos do Microsoft Graph expõem as propriedades declaradas do recurso, bem como as relações delas com outros recursos. Essas relações também são chamadas de propriedades de referência ou propriedades de navegação e podem fazer referência a um único recurso ou a um conjunto de recursos. Por exemplo, as pastas de email, gerente e subordinados diretos de um usuário são todas expostas como relações. 

Normalmente, você pode consultar as propriedades de um recurso ou um de seus relacionamentos em uma única solicitação, mas não ambos. Você pode usar o parâmetro de cadeia de caracteres de consulta `$expand` para incluir o recurso expandido ou coleção referenciada por um único relacionamento (propriedade de navegação) em seus resultados. Apenas um relacionamento pode ser expandido em uma única solicitação.

O exemplo a seguir obtém informações da unidade raiz juntamente com os itens filho de nível superior em uma unidade:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```


Com alguns conjuntos de recursos, você também pode especificar as propriedades a serem retornadas nos recursos expandidos adicionando um parâmetro `$select`. O exemplo a seguir executa a mesma consulta que o exemplo anterior, mas usa uma instrução [`$select`](#select-parameter) para limitar as propriedades retornadas para os itens filho expandidos para as propriedades **id** e **name**.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

> [!NOTE]
> + Nem todos os relacionamentos e recursos oferecem suporte ao parâmetro de consulta `$expand`. Por exemplo, você pode expandir os relacionamentos **directReports**, **manager** e **memberOf** em um usuário, mas não pode expandir seus **eventos**, **mensagens** ou **fotos**. Nem todos os recursos ou relacionamentos suportam o uso de `$select` em itens expandidos. 
> 
> + Com os recursos do Azure Active Directory derivados de [directoryObject](/graph/api/resources/directoryobject), como [usuário](/graph/api/resources/user) e [grupo](/graph/api/resources/group), `$expand` normalmente retorna no máximo 20 itens para o relacionamento expandido e não tem [@odata.nextLink](./paging.md). Veja mais [problemas conhecidos](known-issues.md#query-parameters).
>
> + `$expand` atualmente não é compatível com [consultas avançadas](/graph/aad-advanced-queries).

## <a name="filter-parameter"></a>parâmetro filter

Use o parâmetro de consulta `$filter` para recuperar apenas um subconjunto de um conjunto. O parâmetro de consulta `$filter` também pode ser usado para recuperar relações como members, memberOf, transitiveMembers e transitiveMemberOf. Por exemplo, obter todos os grupos de segurança dos quais sou membro.

O exemplo a seguir encontra o usuários cujo nome de exibição começa com a letra 'J':

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=startsWith(displayName,'J')
```

O suporte para operadores `$filter` varia entre as APIs do Microsoft Graph. Os seguintes operadores lógicos geralmente são suportados:

| Tipo de operador | Operador |
| --- | --- |
| Operadores de igualdade | <ul><li> Igual a (`eq`) </li><li> Não é igual a (`ne`)</li><li> Negação lógica (`not`)</li><li> Em (`in`)</li></ul> |
| Operadores relacionais | <ul><li> Menor que (`lt`) </li><li> Maior que (`gt`)</li><li> Menor ou igual a ( `le` )</li><li> Maior ou igual a (`ge`)</li></ul> |
| Operadores Lambda | <ul><li> Qualquer (`any`) </li><li> Todos (`all`)</li></ul>|
| Operadores condicionais | <ul><li> E (`and`) </li><li> Ou (`or`)</li> |
| Functions | <ul><li> Inicia com ( `startsWith` ) </li><li> Termina com (`endsWith`)</li><li> Contém ( `contains` )</li></ul>|


> **Observação:** o suporte para esses operadores varia de acordo com a entidade e algumas propriedades oferecem suporte `$filter` apenas em [consultas avançadas](/graph/aad-advanced-queries). Consulte a documentação específica da entidade para obter detalhes.

### <a name="filter-using-lambda-operators"></a>Filtrar usando operadores lambda

OData define os operadores `any` e `all` para avaliar correspondências em propriedades com valores múltiplos, ou seja, uma coleção de valores primitivos, como tipos de cadeia de caracteres ou coleção de entidades.

#### <a name="any-operator"></a>Operador  `any`

O operador `any` aplica iterativamente uma expressão booleana a cada membro de uma coleção e retorna `true` se a expressão for `true` para *qualquer membro* da coleção, caso contrário, retorna `false`. A seguir está a sintaxe do operador `any`:

```http
$filter=param/any(var:var/subparam eq 'value-to-match')
```

Em que
+ *param* é a propriedade que contém uma coleção de valores ou uma coleção de entidades.
+ *var:var* é uma variável de intervalo que contém o elemento atual da coleção durante a iteração. Essa variável pode ser nomeada praticamente qualquer coisa, por exemplo, *adele:adele* ou *x:x*.
+ *subparam* é necessário quando a consulta se aplica a uma coleção de entidades. Ele representa a propriedade do tipo complexo cujo valor estamos correspondendo.
+ *value-to-match* representa o membro da coleção com o qual estamos correspondendo.

Por exemplo, a propriedade **imAddresses** do recurso do usuário contém uma coleção do tipo Cadeia de Caracteres primitiva. A consulta a seguir recupera apenas os usuários com um imAddress de `admin@contoso.com`.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=imAddresses/any(s:s eq 'admin@contoso.com')
```

A propriedade **assignLicenses** do recurso do usuário contém uma coleção de objetos **assignLicense**, um tipo complexo com duas propriedades, **skuId** e **disabledPlans**. A consulta a seguir recupera apenas os usuários com uma licença atribuída identificada pela **skuId** `184efa21-98c3-4e5d-95ab-d07053a96e67`.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=assignedLicenses/any(s:s/skuId eq 184efa21-98c3-4e5d-95ab-d07053a96e67)
```

Para negar o resultado da expressão dentro da cláusula `any`, use o operador `not`, não o operador `ne`. Por exemplo, a consulta a seguir recupera apenas os usuários que não receberam o **imAddress** de `admin@contoso.com`.
>**Observação:** Para objetos de diretório como usuários, os operadores `not` e `ne` são suportados apenas em [consultas avançadas](/graph/aad-advanced-queries).

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=NOT(imAddresses/any(s:s eq 'admin@contoso.com'))&$count=true
ConsistencyLevel: eventual
```

#### <a name="all-operator"></a>Operador  `all`

O operador `all` aplica uma Expressão booleana a cada membro de uma coleção e retorna `true` se a expressão for `true` para *todos os membros* da coleção, caso contrário, retorna `false`. Não é suportado por nenhuma propriedade.

### <a name="examples-using-the-filter-query-operator"></a>Exemplos usando o operador de consulta de filtro

A tabela a seguir mostra alguns exemplos que usam o parâmetro de consulta `$filter`. Para obter mais detalhes sobre a sintaxe `$filter`, confira o [protocolo OData][odata-filter].

> **Observação:** Clique nos exemplos para testá-los no [Explorador do Graph][graph-explorer].

| Descrição | Exemplo
|:------------|:--------|
| Pesquisar por usuários com o nome Clara entre várias propriedades. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) `../users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')` |
| Obter todos os usuários com o domínio de email igual a 'hotmail.com' | [OBTER](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40hotmail.com')%26%24select%3Did%2CdisplayName%2Cmail&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@hotmail.com')`. Esta é uma [consulta avançada](/graph/aad-advanced-queries). |
| Obtenha todos os usuários sem licenças atribuídas | [OBTER](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedLicenses%2F%24count%2Bne%2B0%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedLicenses/$count eq 0&$count=true`. Esta é uma [consulta avançada](/graph/aad-advanced-queries). |
| Obter todos os eventos do usuário conectado que começaram após 01/07/2017. | 
  [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) `../me/events?$filter=start/dateTime ge '2017-07-01T08:00'`. <br/>**OBSERVAÇÃO:** A propriedade **dateTime** é um tipo Cadeia de caracteres. |
| Obter todos os emails de um endereço específico recebidos pelo usuário conectado. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) `../me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'` |
| Obter todos os emails recebidos pelo usuário conectado em abril de 2017. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01` |
| Obter todos os emails não lidos na caixa de entrada do usuário conectado. | [GET](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) `../me/mailFolders/inbox/messages?$filter=isRead eq false` |
| Obter todos os usuários nos departamentos de Varejo e Vendas. | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3Ddepartment%20in%20('Retail'%2C%20'Sales')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) `../users?$filter=department in ('Retail', 'Sales')`| 
| Listar os usuários com um plano de serviço específico que está em um estado suspenso. | [OBTER](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DassignedPlans%2Fany(a%3Aa%2FservicePlanId%20eq%202e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2%20and%20a%2FcapabilityStatus%20eq%20'Suspended')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=assignedPlans/any(a:a/servicePlanId eq 2e2ddb96-6af9-4b1d-a3f0-d6ecfd22edb2 and a/capabilityStatus eq 'Suspended')&$count=true`. Esta é uma [consulta avançada](/graph/aad-advanced-queries). |
| Listar todos os grupos que não são do Microsoft 365 em uma organização. | [OBTER](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DNOT%20groupTypes%2Fany(c%3Ac%20eq%20'Unified')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=NOT groupTypes/any(c:c eq 'Unified')&$count=true`. Esta é uma [consulta avançada](/graph/aad-advanced-queries). |
| Listar todos os usuários cujo nome da empresa não é indefinido (ou seja, não é um valor `null`) ou Microsoft. | [OBTER](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`. Esta é uma [consulta avançada](/graph/aad-advanced-queries). |
| Listar todos os usuários cujo nome da empresa seja indefinido ou Microsoft. | [OBTER](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20in%20(null%2C%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName in (null, 'Microsoft')&$count=true`. Esta é uma [consulta avançada](/graph/aad-advanced-queries). |
| Use a conversão OData para obter uma participação transitória em grupos com um nome de exibição que comece com “a”, incluindo o número de objetos retornados. | [OBTER](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true&$filter=startswith(displayName, 'a')`. Esta é uma [consulta avançada](/graph/aad-advanced-queries). |

## <a name="format-parameter"></a>parâmetro format

Use o parâmetro de consulta `$format` para especificar o formato de mídia dos itens retornados do Microsoft Graph.

Por exemplo, a seguinte solicitação retorna os usuários na organização no formato json:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$format=json
```


> **Observação:** o parâmetro de consulta `$format` é compatível com vários formatos (por exemplo, atom, xml e json), mas os resultados podem não ser retornados em todos os formatos.

## <a name="orderby-parameter"></a>parâmetro orderby

Use o parâmetro de consulta `$orderby` para especificar a ordem de classificação dos itens retornados do Microsoft Graph. A ordem padrão é crescente.

Por exemplo, a solicitação a seguir retorna os usuários da organização ordenados por seu nome de exibição:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```

Você também pode classificar por entidades de tipo complexo. A solicitação abaixo obtém mensagens e as classifica pelo campo **address** da propriedade **from**, que é do tipo complexo **emailAddress**:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```

Para classificar os resultados em ordem crescente ou decrescente, anexe `asc` ou `desc` ao nome do campo, separado por um espaço, por exemplo, `?$orderby=name%20desc`. Se a ordem de classificação não for especificada, o padrão (ordem crescente) será inferido.

Com algumas APIs, você pode ordenar os resultados em várias propriedades. Por exemplo, a solicitação a seguir ordena as mensagens na caixa de entrada do usuário primeiro pelo nome da pessoa que enviou, em ordem decrescente (Z a A) e, em seguida, por assunto, em ordem crescente (padrão).

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

> **Observação:** Quando você especificar `$filter` o servidor inferirá uma ordem de classificação para os resultados. Se você usar `$orderby` e `$filter` juntos para receber mensagens, como o servidor sempre infere uma ordem de classificação para os resultados de `$filter`, você deve [especificar propriedades de determinadas maneiras](/graph/api/user-list-messages#using-filter-and-orderby-in-the-same-query).


O exemplo a seguir mostra uma consulta filtrada pelas propriedades **subject** e **priority** e classificadas pelas propriedades **subject**, **priority** e **receivedDateTime** em ordem decrescente.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```


> [!NOTE] 
> A combinação dos parâmetros de consulta `$orderby` e `$filter` não tem suporte para objetos de diretório. Consulte [Recursos avançados de consulta em objetos de diretório do Microsoft Azure Active Directory](/graph/aad-advanced-queries).

## <a name="search-parameter"></a>parâmetro search

Use o parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa. Sua sintaxe e comportamento variam de uma operação de API para outra. Para ver a sintaxe para `$search` em diferentes recursos, consulte [Usar o parâmetro de consulta $search para corresponder a um critério de pesquisa](/graph/search-query-parameter).

## <a name="select-parameter"></a>parâmetro select

Use o parâmetro de consulta `$select` para retornar um conjunto de propriedades diferente do padrão definido para um recurso individual ou um conjunto de recursos. Com `$select`, você pode especificar um subconjunto ou um superconjunto das propriedades padrão.

Por exemplo, ao recuperar as mensagens do usuário conectado, você pode especificar que somente as propriedades **from** e **subject** sejam retornadas:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```


> **Importante:** Em geral, recomendamos que você use `$select` para limitar as propriedades retornadas por uma consulta àqueles exigidas pelo aplicativo. Isso se aplica particularmente a consultas com o potencial de retornar um conjunto de resultados amplo. Limitar as propriedades retornadas em cada linha reduzirá a carga de rede e ajudará a melhorar o desempenho do aplicativo.
>
> No `v1.0`, alguns recursos do Azure AD que derivam de [directoryObject](/graph/api/resources/directoryobject), como [usuário](/graph/api/resources/user) e [grupo](/graph/api/resources/group), retornam um subconjunto limitado padrão de propriedades em leituras. Para esses recursos, você deve usar `$select` para retornar propriedades fora do conjunto padrão.  

## <a name="skip-parameter"></a>parâmetro skip

Use o parâmetro de consulta `$skip` para definir o número de itens para ignorar no início de um conjunto. Por exemplo, a solicitação a seguir retorna eventos para o usuário classificadas por data de criação, começando com o evento 21 no conjunto:

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```


> **Observação:** algumas APIs do Microsoft Graph, como Email e Calendário do Outlook (**message**, **event** e **calendar**), usam `$skip` para implementar a paginação. Quando os resultados de uma consulta ocuparem várias páginas, essas APIs retornarão uma propriedade `@odata:nextLink` com uma URL que contém um parâmetro `$skip`. Você pode usar essa URL para retornar a próxima página de resultados. Para saber mais, confira [Paginação](./paging.md).
>
> O cabeçalho **ConsistencyLevel** necessário para consultas avançadas em objetos de diretório não é incluído por padrão nas solicitações de página subsequentes. Deve ser definido explicitamente nas páginas subsequentes.

## <a name="skiptoken-parameter"></a>parâmetro skipToken

Algumas solicitações retornam várias páginas de dados, devido à paginação do lado do servidor ou ao uso do parâmetro [`$top`](#top-parameter) para limitar o tamanho da página da resposta. Muitas APIs do Microsoft Graph usam o parâmetro de consulta `skipToken` para fazer referência às páginas subsequentes do resultado.  
O parâmetro `$skiptoken` contém um token opaco que faz referência à próxima página de resultados e é retornado no URL fornecido na propriedade `@odata.nextLink` na resposta. Para saber mais, consulte [Paging](./paging.md).
> **Observação:** Se você estiver usando a OData Count (adicionando `$count=true` na cadeia de caracteres de consulta) para consultas em objetos de diretório, a propriedade `@odata.count` estará presente apenas na primeira página.
>
> O cabeçalho **ConsistencyLevel** necessário para consultas avançadas em objetos de diretório não é incluído por padrão nas solicitações de página subsequentes. Deve ser definido explicitamente nas páginas subsequentes.

## <a name="top-parameter"></a>parâmetro top

Use o parâmetro de consulta `$top` para especificar o tamanho de página do conjunto de resultados. 

Se restarem mais itens no conjunto de resultados, o corpo da resposta conterá um parâmetro `@odata.nextLink`. Esse parâmetro contém uma URL que você pode usar para obter a próxima página de resultados. Para saber mais, confira [Paginação](./paging.md). 

O valor mínimo de $top é 1 e o máximo depende da API correspondente.  

Por exemplo, a seguinte solicitação de [lista de mensagens](/graph/api/user-list-messages) retorna as cinco primeiras mensagens na caixa de correio do usuário:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```


> O cabeçalho **ConsistencyLevel** necessário para consultas avançadas em objetos de diretório não é incluído por padrão nas solicitações de página subsequentes. Deve ser definido explicitamente nas páginas subsequentes.

## <a name="error-handling-for-query-parameters"></a>Tratamento de erro para parâmetros de consulta

Algumas solicitações retornarão uma mensagem de erro se não houver suporte para um parâmetro de consulta especificado. Por exemplo, você não pode usar `$expand` na relação `user/photo`. 

```http
https://graph.microsoft.com/v1.0/me?$expand=photo
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

## <a name="see-also"></a>Confira também

- [Recursos avançados de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries)
- [Usar o parâmetro de consulta $search para corresponder a um critério de pesquisa](/graph/search-query-parameter)
- [Limitações de parâmetro de consulta](known-issues.md#query-parameters)
