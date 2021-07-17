---
title: Criar externalItem
description: Crie um novo externalItem.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: eba04bf339eeed41f9fe59831773d413bbed3111
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467182"
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
POST /connections/{connectionsId}/items
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto externalItem.](../resources/externalconnectors-externalitem.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [externalItem](../resources/externalconnectors-externalitem.md).

|Propriedade|Tipo| Obrigatório (Y/N) | Descrição|
|:---|:---|:---|:---|
|id|String|Y|A ID do item|
|properties|[microsoft.graph.externalConnectors.properties](../resources/externalconnectors-properties.md)|Y|As propriedades do item. O `properties` objeto deve conter pelo menos uma propriedade. Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601.|
|conteúdo|[microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md)|N|O conteúdo do item externo|
|acl|[Coleção microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md)|Y|A lista de controles de acesso|

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

Se bem sucedido, este método retorna um código de resposta `200 OK`.

## <a name="examples"></a>Exemplos

### <a name="example-create-a-custom-item"></a>Exemplo: Criar um item personalizado

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_externalConnections"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/connections/contosohr/items/TSP228082938
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


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

