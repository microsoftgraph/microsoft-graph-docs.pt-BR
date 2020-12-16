---
title: Desinstalar o aplicativo em um chat
description: Desinstale (remover) um aplicativo instalado em um chat.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 212a033198a5bb1b6303b3d1a848ad32da4df5ab
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690092"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="65b77-103">Desinstalar o aplicativo em um chat</span><span class="sxs-lookup"><span data-stu-id="65b77-103">Uninstall app in a chat</span></span>

<span data-ttu-id="65b77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65b77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65b77-105">Desinstalar um [aplicativo](../resources/teamsapp.md) instalado em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="65b77-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="65b77-106">**Nota**: Se o chat estiver associado a uma instância [onlineMeeting](../resources/onlinemeeting.md), então, efetivamente, o **teamsApp** será removido da reunião.</span><span class="sxs-lookup"><span data-stu-id="65b77-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="65b77-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="65b77-107">Permissions</span></span>

<span data-ttu-id="65b77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65b77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65b77-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65b77-110">Permission type</span></span>      | <span data-ttu-id="65b77-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65b77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65b77-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65b77-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65b77-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="65b77-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="65b77-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65b77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b77-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65b77-115">Not supported.</span></span>   |
|<span data-ttu-id="65b77-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65b77-116">Application</span></span> | <span data-ttu-id="65b77-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="65b77-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65b77-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65b77-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="response"></a><span data-ttu-id="65b77-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="65b77-119">Response</span></span>

<span data-ttu-id="65b77-120">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65b77-120">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="65b77-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65b77-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="65b77-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65b77-122">Request</span></span>

<span data-ttu-id="65b77-123">O exemplo a seguir desinstala um aplicativo do chat especificado.</span><span class="sxs-lookup"><span data-stu-id="65b77-123">The following example uninstalls an app from the specified chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="65b77-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b77-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```
# <a name="c"></a>[<span data-ttu-id="65b77-125">C#</span><span class="sxs-lookup"><span data-stu-id="65b77-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65b77-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65b77-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65b77-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65b77-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65b77-128">Java</span><span class="sxs-lookup"><span data-stu-id="65b77-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65b77-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="65b77-129">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat delete installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
