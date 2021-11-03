---
title: Atualizar externalItem
description: Atualize as propriedades de um externalitem.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7eb8742f912158b20464cf456086d8246c21feaa
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694512"
---
# <a name="update-externalitem"></a>Atualizar externalItem

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um externalitem](../resources/externalconnectors-externalitem.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Parâmetros do caminho

| Parâmetro     | Tipo   | Descrição                                         |
|:--------------|:-------|:----------------------------------------------------|
| connection-id | cadeia de caracteres | A `id` propriedade do [externalConnection que](../resources/externalconnectors-externalconnection.md) contém |
| item-id       | cadeia de caracteres | A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalconnectors-externalitem.md). |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
|:--------------|:----------------------------|
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. As propriedades existentes (excluindo propriedades dentro do objeto) que não estão incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base em alterações em outros valores `properties` de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades a seguir podem ser atualizadas.

| Propriedade   | Tipo                                  | Descrição               |
|:-----------|:--------------------------------------|:--------------------------|
| acl        | [Coleção microsoft.graph.externalConnectors.acl](../resources/externalconnectors-acl.md) | Uma matriz de entradas de controle de acesso. Cada entrada especifica o acesso concedido a um usuário ou grupo. |
| conteúdo    | [microsoft.graph.externalConnectors.externalItemContent](../resources/externalconnectors-externalitemcontent.md) | Uma representação em texto sem texto do conteúdo do item. O texto nesta propriedade é indexado em texto completo. |
| properties | Objeto                                | Um pacote de propriedades com as propriedades do item. As propriedades DEVEM estar em conformidade [com o esquema](../resources/externalconnectors-schema.md) definido para [externalConnection](../resources/externalconnectors-externalconnection.md). |

### <a name="updating-the-acl-collection"></a>Atualizando a coleção acl

Se a propriedade for incluída em uma solicitação de atualização, a coleção ACL existente será substituída com a `acl` coleção incluída na solicitação.

### <a name="updating-the-properties-object"></a>Atualizando o objeto properties

Se a propriedade for incluída em uma solicitação de atualização, o pacote de propriedades existente será substituído com o `properties` valor incluído na solicitação.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto externalItem](../resources/externalconnectors-externalitem.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_externalitem",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}-->

```http
PATCH https://graph.microsoft.com/beta/external/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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
  "id": "TSP228082938",
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalConnectors.externalItemContent",
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",
    "type": "html"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update externalitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: update_externalitem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->


