---
title: 'teamsAppInstallation: upgrade'
description: Atualize um aplicativo instalado em um chat e sincronize-o com a versão atual disponível no catálogo de aplicativos do locatário.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9da26926b9e41c7c4897744d9cb062a36003af4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776120"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="fb8fa-103">teamsAppInstallation: upgrade</span><span class="sxs-lookup"><span data-stu-id="fb8fa-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="fb8fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb8fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb8fa-105">Atualize uma [instalação de aplicativo](../resources/teamsappinstallation.md) em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="fb8fa-105">Upgrade an [app installation](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="fb8fa-106">**Observação**: se o chat estiver associado a uma instância do [onlineMeeting](../resources/onlinemeeting.md), em seguida, o **teamsApp** instalado na reunião será atualizado.</span><span class="sxs-lookup"><span data-stu-id="fb8fa-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then effectively, the **teamsApp** installed in the meeting will get upgraded.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb8fa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb8fa-107">Permissions</span></span>

<span data-ttu-id="fb8fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb8fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb8fa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb8fa-110">Permission type</span></span>      | <span data-ttu-id="fb8fa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb8fa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb8fa-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb8fa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fb8fa-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="fb8fa-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="fb8fa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb8fa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb8fa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb8fa-115">Not supported.</span></span>   |
|<span data-ttu-id="fb8fa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb8fa-116">Application</span></span> | <span data-ttu-id="fb8fa-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="fb8fa-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb8fa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb8fa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="response"></a><span data-ttu-id="fb8fa-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb8fa-119">Response</span></span>

<span data-ttu-id="fb8fa-120">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fb8fa-120">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb8fa-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb8fa-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb8fa-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb8fa-122">Request</span></span>

<span data-ttu-id="fb8fa-123">O exemplo a seguir atualiza um aplicativo instalado em um chat.</span><span class="sxs-lookup"><span data-stu-id="fb8fa-123">The following example upgrades an app installed in a chat.</span></span>

<!-- {
  "blockType": "request",
  "name": "upgrade_installedApps_in_chat"
}-->

```http
POST https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=/upgrade
```


### <a name="response"></a><span data-ttu-id="fb8fa-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb8fa-124">Response</span></span>

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
  "description": "Chat update installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
