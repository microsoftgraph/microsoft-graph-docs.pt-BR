---
title: Criar esquema
description: Crie o esquema para uma Pesquisa da Microsoft conexão.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6f271195136a3a469de871e3f17fec5e485ff86c
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580706"
---
# <a name="create-schema"></a>Criar esquema
Namespace: microsoft.graph.externalConnectors



Crie um novo [objeto de esquema.](../resources/externalconnectors-schema.md)

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
No corpo da solicitação, fornece uma representação JSON de um [objeto de esquema.](../resources/externalconnectors-schema.md)

Ao registrar um esquema de item personalizado, o objeto DEVE ter a propriedade `schema` definida como e DEVE conter a `baseType` `microsoft.graph.externalItem` `properties` propriedade. O `properties` objeto deve conter pelo menos uma propriedade, até um máximo de 64.

## <a name="response"></a>Resposta

Com o header incluído na solicitação, se bem-sucedido, este método retorna um código de resposta e uma URL no header de resposta que podem ser usados para obter o `Prefer: respond-async` `202 Accepted` status da `Location` [operação](../api/externalconnectors-connectionoperation-get.md).

Sem o header incluído na solicitação, se bem-sucedido, este método retorna um código de resposta e um novo objeto `Prefer: respond-async` de esquema no corpo da `201 Created` resposta. [](../resources/externalconnectors-schema.md)

> [!NOTE]
> A criação de um esquema é um processo de longa duração propenso a tempos-de-tempo de gateway. Recomendamos usar `Prefer: respond-async` o header para evitar erros de tempo de tempo.

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
Prefer: respond-async

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
