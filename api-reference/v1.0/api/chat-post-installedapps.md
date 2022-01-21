---
title: Adicionar o aplicativo ao chat
description: Instalar um aplicativo para chat.
author: subray
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7a1aeb13e8b0f0e6ba664012fc074533e4a543c1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122299"
---
# <a name="add-app-to-chat"></a>Adicionar o aplicativo ao chat

Namespace: microsoft.graph


Instale um [teamsApp](../resources/teamsapp.md) para o [chat](../resources/chat.md)especificado.

> **Observações**:
> - Se o chat estiver associado a uma instância do [onlineMeeting](../resources/onlinemeeting.md), então, efetivamente, o **teamsApp** será instalado na reunião.
> - Atualmente, essa operação não dá suporte à instalação de aplicativos que exigem permissões de consentimento específicas do recurso. Para mais detalhes, confira [Problemas conhecidos](/graph/known-issues#Installation-of-apps-that-require-resource-specific-consent-permissions-is-not-supported).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { 
"blockType": "ignored" 
} -->

```http
POST /chats/{chat-id}/installedApps
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

O corpo da solicitação deve conter a ID do aplicativo gerado pelo aplicativo de catálogo. Para obter detalhes, confira [teamsApp properties](../resources/teamsapp.md#properties).

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `201 Created`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_app_in_chat"
}-->

```http
POST https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps
Content-Type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-app-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-app-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-app-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-app-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-app-in-chat-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/add-app-in-chat-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat add installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
