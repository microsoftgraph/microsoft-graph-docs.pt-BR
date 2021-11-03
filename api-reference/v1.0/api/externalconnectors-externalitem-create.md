---
title: Criar externalItem
description: Crie um novo externalItem.
author: snlraju-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 21dc72a90dc863344380da4ece717bddba375cac
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688113"
---
# <a name="create-externalitem"></a>Criar externalItem

Namespace: microsoft.graph.externalConnectors

Crie um novo [objeto externalItem.](../resources/externalconnectors-externalitem.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Não aplicável|
|Delegado (conta pessoal da Microsoft)|Não aplicável|
|Aplicativo| ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /external/connections/{connectionsId}/items
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto externalItem.](../resources/externalconnectors-externalitem.md)

Você pode especificar as seguintes propriedades ao criar [um externalItem](../resources/externalconnectors-externalitem.md).

|Propriedade|Tipo| Descrição|
|:---|:---|:---|
|id|String|A ID do item. Obrigatório.|
|properties|[microsoft.graph.externalConnectors.properties](../resources/externalconnectors-properties.md)|As propriedades do item. O `properties` objeto deve conter pelo menos uma propriedade. Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601. Obrigatório.|
|conteúdo|[microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md)|O conteúdo do item externo. Opcional.|
|acl|[Coleção microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)|A lista de controles de acesso. Obrigatório.|

As propriedades em um `externalItem` devem usar especificadores de tipo na carga nos seguintes cenários:

- Para `String` propriedades de tipo, se o valor contiver caracteres não ASCII.

    ```json
    "description@odata.type": "String",
    "description": "Kandierte Äpfel"
    ```

- Para todos os tipos de coleção.

    ```json
    "categories@odata.type": "Collection(String)"
    "categories": [
      "red",
      "blue"
    ]
    ```

    > [!IMPORTANT]
    > Ao incluir uma propriedade do tipo `Collection(DateTime)` , você deve usar o especificador de tipo `Collection(DateTimeOffset)` .

## <a name="response"></a>Resposta 

Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.

## <a name="examples"></a>Exemplos

### <a name="example-create-a-custom-item"></a>Exemplo: Criar um item personalizado

### <a name="request"></a>Solicitação



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_externalConnections"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/external/connections/contosohr/items/TSP228082938
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-externalconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-externalconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-externalconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

