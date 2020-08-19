---
title: Listar posições
description: Recupere uma lista de objetos workPosition.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 60770c962298a764b686c6fa7c578c69e95dc0ec
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810676"
---
# <a name="list-positions"></a>Listar posições

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de objetos [workPosition](../resources/workposition.md) de um [perfil](../resources/profile.md)de usuário.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All |
| Delegada (conta pessoal da Microsoft) | User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All |
| Aplicativo                            | User. ReadBasic. All, User. Read. All, User. ReadWrite. All                            |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/positions
GET /users/{id | userPrincipalName}/profile/positions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

|Nome            |Valor    |Descrição                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|$filter         |string   |Limita a resposta somente aos objetos que contêm os critérios especificados.                                                                                             |
|$orderby        |cadeia de caracteres   |Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta. Você pode alterar a ordem da resposta usando o `$orderby` parâmetro.|
|$select         |string   |Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.                                        |
|$skip           |int      |Ignore os primeiros n resultados, útil para paginação.                                                                                                                                |
|$top            |int      |Número de resultados a ser retornado.                                                                                                                                           |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           |Descrição                  |
|:---------------|:----------------------------|
| Autorização  | {token} de portador. Obrigatório.   |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [workPosition](../resources/workposition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_positions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/positions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-positions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-positions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-positions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "source": null,
      "categories": null,
      "detail": {
        "company": {
          "displayName": "Adventureworks Ltd.",
          "pronunciation": null,
          "department": "Consulting",
          "officeLocation": "AW23/344",
          "address": {
            "type": "business",
            "postOfficeBox": null,
            "street": "123 Patriachy Ponds",
            "city": "Moscow",
            "state": null,
            "countryOrRegion": "Russian Federation",
            "postalCode": "RU-34621"
          },
          "webUrl": "https://www.adventureworks.com"
        },
        "description": null,
        "endMonthYear": null,
        "jobTitle": "Senior Product Branding Manager II",
        "role": "consulting",
        "startMonthYear": "datetime-value",
        "summary": null
      },
      "manager": null,
      "colleagues": null,
      "isCurrent": true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List positions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
