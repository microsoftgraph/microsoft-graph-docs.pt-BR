---
title: Atualizar accessPackageCatalog
description: Atualize as propriedades de um objeto accessPackageCatalog.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3fbdeaae5ce9f0f09ded8f47b25213183f2da3ca
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60940110"
---
# <a name="update-accesspackagecatalog"></a>Atualizar accessPackageCatalog

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize um objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) existente para alterar uma ou mais de suas propriedades, como o nome de exibição ou a descrição.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto accessPackageCatalog.](../resources/accesspackagecatalog.md)

A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o accessPackageCatalog](../resources/accesspackagecatalog.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome do catálogo de pacotes de acesso.|
|description|Cadeia de caracteres|A descrição do catálogo de pacotes de acesso.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `204 No Content`.



## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
Content-Type: application/json

{
  "displayName":"Catalog One"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackagecatalog-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


