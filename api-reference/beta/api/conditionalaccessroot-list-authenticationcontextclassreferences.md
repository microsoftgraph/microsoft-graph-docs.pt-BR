---
title: Listar authenticationContextClassReferences
description: Recupere uma lista de objetos authenticationContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c5ad949518d8371e18fc1ef10e680f618056b7f5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547308"
---
# <a name="list-authenticationcontextclassreferences"></a>Listar authenticationContextClassReferences

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de [objetos authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos `$filter` `$select` parâmetros de consulta E OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [authenticationContextClassReference](..\resources\authenticationcontextclassreference.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
```



### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#/conditionalAccess/authenticationContextClassReferences",
  "value": [
    {
      "id": "c1",
      "displayName": "Contoso trusted locations",
      "description": "Access is only allowed from trusted locations",
      "isAvailable": true
    }
  ]
}


```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List authenticationContextClassReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
