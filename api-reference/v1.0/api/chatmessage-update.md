---
title: Atualizar chatMessage
description: Atualizar a propriedade policyViolation de um chatMessage.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ee729e5285bfd6938329800d8bcedbf611391221
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115203"
---
# <a name="update-chatmessage"></a><span data-ttu-id="bdd28-103">Atualizar chatMessage</span><span class="sxs-lookup"><span data-stu-id="bdd28-103">Update chatMessage</span></span>

<span data-ttu-id="bdd28-104">Atualize [um objeto chatMessage.](../resources/chatMessage.md)</span><span class="sxs-lookup"><span data-stu-id="bdd28-104">Update a [chatMessage](../resources/chatMessage.md) object.</span></span> <span data-ttu-id="bdd28-105">Somente a **propriedade policyViolation** de um **chatMessage** pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="bdd28-105">Only the **policyViolation** property of a **chatMessage** can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd28-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdd28-106">Permissions</span></span>

<span data-ttu-id="bdd28-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdd28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdd28-109">Permission type</span></span>      | <span data-ttu-id="bdd28-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdd28-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdd28-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bdd28-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdd28-112">Not supported.</span></span> |
|<span data-ttu-id="bdd28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdd28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdd28-114">Not supported.</span></span>    |
|<span data-ttu-id="bdd28-115">Application</span><span class="sxs-lookup"><span data-stu-id="bdd28-115">Application</span></span> | <span data-ttu-id="bdd28-116">Chat.UpdatePolicyViolation.All para uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bdd28-116">Chat.UpdatePolicyViolation.All for a chat message.</span></span></br><span data-ttu-id="bdd28-117">ChannelMessage.UpdatePolicyViolation.All para uma mensagem de canal.</span><span class="sxs-lookup"><span data-stu-id="bdd28-117">ChannelMessage.UpdatePolicyViolation.All for a channel message.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdd28-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd28-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/(team-id)/channels/{channel-id}/messages/{message-id}
PATCH /chats/{chatThread-id}/messages/{message-id}
```

## <a name="request-headers"></a><span data-ttu-id="bdd28-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd28-119">Request headers</span></span>

| <span data-ttu-id="bdd28-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bdd28-120">Name</span></span>       | <span data-ttu-id="bdd28-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdd28-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="bdd28-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdd28-122">Authorization</span></span>  | <span data-ttu-id="bdd28-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdd28-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdd28-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdd28-125">Content-Type</span></span> | <span data-ttu-id="bdd28-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdd28-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdd28-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd28-128">Request body</span></span>

<span data-ttu-id="bdd28-129">No corpo da solicitação, fornece uma representação JSON de um objeto [chatMessage,](../resources/chatMessage.md) especificando apenas a **propriedade policyViolation.**</span><span class="sxs-lookup"><span data-stu-id="bdd28-129">In the request body, supply a JSON representation of a [chatMessage](../resources/chatMessage.md) object, specifying only the **policyViolation** property.</span></span>

## <a name="response"></a><span data-ttu-id="bdd28-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdd28-130">Response</span></span>

<span data-ttu-id="bdd28-131">Se bem-sucedido, este método retorna uma `200 OK` resposta.</span><span class="sxs-lookup"><span data-stu-id="bdd28-131">If successful, this method returns a `200 OK` response.</span></span>

## <a name="example"></a><span data-ttu-id="bdd28-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdd28-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdd28-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd28-133">Request</span></span>

<span data-ttu-id="bdd28-134">A seguir está um exemplo da solicitação para atualizar a **propriedade policyViolation** em uma mensagem de canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bdd28-134">The following is an example of the request to update the **policyViolation** property on a Microsoft Teams channel message.</span></span>


# <a name="http"></a>[<span data-ttu-id="bdd28-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd28-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chatMessage.PatchPolicyViolation.All"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
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
# <a name="c"></a>[<span data-ttu-id="bdd28-136">C#</span><span class="sxs-lookup"><span data-stu-id="bdd28-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chatmessagepatchpolicyviolationall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdd28-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdd28-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chatmessagepatchpolicyviolationall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdd28-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdd28-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chatmessagepatchpolicyviolationall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bdd28-139">Java</span><span class="sxs-lookup"><span data-stu-id="bdd28-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chatmessagepatchpolicyviolationall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="bdd28-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdd28-140">Response</span></span>

<span data-ttu-id="bdd28-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdd28-141">Here is an example of the response.</span></span>

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
