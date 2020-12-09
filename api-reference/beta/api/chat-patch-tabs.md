---
title: Guia atualizar no chat
description: Atualiza as propriedades da guia especificada em um chat.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e7b8a1bb20b9e80dc8e86768ae5edf3216090287
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607455"
---
# <a name="update-tab-in-chat"></a><span data-ttu-id="9962f-103">Guia atualizar no chat</span><span class="sxs-lookup"><span data-stu-id="9962f-103">Update tab in chat</span></span>

<span data-ttu-id="9962f-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9962f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9962f-105">Atualiza as propriedades da [guia](../resources/teamstab.md) especificada em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="9962f-105">Update the properties of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> <span data-ttu-id="9962f-106">Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="9962f-106">This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="9962f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9962f-107">Permissions</span></span>
<span data-ttu-id="9962f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9962f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9962f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9962f-110">Permission type</span></span>      | <span data-ttu-id="9962f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9962f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9962f-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9962f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9962f-113">TeamsTab. ReadWriteForChat, TeamsTab. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9962f-113">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="9962f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9962f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9962f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9962f-115">Not supported.</span></span>    |
|<span data-ttu-id="9962f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9962f-116">Application</span></span> | <span data-ttu-id="9962f-117">TeamsTab. ReadWriteForChat, TeamsTab. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9962f-117">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="9962f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9962f-118">HTTP request</span></span>
```http
PATCH /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="9962f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9962f-119">Request headers</span></span>
| <span data-ttu-id="9962f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9962f-120">Header</span></span>       | <span data-ttu-id="9962f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9962f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9962f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9962f-122">Authorization</span></span>  | <span data-ttu-id="9962f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9962f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9962f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9962f-125">Content-Type</span></span>  | <span data-ttu-id="9962f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9962f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9962f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9962f-128">Request body</span></span>
<span data-ttu-id="9962f-129">No corpo da solicitação, forneça uma representação JSON do objeto [Tab](../resources/teamstab.md) .</span><span class="sxs-lookup"><span data-stu-id="9962f-129">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9962f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9962f-130">Response</span></span>

<span data-ttu-id="9962f-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e o recurso **teamsTab** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9962f-131">If successful, this method returns a `200 OK` response code and the updated **teamsTab** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9962f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9962f-132">Examples</span></span>
### <a name="example-1-update-the-name-of-a-tab-in-a-chat"></a><span data-ttu-id="9962f-133">Exemplo 1: atualizar o nome de uma guia em um chat</span><span class="sxs-lookup"><span data-stu-id="9962f-133">Example 1: Update the name of a tab in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="9962f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9962f-134">Request</span></span>
<span data-ttu-id="9962f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9962f-135">The following is an example of the request.</span></span>
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
#### <a name="response"></a><span data-ttu-id="9962f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9962f-136">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9962f-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="9962f-137">See also</span></span>

- [<span data-ttu-id="9962f-138">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="9962f-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="9962f-139">Guia atualizar no canal</span><span class="sxs-lookup"><span data-stu-id="9962f-139">Update tab in channel</span></span>](channel-patch-tabs.md)

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


