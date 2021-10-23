---
title: Obter externalItem
description: Leia as propriedades e as relações de um objeto externalItem.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c983947208ea02f4af0f395c3e294acedc894b89
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558543"
---
# <a name="get-externalitem"></a>Obter externalItem
Namespace: microsoft.graph.externalConnectors



Leia as propriedades e as relações de um [objeto externalItem.](../resources/externalconnectors-externalitem.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Não aplicável|
|Delegado (conta pessoal da Microsoft)|Não aplicável|
|Application| ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /external/connections/{connectionsId}/items/{externalItemId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [externalItem](../resources/externalconnectors-externalitem.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

```http
GET https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant"
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "value": "Error in payment gateway...",
    "type": "text"
  }
}
```

