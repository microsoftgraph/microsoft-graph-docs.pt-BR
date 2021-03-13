---
title: Guia Atualizar no chat
description: Atualize as propriedades da guia especificada em um chat.
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ce831bafc46bd553da0c8e2d11af0e5c7303ff6a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777332"
---
# <a name="update-tab-in-chat"></a><span data-ttu-id="df402-103">Guia Atualizar no chat</span><span class="sxs-lookup"><span data-stu-id="df402-103">Update tab in chat</span></span>

<span data-ttu-id="df402-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df402-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df402-105">Atualize as propriedades da guia [especificada](../resources/teamstab.md) em um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="df402-105">Update the properties of the specified [tab](../resources/teamstab.md) in a [chat](../resources/chat.md).</span></span> <span data-ttu-id="df402-106">Isso pode ser usado para configurar o conteúdo da guia.</span><span class="sxs-lookup"><span data-stu-id="df402-106">This can be used to configure the content of the tab.</span></span>

> <span data-ttu-id="df402-107">**Observação**: se o chat estiver associado a uma instância [onlineMeeting,](../resources/onlinemeeting.md) então, efetivamente, a guia fixada na reunião será atualizada.</span><span class="sxs-lookup"><span data-stu-id="df402-107">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the tab pinned in the meeting will be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="df402-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="df402-108">Permissions</span></span>
<span data-ttu-id="df402-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df402-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="df402-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df402-111">Permission type</span></span>      | <span data-ttu-id="df402-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df402-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df402-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df402-113">Delegated (work or school account)</span></span> | <span data-ttu-id="df402-114">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df402-114">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="df402-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df402-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df402-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df402-116">Not supported.</span></span>    |
|<span data-ttu-id="df402-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df402-117">Application</span></span> | <span data-ttu-id="df402-118">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df402-118">TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="df402-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df402-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /chats/{chat-id}/tabs/{tab-id}
```

## <a name="request-headers"></a><span data-ttu-id="df402-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df402-120">Request headers</span></span>
| <span data-ttu-id="df402-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df402-121">Header</span></span>       | <span data-ttu-id="df402-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df402-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df402-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df402-123">Authorization</span></span>  | <span data-ttu-id="df402-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df402-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df402-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df402-126">Content-Type</span></span>  | <span data-ttu-id="df402-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df402-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df402-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df402-129">Request body</span></span>
<span data-ttu-id="df402-130">No corpo da solicitação, fornece uma representação JSON do [objeto tab.](../resources/teamstab.md)</span><span class="sxs-lookup"><span data-stu-id="df402-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df402-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="df402-131">Response</span></span>

<span data-ttu-id="df402-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e o recurso **teamsTab** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df402-132">If successful, this method returns a `200 OK` response code and the updated **teamsTab** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df402-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df402-133">Examples</span></span>
### <a name="example-1-update-the-name-of-a-tab-in-a-chat"></a><span data-ttu-id="df402-134">Exemplo 1: atualizar o nome de uma guia em um chat</span><span class="sxs-lookup"><span data-stu-id="df402-134">Example 1: Update the name of a tab in a chat</span></span>

#### <a name="request"></a><span data-ttu-id="df402-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df402-135">Request</span></span>
<span data-ttu-id="df402-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="df402-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tabs_in_chat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff
Content-type: application/json
Content-length: 211

{
  "displayName": "My Contoso Tab - updated again"
}
```


#### <a name="response"></a><span data-ttu-id="df402-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="df402-137">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="df402-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="df402-138">See also</span></span>

- [<span data-ttu-id="df402-139">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="df402-139">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="df402-140">Guia atualizar no canal</span><span class="sxs-lookup"><span data-stu-id="df402-140">Update tab in channel</span></span>](channel-patch-tabs.md)

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


