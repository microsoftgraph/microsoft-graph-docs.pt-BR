---
title: Atualizar esquema
description: Atualize as propriedades de um esquema para um externalConnection.
ms.localizationpriority: medium
author: mecampos
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: bd0aa8d8d37c9cf7652853b530f91627f2286974
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266426"
---
# <a name="update-schema"></a>Atualizar esquema

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um esquema](../resources/externalconnectors-schema.md) para [um externalConnection](../resources/externalconnectors-externalconnection.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | ExternalConnection.ReadWrite.OwnedBy |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /external/connections/{connectionId}/schema
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome                  | Descrição                                                        |
|:----------------------|:-------------------------------------------------------------------|
| Autorização         | {token} de portador. Obrigatório.                                          |
| Content-Type          | application/json. Obrigatório.                                        |
| Prefer: respond-async | Use isso para fazer com que a solicitação seja executada de forma assíncrona. Opcional. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto de esquema.](../resources/externalconnectors-schema.md)

Quando você registra um esquema de item  personalizado, o objeto **de esquema** deve ter a **propriedade baseType** definida como e `microsoft.graph.externalItem` **deve** conter a **propriedade properties.** O **objeto properties** **deve** conter pelo menos uma propriedade, até um máximo de 128.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma URL no header de resposta que podem ser usados `202 Accepted` para obter o status da `Location` [operação.](../api/externalconnectors-connectionoperation-get.md)

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "update_schema"
}-->

```http
PATCH https://graph.microsoft.com/beta/external/connections/contosohr/schema
Content-type: application/json

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "string",
      "isSearchable": "true",
      "isRetrievable": "true",
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "string",
      "isQueryable": "true",
      "isRetrievable": "true",
      "isSearchable": "false"
    },
    {
      "name": "assignee",
      "type": "string",
      "isRetrievable": "true"
    }
  ]
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta
<!-- markdownlint-enable MD024 -->

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/external/connections/contosohr/operations/616bfeed-666f-4ce0-8cd9-058939010bfc

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
