---
title: Listar educationSchools
description: Recupere uma lista de todos os objetos de escola.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cf6bde0c9230be7932c86b6a4bb7a6de63f5b351
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366020"
---
# <a name="list-educationschools"></a>Listar educationSchools

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de todos os objetos de escola.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | EduRoster.ReadBasic                         |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | EduRoster.Read.All, EduRoster.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http 
GET /education/schools
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                     |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de objetos [educationSchool](../resources/educationschool.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_schools_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schools-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schools-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schools-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schools-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-schools-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-schools-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "value":[
      {
         "id":"10001",
         "displayName":"Contoso High School",
         "description":"Public 9-12 high school",
         "status":"active",
         "externalSource":"sis",
         "principalEmail":"amyr@contoso.com",
         "principalName":"Amy Roebuck",
         "externalPrincipalId":"14007",
         "highestGrade":"12",
         "lowestGrade":"9",
         "schoolNumber":"10001",
         "address":{
            "city":"Los Angeles",
            "countryOrRegion":"United States",
            "postalCode":"98055",
            "state":"CA",
            "street":"12345 Main St."
         },
         "createdBy":{
            "user":{
               "displayName":"Susana Rocha",
               "id":"14012"
            }
         },
         "externalId":"10001",
         "phone":"+1 (253) 555-0102"
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
