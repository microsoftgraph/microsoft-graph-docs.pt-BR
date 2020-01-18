---
title: Listar se aplica
description: Obtenha uma lista de objetos directoryobject aos quais um objeto tokenLifetimePolicy foi aplicado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec486f79c1f9c61c606c5630aa7810480a1d2b81
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234115"
---
# <a name="list-appliesto"></a>Listar se aplica

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista de objetos [directoryobject](../resources/directoryObject.md) aos quais um objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) foi aplicado. O tokenLifetimePolicy só pode ser aplicado aos recursos [Application](../resources/application.md) e [servicePrincipalName](../resources/serviceprincipal.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Policy. Read. All e Application. Read. All, Directory. Read. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Policy. Read. All e Application. Read. All, Directory. Read. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método oferece suporte `$expand`ao `$select` e `$top` aos parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters). Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/tokenLifetimePolicies/{id}/appliesTo
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->