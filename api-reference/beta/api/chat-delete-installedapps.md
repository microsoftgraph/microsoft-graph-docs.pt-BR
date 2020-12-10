---
title: Desinstalar o aplicativo em um chat
description: Desinstale (remover) um aplicativo instalado em um chat.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a463fd0c57f707c766367b2bd6e7abc326d35aa2
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607470"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="f3ba5-103">Desinstalar o aplicativo em um chat</span><span class="sxs-lookup"><span data-stu-id="f3ba5-103">Uninstall app in a chat</span></span>

<span data-ttu-id="f3ba5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3ba5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3ba5-105">Desinstalar um [aplicativo](../resources/teamsapp.md) instalado em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="f3ba5-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f3ba5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f3ba5-106">Permissions</span></span>

<span data-ttu-id="f3ba5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3ba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3ba5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3ba5-109">Permission type</span></span>      | <span data-ttu-id="f3ba5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3ba5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3ba5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3ba5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f3ba5-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="f3ba5-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="f3ba5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3ba5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3ba5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3ba5-114">Not supported.</span></span>   |
|<span data-ttu-id="f3ba5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3ba5-115">Application</span></span> | <span data-ttu-id="f3ba5-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="f3ba5-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3ba5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3ba5-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="response"></a><span data-ttu-id="f3ba5-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ba5-118">Response</span></span>

<span data-ttu-id="f3ba5-119">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f3ba5-119">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3ba5-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3ba5-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3ba5-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3ba5-121">Request</span></span>

<span data-ttu-id="f3ba5-122">O exemplo a seguir desinstala um aplicativo do chat especificado.</span><span class="sxs-lookup"><span data-stu-id="f3ba5-122">The following example uninstalls an app from the specified chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```

### <a name="response"></a><span data-ttu-id="f3ba5-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ba5-123">Response</span></span>

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
