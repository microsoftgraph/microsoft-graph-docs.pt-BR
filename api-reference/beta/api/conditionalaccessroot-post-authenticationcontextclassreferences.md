---
title: Criar authenticationContextClassReference
description: Crie uma nova autenticaçãoContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8ad536988d73e8550ec4561f0ca6ead77c40d256
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547305"
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
