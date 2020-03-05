---
title: Excluir conversationMember
description: Excluir um conversationMember de um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a6ac8b72f5dea24c0f60062b91dac7648b91e85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436563"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="db632-103">Excluir conversationMember</span><span class="sxs-lookup"><span data-stu-id="db632-103">Delete conversationMember</span></span>

<span data-ttu-id="db632-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="db632-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db632-105">Excluir um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="db632-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="db632-106">Essa operação só é suportada em canais [](../resources/enums.md#channelmembershiptype-values) com channelMembershipType `private`de.</span><span class="sxs-lookup"><span data-stu-id="db632-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="db632-107">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="db632-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="db632-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="db632-108">Permissions</span></span>

<span data-ttu-id="db632-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db632-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db632-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db632-111">Permission Type</span></span>|<span data-ttu-id="db632-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db632-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="db632-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db632-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db632-114">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="db632-114">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="db632-115">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db632-115">Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="db632-116">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="db632-116">For **channel** resource:</span></span><br/><span data-ttu-id="db632-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db632-117">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="db632-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db632-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db632-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="db632-119">Not supported</span></span>|
|<span data-ttu-id="db632-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db632-120">Application</span></span>| <span data-ttu-id="db632-121">Para o recurso de **usuário** ou **chat** :</span><span class="sxs-lookup"><span data-stu-id="db632-121">For **user** or **chat** resource:</span></span><br/><span data-ttu-id="db632-122">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db632-122">Chat.Read.All, Chat.ReadWrite.All</span></span><br/><br/><span data-ttu-id="db632-123">Para o recurso de **canal**:</span><span class="sxs-lookup"><span data-stu-id="db632-123">For **channel** resource:</span></span><br/><span data-ttu-id="db632-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db632-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db632-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db632-125">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db632-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db632-126">Request headers</span></span>

| <span data-ttu-id="db632-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db632-127">Header</span></span>       | <span data-ttu-id="db632-128">Valor</span><span class="sxs-lookup"><span data-stu-id="db632-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="db632-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="db632-129">Authorization</span></span>  | <span data-ttu-id="db632-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db632-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db632-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db632-132">Request body</span></span>

<span data-ttu-id="db632-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="db632-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db632-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="db632-134">Response</span></span>

<span data-ttu-id="db632-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="db632-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db632-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db632-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="db632-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db632-137">Request</span></span>

<span data-ttu-id="db632-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db632-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db632-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="db632-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="db632-140">C#</span><span class="sxs-lookup"><span data-stu-id="db632-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db632-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db632-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db632-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db632-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db632-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="db632-143">Response</span></span>

<span data-ttu-id="db632-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db632-144">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
