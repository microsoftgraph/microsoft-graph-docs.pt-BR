---
title: Obter o aplicativo instalado no chat
description: Obtenha o aplicativo instalado em um chat.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d5577c1dacf64f42888432785eebe9881563c425
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607469"
---
# <a name="get-installed-app-in-chat"></a><span data-ttu-id="f43e7-103">Obter o aplicativo instalado no chat</span><span class="sxs-lookup"><span data-stu-id="f43e7-103">Get installed app in chat</span></span>

<span data-ttu-id="f43e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f43e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f43e7-105">Obter um [aplicativo](../resources/teamsappinstallation.md) instalado em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="f43e7-105">Get an [app](../resources/teamsappinstallation.md) installed in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f43e7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f43e7-106">Permissions</span></span>

<span data-ttu-id="f43e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f43e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f43e7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f43e7-109">Permission type</span></span>      | <span data-ttu-id="f43e7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f43e7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f43e7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f43e7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f43e7-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="f43e7-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="f43e7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f43e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f43e7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f43e7-114">Not supported.</span></span>    |
|<span data-ttu-id="f43e7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f43e7-115">Application</span></span> | <span data-ttu-id="f43e7-116">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="f43e7-116">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f43e7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f43e7-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
GET /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="f43e7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f43e7-118">Request headers</span></span>

|<span data-ttu-id="f43e7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f43e7-119">Name</span></span>|<span data-ttu-id="f43e7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f43e7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f43e7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f43e7-121">Authorization</span></span>|<span data-ttu-id="f43e7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f43e7-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="f43e7-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f43e7-124">Response</span></span>

<span data-ttu-id="f43e7-125">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [TeamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f43e7-125">If successful, this method returns a `200 OK` and a [teamsApp](../resources/teamsapp.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="f43e7-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f43e7-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="f43e7-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f43e7-127">Request</span></span>

<span data-ttu-id="f43e7-128">O exemplo a seguir obtém um aplicativo instalado no chat especificado.</span><span class="sxs-lookup"><span data-stu-id="f43e7-128">The following example gets an app installed in the specified chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_installedApps_in_chat"
}-->

```http
GET https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps/MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```

### <a name="response"></a><span data-ttu-id="f43e7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f43e7-129">Response</span></span>

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
