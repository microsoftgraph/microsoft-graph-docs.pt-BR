---
title: Criar authenticationContextClassReference
description: Crie uma nova autenticaçãoContextClassReference.
ms.localizationpriority: medium
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: afeaff3ef69ac7fdfb893a83fff24d4a7beac02a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028864"
---
# <a name="create-authenticationcontextclassreference"></a>Criar authenticationContextClassReference

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar uma nova [autenticaçãoContextClassReference](../resources/authenticationContextClassReference.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                    |
|:--------------------------------------|:---------------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Policy.ReadWrite.ConditionalAccess |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Policy.ReadWrite.ConditionalAccess |

> [!NOTE]
> Essa API tem um [problema conhecido relacionado](/graph/known-issues#permissions) a permissões.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/authenticationContextClassReferences
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição      |
|:--------------|:-----------------|
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto authenticationContextClassReference](../resources/authenticationcontextclassreference.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
O exemplo a seguir mostra a criação de uma nova authenticationcontextclassreference que está disponível para aplicativos usarem.




# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_authenticationcontextclassreference"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
Content-type: application/json

{
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-authenticationcontextclassreference-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-authenticationcontextclassreference-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-authenticationcontextclassreference-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-authenticationcontextclassreference-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReference/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
