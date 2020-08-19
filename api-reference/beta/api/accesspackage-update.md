---
title: Atualizar accessPackage
description: Atualiza as propriedades de um objeto accessPackage.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 33a274dd9d8c06e01b8a27ac5a54df6407280a41
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806447"
---
# <a name="update-accesspackage"></a>Atualizar accessPackage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize um objeto [accessPackage](../resources/accesspackage.md) existente para alterar uma ou mais de suas propriedades, como o nome para exibição ou a descrição.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)     | EntitlementManagement.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros de um objeto [accessPackage](../resources/accesspackage.md) .

A tabela a seguir mostra as propriedades que podem ser fornecidas ao atualizar um [accessPackage](../resources/accesspackage.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome do pacote de acesso.|
|description|String|A descrição do pacote do Access.|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
Content-Type: application/json
Content-length: 38

{
  "displayName":"Access Package New Name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackage-objc-snippets.md)]
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
  "description": "Update accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
