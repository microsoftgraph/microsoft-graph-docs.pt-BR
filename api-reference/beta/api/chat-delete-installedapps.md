---
title: Desinstalar o aplicativo em um chat
description: Desinstale (remover) um aplicativo instalado em um chat.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3566191d894c2e98ccdb3d91c513f1581e6d6716
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971374"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="0d93e-103">Desinstalar o aplicativo em um chat</span><span class="sxs-lookup"><span data-stu-id="0d93e-103">Uninstall app in a chat</span></span>

<span data-ttu-id="0d93e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d93e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d93e-105">Desinstalar um [aplicativo](../resources/teamsapp.md) instalado em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="0d93e-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="0d93e-106">**Nota**: Se o chat estiver associado a uma instância [onlineMeeting](../resources/onlinemeeting.md), então, efetivamente, o **teamsApp** será removido da reunião.</span><span class="sxs-lookup"><span data-stu-id="0d93e-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d93e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d93e-107">Permissions</span></span>

<span data-ttu-id="0d93e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d93e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d93e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d93e-110">Permission type</span></span>      | <span data-ttu-id="0d93e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d93e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d93e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d93e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0d93e-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="0d93e-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="0d93e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d93e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d93e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d93e-115">Not supported.</span></span>   |
|<span data-ttu-id="0d93e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d93e-116">Application</span></span> | <span data-ttu-id="0d93e-117">Chat.Manage.Chat\*, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="0d93e-117">Chat.Manage.Chat\*, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

> <span data-ttu-id="0d93e-118">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="0d93e-118">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="0d93e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d93e-119">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="0d93e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d93e-120">Request headers</span></span>
|<span data-ttu-id="0d93e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0d93e-121">Name</span></span>|<span data-ttu-id="0d93e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d93e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0d93e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d93e-123">Authorization</span></span>|<span data-ttu-id="0d93e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d93e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d93e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d93e-126">Request body</span></span>
<span data-ttu-id="0d93e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d93e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d93e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d93e-128">Response</span></span>

<span data-ttu-id="0d93e-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d93e-129">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d93e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d93e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d93e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d93e-131">Request</span></span>

<span data-ttu-id="0d93e-132">O exemplo a seguir desinstala um aplicativo do chat especificado.</span><span class="sxs-lookup"><span data-stu-id="0d93e-132">The following example uninstalls an app from the specified chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d93e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d93e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```
# <a name="c"></a>[<span data-ttu-id="0d93e-134">C#</span><span class="sxs-lookup"><span data-stu-id="0d93e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d93e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d93e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d93e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d93e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d93e-137">Java</span><span class="sxs-lookup"><span data-stu-id="0d93e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d93e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d93e-138">Response</span></span>

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
