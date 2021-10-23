---
title: Excluir externalItem
description: Exclua um externalItem.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: abd29c8b59b169ff007dd2115c179a24fa8111d6
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561252"
---
# <a name="delete-externalitem"></a>Excluir externalItem

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excluir [um externalitem](../resources/externalconnectors-externalitem.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Parâmetros do caminho

| Parâmetro     | Tipo   | Descrição                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | string | A `id` propriedade do [externalConnection que](../resources/externalconnectors-externalconnection.md) contém |
| item-id       | string | A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalconnectors-externalitem.md). |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
```


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta
<!-- markdownlint-enable MD024 -->

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


