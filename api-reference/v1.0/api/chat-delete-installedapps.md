---
title: Desinstalar o aplicativo em um chat
description: Desinstale (remover) um aplicativo instalado em um chat.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a0cf8814fac6d99c3c71099bb7902a7ad4c6ed4c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777598"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="f473a-103">Desinstalar o aplicativo em um chat</span><span class="sxs-lookup"><span data-stu-id="f473a-103">Uninstall app in a chat</span></span>

<span data-ttu-id="f473a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f473a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f473a-105">Desinstalar um [aplicativo](../resources/teamsapp.md) instalado em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="f473a-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="f473a-106">**Nota**: Se o chat estiver associado a uma instância [onlineMeeting](../resources/onlinemeeting.md), então, efetivamente, o **teamsApp** será removido da reunião.</span><span class="sxs-lookup"><span data-stu-id="f473a-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="f473a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f473a-107">Permissions</span></span>

<span data-ttu-id="f473a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f473a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f473a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f473a-110">Permission type</span></span>      | <span data-ttu-id="f473a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f473a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f473a-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f473a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f473a-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="f473a-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="f473a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f473a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f473a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f473a-115">Not supported.</span></span>   |
|<span data-ttu-id="f473a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f473a-116">Application</span></span> | <span data-ttu-id="f473a-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="f473a-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f473a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f473a-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="f473a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f473a-119">Request headers</span></span>
|<span data-ttu-id="f473a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f473a-120">Name</span></span>|<span data-ttu-id="f473a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f473a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f473a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f473a-122">Authorization</span></span>|<span data-ttu-id="f473a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f473a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f473a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f473a-125">Request body</span></span>
<span data-ttu-id="f473a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f473a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f473a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f473a-127">Response</span></span>

<span data-ttu-id="f473a-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f473a-128">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f473a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f473a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f473a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f473a-130">Request</span></span>

<span data-ttu-id="f473a-131">O exemplo a seguir desinstala um aplicativo do chat especificado.</span><span class="sxs-lookup"><span data-stu-id="f473a-131">The following example uninstalls an app from the specified chat.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```


### <a name="response"></a><span data-ttu-id="f473a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f473a-132">Response</span></span>

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
