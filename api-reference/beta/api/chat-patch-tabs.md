---
title: Guia atualizar no chat
description: Atualiza as propriedades da guia especificada em um chat.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0225dd70a952d7d977c77c42595d19f7e671f9ff
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689802"
---
# <a name="update-tab-in-chat"></a><span data-ttu-id="b7b2a-103">Guia atualizar no chat</span><span class="sxs-lookup"><span data-stu-id="b7b2a-103">Update tab in chat</span></span>

<span data-ttu-id="b7b2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7b2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b2a-105">Atualiza as propriedades da [guia](../resources/teamstab.md) especificada em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="b7b2a-105">Update the properties of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> <span data-ttu-id="b7b2a-106">Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="b7b2a-106">This can be used to configure the content of the tab.</span></span>

> <span data-ttu-id="b7b2a-107">**Observação**: se o chat estiver associado a uma instância do [onlineMeeting](../resources/onlinemeeting.md) , em seguida, efetivamente, a guia fixa na reunião será atualizada.</span><span class="sxs-lookup"><span data-stu-id="b7b2a-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab pinned in the meeting will be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7b2a-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="b7b2a-108">Permissions</span></span>
<span data-ttu-id="b7b2a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7b2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b7b2a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7b2a-111">Permission type</span></span>      | <span data-ttu-id="b7b2a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7b2a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7b2a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7b2a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b7b2a-114">TeamsTab. ReadWriteForChat, TeamsTab. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7b2a-114">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="b7b2a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7b2a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7b2a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7b2a-116">Not supported.</span></span>    |
|<span data-ttu-id="b7b2a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7b2a-117">Application</span></span> | <span data-ttu-id="b7b2a-118">TeamsTab. ReadWriteForChat, TeamsTab. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b7b2a-118">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="b7b2a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b2a-119">HTTP request</span></span>
```http
PATCH /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="b7b2a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b2a-120">Request headers</span></span>
| <span data-ttu-id="b7b2a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7b2a-121">Header</span></span>       | <span data-ttu-id="b7b2a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7b2a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7b2a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7b2a-123">Authorization</span></span>  | <span data-ttu-id="b7b2a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7b2a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b7b2a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7b2a-126">Content-Type</span></span>  | <span data-ttu-id="b7b2a-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7b2a-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7b2a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b2a-129">Request body</span></span>
<span data-ttu-id="b7b2a-130">No corpo da solicitação, forneça uma representação JSON do objeto [Tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="b7b2a-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b7b2a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7b2a-131">Response</span></span>

<span data-ttu-id="b7b2a-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e o recurso **teamsTab** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7b2a-132">If successful, this method returns a `200 OK` response code and the updated **teamsTab** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b7b2a-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b7b2a-133">Examples</span></span>
### <a name="example-1-update-the-name-of-a-tab-in-a-chat"></a><span data-ttu-id="b7b2a-134">Exemplo 1: atualizar o nome de uma guia em um chat</span><span class="sxs-lookup"><span data-stu-id="b7b2a-134">Example 1: Update the name of a tab in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="b7b2a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b2a-135">Request</span></span>
<span data-ttu-id="b7b2a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7b2a-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7b2a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b2a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tabs_in_chat"
}-->
```http
PATCH https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated again"
}
```
# <a name="c"></a>[<span data-ttu-id="b7b2a-138">C#</span><span class="sxs-lookup"><span data-stu-id="b7b2a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tabs-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7b2a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7b2a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tabs-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7b2a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7b2a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tabs-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7b2a-141">Java</span><span class="sxs-lookup"><span data-stu-id="b7b2a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tabs-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b7b2a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7b2a-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab - updated again",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
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

## <a name="see-also"></a><span data-ttu-id="b7b2a-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="b7b2a-143">See also</span></span>

- [<span data-ttu-id="b7b2a-144">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="b7b2a-144">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="b7b2a-145">Guia atualizar no canal</span><span class="sxs-lookup"><span data-stu-id="b7b2a-145">Update tab in channel</span></span>](channel-patch-tabs.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update tab in chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


