---
title: Remover membro do canal
description: Remova um membro de um canal.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5602b45557fa8da4a237cb113b2cb72690e31e19
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059969"
---
# <a name="remove-member-from-channel"></a><span data-ttu-id="031e4-103">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="031e4-103">Remove member from channel</span></span>

<span data-ttu-id="031e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="031e4-104">Namespace: microsoft.graph</span></span>
 
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="031e4-105">Excluir uma [conversaMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="031e4-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span> <span data-ttu-id="031e4-106">Essa operação só é permitida para canais com **um valor membershipType** de `private` .</span><span class="sxs-lookup"><span data-stu-id="031e4-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>


## <a name="permissions"></a><span data-ttu-id="031e4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="031e4-107">Permissions</span></span>

<span data-ttu-id="031e4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="031e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="031e4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="031e4-110">Permission Type</span></span>|<span data-ttu-id="031e4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="031e4-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="031e4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="031e4-112">Delegated (work or school account)</span></span>| <span data-ttu-id="031e4-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="031e4-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="031e4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="031e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="031e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="031e4-115">Not supported.</span></span>|
|<span data-ttu-id="031e4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="031e4-116">Application</span></span>| <span data-ttu-id="031e4-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="031e4-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="031e4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="031e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->

```http
DELETE /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="031e4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="031e4-119">Request headers</span></span>

| <span data-ttu-id="031e4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="031e4-120">Header</span></span>       | <span data-ttu-id="031e4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="031e4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="031e4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="031e4-122">Authorization</span></span>  | <span data-ttu-id="031e4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="031e4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="031e4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="031e4-125">Request body</span></span>

<span data-ttu-id="031e4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="031e4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="031e4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="031e4-127">Response</span></span>

<span data-ttu-id="031e4-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="031e4-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="031e4-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="031e4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="031e4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="031e4-130">Request</span></span>

<span data-ttu-id="031e4-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="031e4-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="031e4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="031e4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel-member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="031e4-133">C#</span><span class="sxs-lookup"><span data-stu-id="031e4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="031e4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="031e4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="031e4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="031e4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="031e4-136">Java</span><span class="sxs-lookup"><span data-stu-id="031e4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="031e4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="031e4-137">Response</span></span>

<span data-ttu-id="031e4-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="031e4-138">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="031e4-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="031e4-139">See also</span></span>

- [<span data-ttu-id="031e4-140">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="031e4-140">Remove member from team</span></span>](team-delete-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete_channel_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

