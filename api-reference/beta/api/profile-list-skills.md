---
title: Listar habilidades
description: Recupere uma lista de objetos skillProficiency.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7040a3781de4f30feca7c45d303484855915e53e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135312"
---
# <a name="list-skills"></a>Listar habilidades

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [objetos skillProficiency](../resources/skillproficiency.md) no perfil de um [usuário.](../resources/profile.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All |
| Aplicativo                            | User.ReadBasic.All, User.Read.All, User.ReadWrite.All                            |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills
GET /users/{id | userPrincipalName}/profile/skills
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

|Nome            |Valor    |Descrição                                                                                                                                                                      |
|:---------------|:--------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|$filter         |string   |Limita a resposta apenas aos objetos que contêm os critérios especificados.                                                                                                  |
|$orderby        |cadeia de caracteres   |Por padrão, os objetos na resposta são classificação pelo valor **createdDateTime** em uma consulta. Você pode alterar a ordem da resposta usando o `$orderby` parâmetro.|
|$select         |string   |Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.                                             |
|$skip           |int      |Ignore os primeiros resultados n, úteis para pajamento.                                                                                                                                     |
|$top            |int      |Número de resultados a ser retornado.                                                                                                                                                |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           |Descrição                  |
|:---------------|:----------------------------|
| Autorização  | {token} de portador. Obrigatório.   |
| Content-Type   | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos skillProficiency](../resources/skillproficiency.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_skills"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/skills
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-skills-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-skills-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-skills-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-skills-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-skills-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-skills-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency",
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
      "categories": [
        "Professional"
      ],
      "displayName": "API Design",
      "proficiency": "advancedProfessional",
      "webUrl": null,
      "collaborationTags": [
        "ableToMentor"
      ]
    }
  ]
}
```


