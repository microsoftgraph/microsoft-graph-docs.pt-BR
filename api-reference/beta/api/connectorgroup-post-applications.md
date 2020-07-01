---
title: Atribuir um conector a um aplicativo
description: Use esta API para atribuir um conector a um aplicativo
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a45037dc22298482001bb3f010aca538e4939ecd
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006854"
---
# <a name="assign-a-connectorgroup-to-an-application"></a>Atribuir um conector a um aplicativo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atribuir um [conector](../resources/connectorgroup.md) a um [aplicativo](../resources/application.md).

## <a name="permissions"></a>Permissões
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /applications/{id}/connectorGroup/$ref

```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | Portador. Obrigatório.|
| Content-type | application/json. Required.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto do objeto de [conexão](../resources/connectorgroup.md) .

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/connectorGroup/$ref

Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Assign a connectorGroup to an application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
