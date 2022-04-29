---
title: Obter externalItem
description: Obter um externalItem.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 09eac8a949db61342c386bef6a90290346d4a371
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133248"
---
# <a name="get-externalitem"></a>Obter externalItem

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter as propriedades e as relações de um [objeto externalitem](../resources/externalconnectors-externalitem.md) .

Essa API é fornecida apenas para fins de diagnóstico. Ele não se destina a ser usado para nenhuma outra finalidade. Solicitações repetidas para essa API podem resultar em `429` erros HTTP.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | ExternalItem.ReadWrite.OwnedBy, ExternalItem.Read.All, ExternalItem.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.Read.All, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Parâmetros do caminho

| Parâmetro     | Tipo   | Descrição                                         |
|:--------------|:-------|:----------------------------------------------------|
| id da conexão | string | A `id` propriedade do [externalConnection que o contém](../resources/externalconnectors-externalconnection.md) |
| item-id       | string | A propriedade fornecida pelo `id` desenvolvedor do [externalItem](../resources/externalconnectors-externalitem.md). |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e um [objeto externalItem](../resources/externalconnectors-externalitem.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

```http
GET https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta
<!-- markdownlint-enable MD024 -->

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "acl": [
    {
      "type": "user",
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874",
      "accessType": "grant",
    },
    {
      "type": "externalGroup",
      "value": "14m1b9c38qe647f6a",
      "accessType": "deny",
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
