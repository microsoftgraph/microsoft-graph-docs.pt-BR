---
title: Desinstalar o aplicativo em um chat
description: Desinstale (remover) um aplicativo instalado em um chat.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 954567f3d899f432922edb2c1c618814282043c4
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658580"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="518fa-103">Desinstalar o aplicativo em um chat</span><span class="sxs-lookup"><span data-stu-id="518fa-103">Uninstall app in a chat</span></span>

<span data-ttu-id="518fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="518fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="518fa-105">Desinstalar um [aplicativo](../resources/teamsapp.md) instalado em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="518fa-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="518fa-106">**Nota**: Se o chat estiver associado a uma instância [onlineMeeting](../resources/onlinemeeting.md), então, efetivamente, o **teamsApp** será removido da reunião.</span><span class="sxs-lookup"><span data-stu-id="518fa-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="518fa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="518fa-107">Permissions</span></span>

<span data-ttu-id="518fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="518fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="518fa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="518fa-110">Permission type</span></span>      | <span data-ttu-id="518fa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="518fa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="518fa-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="518fa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="518fa-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="518fa-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="518fa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="518fa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="518fa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="518fa-115">Not supported.</span></span>   |
|<span data-ttu-id="518fa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="518fa-116">Application</span></span> | <span data-ttu-id="518fa-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="518fa-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="518fa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="518fa-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="response"></a><span data-ttu-id="518fa-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="518fa-119">Response</span></span>

<span data-ttu-id="518fa-120">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="518fa-120">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="518fa-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="518fa-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="518fa-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="518fa-122">Request</span></span>

<span data-ttu-id="518fa-123">O exemplo a seguir desinstala um aplicativo do chat especificado.</span><span class="sxs-lookup"><span data-stu-id="518fa-123">The following example uninstalls an app from the specified chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```

### <a name="response"></a><span data-ttu-id="518fa-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="518fa-124">Response</span></span>

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
