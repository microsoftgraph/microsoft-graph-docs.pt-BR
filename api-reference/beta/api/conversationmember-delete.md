---
title: Excluir conversationMember
description: Excluir um conversationMember de um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 739705d2c57210d15813ad8cbed4627afef29d07
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633877"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="feeed-103">Excluir conversationMember</span><span class="sxs-lookup"><span data-stu-id="feeed-103">Delete conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feeed-104">Excluir um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="feeed-104">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="feeed-105">Essa operação só é suportada em canais [](../resources/enums.md#channelmembershiptype-values) com channelMembershipType `private`de.</span><span class="sxs-lookup"><span data-stu-id="feeed-105">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="feeed-106">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="feeed-106">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="feeed-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="feeed-107">Permissions</span></span>

<span data-ttu-id="feeed-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="feeed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feeed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="feeed-110">Permission Type</span></span>|<span data-ttu-id="feeed-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="feeed-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="feeed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="feeed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="feeed-113">Para o **usuário** ou recurso de **chat** :</span><span class="sxs-lookup"><span data-stu-id="feeed-113">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="feeed-114">Chat. Read, chat. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="feeed-114">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="feeed-115">Para o recurso de **canal** :</span><span class="sxs-lookup"><span data-stu-id="feeed-115">For **channel** resource:</span></span><br/><span data-ttu-id="feeed-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feeed-116">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="feeed-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="feeed-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feeed-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="feeed-118">Not supported</span></span>|
|<span data-ttu-id="feeed-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="feeed-119">Application</span></span>| <span data-ttu-id="feeed-120">Para o **usuário** ou recurso de **chat** :</span><span class="sxs-lookup"><span data-stu-id="feeed-120">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="feeed-121">Chat. Read. All, chat. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="feeed-121">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="feeed-122">Para o recurso de **canal** :</span><span class="sxs-lookup"><span data-stu-id="feeed-122">For **channel** resource:</span></span><br/><span data-ttu-id="feeed-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feeed-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="feeed-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="feeed-124">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="feeed-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="feeed-125">Request headers</span></span>

| <span data-ttu-id="feeed-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="feeed-126">Header</span></span>       | <span data-ttu-id="feeed-127">Valor</span><span class="sxs-lookup"><span data-stu-id="feeed-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="feeed-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="feeed-128">Authorization</span></span>  | <span data-ttu-id="feeed-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feeed-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="feeed-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="feeed-131">Request body</span></span>

<span data-ttu-id="feeed-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="feeed-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="feeed-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="feeed-133">Response</span></span>

<span data-ttu-id="feeed-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="feeed-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="feeed-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="feeed-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="feeed-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="feeed-136">Request</span></span>

<span data-ttu-id="feeed-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feeed-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="feeed-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="feeed-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="feeed-139">C#</span><span class="sxs-lookup"><span data-stu-id="feeed-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="feeed-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="feeed-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="feeed-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="feeed-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="feeed-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="feeed-142">Response</span></span>

<span data-ttu-id="feeed-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="feeed-143">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
