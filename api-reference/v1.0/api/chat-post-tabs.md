---
title: Adicionar guia ao chat
description: 'Adiciona (pinos) uma guia ao chat especificado. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1056a2b04a684102b52f8544724cf0e8c6be1404
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960025"
---
# <a name="add-tab-to-chat"></a><span data-ttu-id="23626-103">Adicionar guia ao chat</span><span class="sxs-lookup"><span data-stu-id="23626-103">Add tab to chat</span></span>

<span data-ttu-id="23626-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23626-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23626-105">Adicione (pin) uma [guia](../resources/teamstab.md) ao chat [especificado.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="23626-105">Add (pin) a [tab](../resources/teamstab.md) to the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="23626-106">O aplicativo correspondente já deve [estar instalado no chat](../api/chat-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="23626-106">The corresponding app must already be [installed in the chat](../api/chat-list-installedapps.md).</span></span>

> <span data-ttu-id="23626-107">**Observação**: se o chat estiver associado a uma instância [onlineMeeting,](../resources/onlinemeeting.md) então, efetivamente, a guia será adicionada à reunião.</span><span class="sxs-lookup"><span data-stu-id="23626-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab will get added to the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="23626-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="23626-108">Permissions</span></span>
<span data-ttu-id="23626-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23626-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23626-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23626-111">Permission type</span></span>      | <span data-ttu-id="23626-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23626-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23626-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23626-113">Delegated (work or school account)</span></span> | <span data-ttu-id="23626-114">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23626-114">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="23626-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23626-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23626-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23626-116">Not supported.</span></span>    |
| <span data-ttu-id="23626-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23626-117">Application</span></span>                            | <span data-ttu-id="23626-118">TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23626-118">TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="23626-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23626-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /chats/{chat-id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="23626-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23626-120">Request headers</span></span>
| <span data-ttu-id="23626-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23626-121">Header</span></span>       | <span data-ttu-id="23626-122">Valor</span><span class="sxs-lookup"><span data-stu-id="23626-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="23626-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23626-123">Authorization</span></span>  | <span data-ttu-id="23626-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23626-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23626-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23626-126">Request body</span></span>

<span data-ttu-id="23626-127">No corpo da solicitação, inclua uma representação JSON de um [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="23626-127">In the request body include a JSON representation of a [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="23626-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="23626-128">Response</span></span>

<span data-ttu-id="23626-129">Se tiver êxito, este método retornará um código de resposta e uma `201 Created` instância do [recurso teamsTab](../resources/teamstab.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="23626-129">If successful, this method returns a `201 Created` response code and an instance of the [teamsTab](../resources/teamstab.md) resource in the body.</span></span>

## <a name="example"></a><span data-ttu-id="23626-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23626-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="23626-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23626-131">Request</span></span>

<span data-ttu-id="23626-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="23626-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="23626-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="23626-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_tab_to_chat"
}
-->

```http
POST https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs
Content-Type: application/json

{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="23626-134">C#</span><span class="sxs-lookup"><span data-stu-id="23626-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-tab-to-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23626-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23626-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-tab-to-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23626-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23626-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-tab-to-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23626-137">Java</span><span class="sxs-lookup"><span data-stu-id="23626-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-tab-to-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="23626-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="23626-138">Response</span></span>

<span data-ttu-id="23626-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="23626-139">The following is an example of the response.</span></span> 

><span data-ttu-id="23626-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="23626-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924"
}
```

## <a name="see-also"></a><span data-ttu-id="23626-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="23626-141">See also</span></span>

- [<span data-ttu-id="23626-142">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="23626-142">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="23626-143">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="23626-143">Add tab to channel</span></span>](channel-post-tabs.md)
- [<span data-ttu-id="23626-144">Adicionar o aplicativo ao chat</span><span class="sxs-lookup"><span data-stu-id="23626-144">Add app to chat</span></span>](chat-post-installedapps.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


