---
title: Atualizar chat
description: Atualize a propriedade policyViolation de um chat.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 938e642866ec6c4cee0a5322faff14ae597abc32
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992510"
---
# <a name="update-chatmessage"></a><span data-ttu-id="0b253-103">Atualizar chat</span><span class="sxs-lookup"><span data-stu-id="0b253-103">Update chatMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="0b253-104">Atualizar um objeto [chat](../resources/chatMessage.md) .</span><span class="sxs-lookup"><span data-stu-id="0b253-104">Update a [chatMessage](../resources/chatMessage.md) object.</span></span> <span data-ttu-id="0b253-105">Somente a propriedade **policyViolation** de um **chat** pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="0b253-105">Only the **policyViolation** property of a **chatMessage** can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b253-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b253-106">Permissions</span></span>

<span data-ttu-id="0b253-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b253-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b253-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b253-109">Permission type</span></span>      | <span data-ttu-id="0b253-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b253-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b253-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b253-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b253-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b253-112">Not supported.</span></span>    |
|<span data-ttu-id="0b253-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b253-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b253-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b253-114">Not supported.</span></span>    |
|<span data-ttu-id="0b253-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b253-115">Application</span></span> | <span data-ttu-id="0b253-116">Chat. UpdatePolicyViolation. All para uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="0b253-116">Chat.UpdatePolicyViolation.All for a chat message.</span></span></br><span data-ttu-id="0b253-117">ChannelMessage. UpdatePolicyViolation. All para uma mensagem de canal.</span><span class="sxs-lookup"><span data-stu-id="0b253-117">ChannelMessage.UpdatePolicyViolation.All for a channel message.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b253-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b253-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/(team-id)/channels/{channel-id}/chatMessages/{message-id}
PATCH /users/(user-id)/chats/{chatThread-id}/chatMessages/{message-id}
```

## <a name="request-headers"></a><span data-ttu-id="0b253-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b253-119">Request headers</span></span>

| <span data-ttu-id="0b253-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0b253-120">Name</span></span>       | <span data-ttu-id="0b253-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b253-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="0b253-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b253-122">Authorization</span></span>  | <span data-ttu-id="0b253-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b253-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b253-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b253-125">Content-Type</span></span> | <span data-ttu-id="0b253-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b253-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b253-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b253-128">Request body</span></span>

<span data-ttu-id="0b253-129">No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatMessage.md) , especificando apenas a propriedade **policyViolation** .</span><span class="sxs-lookup"><span data-stu-id="0b253-129">In the request body, supply a JSON representation of a [chatMessage](../resources/chatMessage.md) object, specifying only the **policyViolation** property.</span></span>

## <a name="response"></a><span data-ttu-id="0b253-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b253-130">Response</span></span>

<span data-ttu-id="0b253-131">Se tiver êxito, este método retornará uma `200 OK` resposta.</span><span class="sxs-lookup"><span data-stu-id="0b253-131">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="0b253-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b253-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b253-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b253-133">Request</span></span>

<span data-ttu-id="0b253-134">Veja a seguir um exemplo da solicitação para atualizar a propriedade **policyViolation** em uma mensagem de canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0b253-134">The following is an example of the request to update the **policyViolation** property on a Microsoft Teams channel message.</span></span>

<!-- {
  "blockType": "request",
  "name": "chatMessage.PatchPolicyViolation.All"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json
Content-Length: 248

{
  "policyViolation": {
    "policyTip": {
      "generalText" : "This item has been blocked by the administrator.",
      "complianceUrl" : "https://contoso.com/dlp-policy-page",
      "matchedConditionDescriptions" : ["Credit Card Number"]
    },
    "verdictDetails" : "AllowOverrideWithoutJustification,AllowFalsePositiveOverride",
    "dlpAction" : "BlockAccess"
  }
}
```

### <a name="response"></a><span data-ttu-id="0b253-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b253-135">Response</span></span>

<span data-ttu-id="0b253-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b253-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessage.UpdatePolicyViolation.All",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
