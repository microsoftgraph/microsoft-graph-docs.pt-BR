---
title: Obter o aplicativo instalado no chat
description: Obtenha o aplicativo instalado em um chat.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f24a896c68ae0fc4a73208929ca0029c8eeb18f8
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971339"
---
# <a name="get-installed-app-in-chat"></a><span data-ttu-id="86254-103">Obter o aplicativo instalado no chat</span><span class="sxs-lookup"><span data-stu-id="86254-103">Get installed app in chat</span></span>

<span data-ttu-id="86254-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86254-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86254-105">Obter um [aplicativo](../resources/teamsappinstallation.md) instalado em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="86254-105">Get an [app](../resources/teamsappinstallation.md) installed in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86254-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="86254-106">Permissions</span></span>

<span data-ttu-id="86254-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86254-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86254-109">Permission type</span></span>      | <span data-ttu-id="86254-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86254-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86254-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86254-111">Delegated (work or school account)</span></span> | <span data-ttu-id="86254-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="86254-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="86254-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86254-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86254-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86254-114">Not supported.</span></span>    |
|<span data-ttu-id="86254-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86254-115">Application</span></span> | <span data-ttu-id="86254-116">TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="86254-116">TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

> <span data-ttu-id="86254-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="86254-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="86254-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86254-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
GET /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="86254-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86254-119">Request headers</span></span>

|<span data-ttu-id="86254-120">Nome</span><span class="sxs-lookup"><span data-stu-id="86254-120">Name</span></span>|<span data-ttu-id="86254-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="86254-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86254-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86254-122">Authorization</span></span>|<span data-ttu-id="86254-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86254-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="86254-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="86254-125">Response</span></span>

<span data-ttu-id="86254-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TeamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86254-126">If successful, this method returns a `200 OK` and a [teamsApp](../resources/teamsapp.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="86254-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86254-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="86254-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86254-128">Request</span></span>

<span data-ttu-id="86254-129">O exemplo a seguir obtém um aplicativo instalado no chat especificado.</span><span class="sxs-lookup"><span data-stu-id="86254-129">The following example gets an app installed in the specified chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="86254-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="86254-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installedApps_in_chat"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps/MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```
# <a name="c"></a>[<span data-ttu-id="86254-131">C#</span><span class="sxs-lookup"><span data-stu-id="86254-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86254-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86254-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86254-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86254-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86254-134">Java</span><span class="sxs-lookup"><span data-stu-id="86254-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86254-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="86254-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps/$entity",
    "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat get installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
