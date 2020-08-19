---
title: Listar nomes
description: Recupere uma lista de objetos PersonName do perfil de um usuário.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 54c54827eb2719323078ca9325c46e0b7cf6449a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810703"
---
# <a name="list-names"></a>Listar nomes

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de objetos [PersonName](../resources/personname.md) do [perfil](../resources/profile.md)de um usuário.

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
GET /me/profile/names
GET /users/{id | userPrincipalName}/profile/names
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

|Nome            |Valor    |Descrição                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|$filter         |string   |Limita a resposta somente aos objetos que contêm os critérios especificados.                                                                                             |
|$orderby        |cadeia de caracteres   |Por padrão, os objetos na resposta são classificados por seu valor createdDateTime em uma consulta. Você pode alterar a ordem da resposta usando o parâmetro *$OrderBy* .|
|$select         |string   |Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.                                        |
|$skip           |int      |Ignore os primeiros n resultados, útil para paginação.                                                                                                                                |
|$top            |int      |Número de resultados a ser retornado.                                                                                                                                           |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           |Descrição                  |
|:---------------|:----------------------------|
| Autorização  | {token} de portador. Obrigatório.   |
| Content-Type   | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [PersonName](../resources/personname.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
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
      "displayName": "Innocenty Popov",
      "first": "Innocenty",
      "initials": "IP",
      "last": "Popov",
      "languageTag": "en-US",
      "maiden": null,
      "middle": null,
      "nickname": "Kesha",
      "suffix": null,
      "title": null,
      "pronunciation": {
        "displayName": "In-no ken-te ",
        "first": "In-no ken-te Pop-ov",
        "maiden": null,
        "middle": null,
        "last": "Pop-ov"
      }
    }
  ]
}
```
