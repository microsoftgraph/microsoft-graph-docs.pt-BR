---
title: Adicionar guia ao chat
description: 'Adiciona (fixa) uma guia ao chat especificado. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6182daa44d0e5ac8deb86a1fb8fe61c5f1376b2f
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607459"
---
# <a name="add-tab-to-chat"></a><span data-ttu-id="9fff3-103">Adicionar guia ao chat</span><span class="sxs-lookup"><span data-stu-id="9fff3-103">Add tab to chat</span></span>

<span data-ttu-id="9fff3-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9fff3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fff3-105">Adicionar (fixar) uma [guia](../resources/teamstab.md) ao [chat](../resources/chat.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="9fff3-105">Add (pin) a [tab](../resources/teamstab.md) to the specified [chat](../resources/chat.md).</span></span> <span data-ttu-id="9fff3-106">O aplicativo correspondente já deve estar [instalado no chat](../api/chat-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="9fff3-106">The corresponding app must already be [installed in the chat](../api/chat-list-installedapps.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9fff3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9fff3-107">Permissions</span></span>
<span data-ttu-id="9fff3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fff3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fff3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fff3-110">Permission type</span></span>      | <span data-ttu-id="9fff3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fff3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fff3-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fff3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9fff3-113">TeamsTab. Create, TeamsTab. ReadWriteForChat, TeamsTab. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9fff3-113">TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All</span></span> |
|<span data-ttu-id="9fff3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fff3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fff3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fff3-115">Not supported.</span></span>    |
| <span data-ttu-id="9fff3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fff3-116">Application</span></span>                            | <span data-ttu-id="9fff3-117">TeamsTab. Create, TeamsTab. ReadWriteForChat. All, TeamsTab. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9fff3-117">TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="9fff3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fff3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /chats/{chat-id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="9fff3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fff3-119">Request headers</span></span>
| <span data-ttu-id="9fff3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fff3-120">Header</span></span>       | <span data-ttu-id="9fff3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9fff3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9fff3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fff3-122">Authorization</span></span>  | <span data-ttu-id="9fff3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fff3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9fff3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fff3-125">Request body</span></span>

<span data-ttu-id="9fff3-126">No corpo da solicitação, inclua uma representação JSON de um [teamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="9fff3-126">In the request body include a JSON representation of a [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="9fff3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fff3-127">Response</span></span>

<span data-ttu-id="9fff3-128">Se tiver êxito, este método retornará um `201 Created` código de resposta e uma instância do recurso [teamsTab](../resources/teamstab.md) no corpo.</span><span class="sxs-lookup"><span data-stu-id="9fff3-128">If successful, this method returns a `201 Created` response code and an instance of the [teamsTab](../resources/teamstab.md) resource in the body.</span></span>

## <a name="example"></a><span data-ttu-id="9fff3-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fff3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fff3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fff3-130">Request</span></span>

<span data-ttu-id="9fff3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fff3-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "add_tab_to_chat"
}
-->

```http
POST https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs
Content-Type: application/json

{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

### <a name="response"></a><span data-ttu-id="9fff3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fff3-132">Response</span></span>

<span data-ttu-id="9fff3-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9fff3-133">The following is an example of the response.</span></span> 

><span data-ttu-id="9fff3-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9fff3-134">**Note:** The response object shown here might be shortened for readability.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="9fff3-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="9fff3-135">See also</span></span>

- [<span data-ttu-id="9fff3-136">Configurar tipos de guia internos</span><span class="sxs-lookup"><span data-stu-id="9fff3-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
- [<span data-ttu-id="9fff3-137">Adicionar uma guia ao canal</span><span class="sxs-lookup"><span data-stu-id="9fff3-137">Add tab to channel</span></span>](channel-post-tabs.md)
- [<span data-ttu-id="9fff3-138">Adicionar aplicativo ao chat</span><span class="sxs-lookup"><span data-stu-id="9fff3-138">Add app to chat</span></span>](chat-post-installedapps.md)


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


