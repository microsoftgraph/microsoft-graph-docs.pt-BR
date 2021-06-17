---
title: Adicionar o aplicativo ao chat
description: Instalar um aplicativo para chat.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c75d92e939e6bbc8661e0d71ffd210cc88a0070a
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971045"
---
# <a name="add-app-to-chat"></a><span data-ttu-id="bf4c8-103">Adicionar o aplicativo ao chat</span><span class="sxs-lookup"><span data-stu-id="bf4c8-103">Add app to chat</span></span>

<span data-ttu-id="bf4c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf4c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf4c8-105">Instale um [teamsApp](../resources/teamsapp.md) para o [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="bf4c8-105">Install a [teamsApp](../resources/teamsapp.md) to the specified [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="bf4c8-106">**Observação**: Se o chat estiver associado a uma instância [onlineMeeting](../resources/onlinemeeting.md), então, efetivamente, o **teamsApp** será instalado na reunião.</span><span class="sxs-lookup"><span data-stu-id="bf4c8-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get installed to the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf4c8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf4c8-107">Permissions</span></span>

<span data-ttu-id="bf4c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf4c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf4c8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf4c8-110">Permission type</span></span>      | <span data-ttu-id="bf4c8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf4c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf4c8-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf4c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bf4c8-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="bf4c8-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="bf4c8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf4c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf4c8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf4c8-115">Not supported.</span></span>    |
|<span data-ttu-id="bf4c8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf4c8-116">Application</span></span> | <span data-ttu-id="bf4c8-117">Chat.Manage.Chat\*, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="bf4c8-117">Chat.Manage.Chat\*, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

> <span data-ttu-id="bf4c8-118">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bf4c8-118">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="bf4c8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf4c8-119">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
POST /chats/{chat-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="bf4c8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf4c8-120">Request headers</span></span>

| <span data-ttu-id="bf4c8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf4c8-121">Header</span></span>       | <span data-ttu-id="bf4c8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bf4c8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf4c8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf4c8-123">Authorization</span></span>  | <span data-ttu-id="bf4c8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf4c8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf4c8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf4c8-126">Content-Type</span></span>  | <span data-ttu-id="bf4c8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf4c8-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf4c8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf4c8-129">Request body</span></span>

<span data-ttu-id="bf4c8-p104">O corpo da solicitação deve conter a ID do aplicativo gerado pelo aplicativo de catálogo. Para obter detalhes, confira [teamsApp properties](../resources/teamsapp.md#properties).</span><span class="sxs-lookup"><span data-stu-id="bf4c8-p104">The request body should contain the catalog app's generated app ID. For details, see [teamsApp properties](../resources/teamsapp.md#properties).</span></span>

## <a name="response"></a><span data-ttu-id="bf4c8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf4c8-132">Response</span></span>

<span data-ttu-id="bf4c8-133">Se tiver êxito, este método retornará um código de resposta `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="bf4c8-133">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bf4c8-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bf4c8-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf4c8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf4c8-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bf4c8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf4c8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_app_in_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps
Content-Type: application/json

{
"teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="bf4c8-137">C#</span><span class="sxs-lookup"><span data-stu-id="bf4c8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-app-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bf4c8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bf4c8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-app-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bf4c8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf4c8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-app-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bf4c8-140">Java</span><span class="sxs-lookup"><span data-stu-id="bf4c8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-app-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bf4c8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf4c8-141">Response</span></span>

<!-- {
  "blockType": "response"
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
