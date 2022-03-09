---
title: Criar esquema
description: Crie o esquema para uma Pesquisa da Microsoft conexão.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: eb0488fed1d07be4532061a3143ec00d39c5fa18
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396648"
---
# <a name="create-schema"></a>Criar esquema
Namespace: microsoft.graph.externalConnectors

Crie um novo [objeto de esquema](../resources/externalconnectors-schema.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|Não aplicável|
|Delegada (conta pessoal da Microsoft)|Não aplicável|
|Aplicativo| ExternalConnection.ReadWrite.OwnedBy|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /external/connections/{id}/schema
```
No corpo da solicitação, fornece uma representação JSON de um [objeto de esquema](../resources/externalconnectors-schema.md) .

Quando você registra um esquema de item personalizado, o objeto **de esquema** deve ter a **propriedade baseType** definida como `microsoft.graph.externalItem` e **deve** conter a **propriedade properties**. O **objeto properties** **deve** conter pelo menos uma propriedade, até um máximo de 128.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `202 Accepted` um código de resposta e uma URL `Location` no header de resposta que podem ser usados para [obter o status da operação](../api/externalconnectors-connectionoperation-get.md).

## <a name="examples"></a>Exemplos

### <a name="example-register-custom-schema-asynchronously"></a>Exemplo: Registrar esquema personalizado de forma assíncrona

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schema_from_connection_async",
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}-->

```http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/schema
Content-type: application/json

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "String",
      "isRetrievable": "true"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schema-from-connection-async-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schema-from-connection-async-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schema-from-connection-async-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schema-from-connection-async-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-schema-from-connection-async-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc
```
