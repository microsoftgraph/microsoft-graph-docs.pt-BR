---
title: Listar pessoas
description: Recupere uma coleção de objetos person ordenados por relevância para o usuário, o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.
author: simonhult
ms.openlocfilehash: 52f3dade14af76732381bf71f0d8556f543287fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350110"
---
# <a name="list-people"></a>Listar pessoas

Recupere uma coleção de objetos [person](../resources/person.md) ordenados por relevância para o [usuário](../resources/user.md), o que é determinado pelo padrões de comunicação e colaboração e pelas relações comerciais do usuário.

Você pode obter essas informações por meio da API de Pessoas. Para ver exemplos, confira a seção [Exemplos](#examples) e o artigo [Obter informações relevantes sobre as pessoas](/graph/people-example).

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

Este método oferece suporte aos [ parâmetros de consulta OData ](/graph/query-parameters) para personalizar a resposta, como mostrado nos exemplos no artigo [Obter informações relevantes sobre pessoas](/graph/people-example).

|Nome|Valor|Descrição|
|:---------------|:--------|:-------|
|$filter|string|Limita a resposta apenas às pessoas cujo registro contém os critérios especificados.|
|$orderby|string|Por padrão, as pessoas na resposta são classificadas pela relevância delas à consulta. Você pode alterar a ordem das pessoas na resposta usando o parâmetro *$orderby*.|
|$search|string|Pesquisar pessoas por nome ou alias. Suporta correspondência difusa. Parâmetro funciona apenas para a pesquisa de pessoas de relevantes do usuário conectado, não para pesquisar pessoas relevantes para outros usuários. Também oferece suporte a `topic` palavra-chave para localizar pessoas com base em tópicos extraídos de conversas de email com essa pessoa. Consulte a seção de *executar uma pesquisa difusa* em [obter as informações relevantes sobre pessoas](/graph/people-example#perform-a-fuzzy-search) para obter informações e exemplos. |
|$select|string|Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.|
|$skip|inteiro|Ignorar os primeiros n resultados, útil para paginação. Não é suportado ao usar *$search*.|
|$top|inteiro|Número de resultados a ser retornado.|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Aceitar | application/json |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [person](../resources/person.md) no corpo da resposta. A resposta pode conter um objeto person ou uma coleção de objetos person.

## <a name="examples"></a>Exemplos

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "name": "get_person_collection",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1370

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
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "relevanceScore": 30.0
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Group",
                "subclass": "UnifiedGroup"
            }
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "IsaiahL@contoso.com",
            "imAddress": "sip:isaiahl@contoso.com",
            "scoredEmailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "relevanceScore": 20.0
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```

Para ver mais exemplos, confira o artigo [Obter informações relevantes sobre as pessoas](/graph/people-example).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
