---
title: Criar externalItem
description: Criar um novo externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 298a5bc01b3891831e1a8fd6774d721dc977b940
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869771"
---
# <a name="create-externalitem"></a>Criar externalItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [externalItem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md).

Essa API pode ser usada para criar um item personalizado ou um arquivo. Especifique o tipo que você está criando incluindo a `@odata.type` Propriedade no corpo JSON. O [externalConnection](../resources/externalconnection.md) recipiente deve ter um [esquema](../resources/schema.md) registrado do tipo correspondente.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application                            | ExternalItem.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PUT /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a>Parâmetros do caminho

| Parâmetro     | Tipo   | Descrição                                         |
|:--------------|:-------|:----------------------------------------------------|
| ID de conexão | string | A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém |
| item-id       | string | A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md) ou do [externalfile](../resources/externalfile.md). Se nenhum item já existir com isso `id`, um novo item é criado. Se já existir um item com isso `id`, ele será substituído pelo objeto enviado no corpo. |

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
|:--------------|:----------------------------|
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [externalItem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md) . A carga é limitada a 4 MB.

### <a name="creating-an-externalitem"></a>Criar um externalItem

Ao criar um `externalItem`, os campos a seguir são `@odata.type`obrigatórios `acl`:, `properties`e. O `properties` objeto deve conter pelo menos uma propriedade.

Todas `DateTime` as propriedades de tipo devem estar no formato ISO 8601.

As propriedades em `externalItem` um devem usar especificadores de tipo na carga nos seguintes cenários:

- Para `String` Propriedades de tipo, se o valor contiver caracteres não-ASCII.

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
    > Ao incluir uma propriedade de tipo `Collection(DateTime)`, você deve usar o especificador `Collection(DateTimeOffset)`de tipo.

### <a name="creating-an-externalfile"></a>Criando um externalfile

Ao criar um `externalFile`, os campos a seguir são obrigatórios `acl`: `name` `@odata.type`,, `url`e.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK`.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-custom-item"></a>Exemplo 1: criar um item personalizado

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalItem",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "deny",
      "identitySource": "Azure Active Directory"
    }
  ],
  "properties": {
    "title": "Error in the payment gateway",
    "priority": 1,
    "assignee": "john@contoso.com"
  },
  "content": "Textual content of the file"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalitem-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalitem-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalitem-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>Resposta
<!-- markdownlint-enable MD024 -->

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

### <a name="example-2-create-a-file"></a>Exemplo 2: criar um arquivo

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a>Solicitação
<!-- markdownlint-enable MD024 -->

Este é um exemplo de solicitação.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalfile_from_connections"
}-->

```http
PUT https://graph.microsoft.com/beta/connections/contosofiles/items/myFile01
Content-type: application/json

{
  "@odata.type": "microsoft.graph.externalFile",
  "acl": [
    {
      "type": "user",
      "value": "49103559-feac-4575-8b94-254814dfca72",
      "accessType": "grant",
      "identitySource": "Azure Active Directory"
    }
  ],
  "createdDateTime": "2019-01-31T03:44:19.0354159Z",
  "modifiedDateTime": "2019-01-31T03:44:19.0354159Z",
  "createdBy": "Pradeep Gupta",
  "lastModifiedBy": "Adele Vance",
  "title": "Enterprise Search Graph Ingestion API",
  "url": "file://filesrv02.corp.contoso.com/data/project/Enterprise Search.docx",
  "name": "Enterprise Search.docx",
  "extension": "docx",
  "size": 8676776,
  "content": "The quick brown fox jumps over the lazy dog."
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalfile-from-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalfile-from-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalfile-from-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>Resposta
<!-- markdownlint-enable MD024 -->

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
