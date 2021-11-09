---
title: Listar pessoas
description: Recupere uma lista de objetos person ordenados por relevância para o usuário, o que é determinado pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.
author: anthona
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: e28372da45a246e92b696f8e8b7ed79e5e7cb050
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780482"
---
# <a name="list-people"></a>Listar pessoas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [objetos](../resources/person.md) de pessoa ordenados por sua relevância para o usuário [,](../resources/user.md)que é determinado pelos padrões de comunicação e colaboração do usuário e pelas relações comerciais.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | People.Read, People.Read.All    |
|Delegado (conta pessoal da Microsoft) | People.Read    |
|Aplicativo | People.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.

|Nome|Valor|Descrição|
|:---------------|:--------|:-------|
|$filter|string|Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.|
|$orderby|cadeia de caracteres|Por padrão, as pessoas na resposta são classificadas por relevância para sua consulta. Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.|
|$search|string|Pesquisar pessoas por nome ou alias. Suporta correspondência difusa. O parâmetro só funciona para pesquisar pessoas relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários. Também dá suporte a `topic` palavra-chave para encontrar pessoas com base em tópicos extraídos a partir de conversas de email com essa pessoa. Confira a seção *Realizar uma pesquisa difusa* em [Obter informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para informações e exemplos.|
|$select|string|Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.|
|$skip|int|Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.|
|$top|int|Número de resultados a ser retornado.|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Aceitar | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [person](../resources/person.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="browse"></a>Procurar

As solicitações nesta seção têm as pessoas mais relevantes para o usuário ( ), com base na `/me` comunicação, colaboração e relações comerciais.

Por padrão, cada resposta retorna 10 registros, mas você pode alterar esse número usando o parâmetro *$top*. Essas solicitações exigem a permissão People.Read.

#### <a name="request"></a>Solicitação

A seguir, um exemplo da solicitação padrão.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/people
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a>Solicitação de uma página subsequente de pessoas

Se a primeira resposta não contiver a lista completa das pessoas relevantes, você poderá fazer uma segunda solicitação usando *$top* e *$skip* para solicitar páginas adicionais de informações. Se a solicitação anterior tiver informações adicionais, a solicitação a seguir obterá a próxima página de pessoas do servidor.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>Classificar a resposta

Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*. Essa consulta seleciona as pessoas mais relevantes para você classificando-as pelo nome de exibição e retorna as dez primeiras pessoas da lista classificada.

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>Alteração do número de pessoas e dos campos retornados

Você pode alterar o número de pessoas retornadas na resposta definindo o parâmetro *$top*.

O exemplo a seguir solicita as 1.000 pessoas mais relevantes para `/me` . A solicitação também limita a quantidade de dados enviados de volta do servidor solicitando apenas o nome de exibição da pessoa.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>Seleção dos campos que devem ser retornados

Você pode limitar a quantidade de dados retornados do servidor usando o parâmetro *$select* para escolher um ou mais campos. O campo *@odata.id* é sempre retornado.

O exemplo a seguir limita a resposta para *DisplayName* e *EmailAddress* das 10 pessoas mais relevantes.

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>Uso de um filtro para limitar a resposta

Você pode usar o parâmetro *$filter* para limitar a resposta apenas às pessoas cujo registro contém os critérios especificados.

A consulta a seguir limita a resposta a pessoas com a origem "Directory".

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>Selecionando os campos para retornar em uma resposta filtrada

Você pode combinar os parâmetros *$select* e *$filter* para criar uma lista personalizada de pessoas relevantes para o usuário e obter somente os campos necessários para seu aplicativo.

O exemplo a seguir obtém *DisplayName* e *EmailAddress* de pessoas cujo nome de exibição é igual ao nome especificado. Neste exemplo, somente as pessoas cujo nome de exibição é igual a "Nestor Kellum" são retornadas.

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>Pesquisar pessoas

As solicitações nesta seção também obterão as pessoas mais relevantes para o usuário de sessão ( `/me` ). As solicitações de pesquisa exigem a permissão People.Read.

#### <a name="using-search-to-select-people"></a>Usando a pesquisa para selecionar pessoas

Use o parâmetro *$search* para selecionar as pessoas que atendem a determinado conjunto de critérios.

A consulta de pesquisa a seguir retorna pessoas `/me` relevantes para cuja GivenName ou Sobrenome começa com a letra "j".

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>Uso da pesquisa para especificar um tópico relevante

A solicitação a seguir retorna pessoas relevantes cujo nome contém "ma" e que têm uma associação `/me` com "planejamento de recursos".

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>Execução de uma pesquisa difusa

A solicitação a seguir faz uma pesquisa para uma pessoa chamada "Hermaini Hall". Como há uma pessoa chamada "Herminia Hull" relevante para o usuário in-loco, as informações de "Herminia Hull" são retornadas.

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>Pessoas relacionadas

A solicitação a seguir obtém as pessoas mais relevantes para outra pessoa na organização do usuário. Essa solicitação requer a permissão User.ReadBasic.All para People.Read.All. Neste exemplo, as pessoas relevantes de Nestor Kellum são exibidas.

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


