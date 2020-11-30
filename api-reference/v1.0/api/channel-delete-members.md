---
title: Remover membro do canal
description: Remover um membro de um canal.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e0f9d8a17403b1d4d7833abcc3f3bdcb69bee741
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387812"
---
# <a name="remove-member-from-channel"></a><span data-ttu-id="be960-103">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="be960-103">Remove member from channel</span></span>

<span data-ttu-id="be960-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be960-104">Namespace: microsoft.graph</span></span>
 
<span data-ttu-id="be960-105">Excluir um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="be960-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span> <span data-ttu-id="be960-106">Essa operação só é permitida para canais com um valor de **membershiptype** de `private` .</span><span class="sxs-lookup"><span data-stu-id="be960-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>


## <a name="permissions"></a><span data-ttu-id="be960-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="be960-107">Permissions</span></span>

<span data-ttu-id="be960-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be960-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be960-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be960-110">Permission Type</span></span>|<span data-ttu-id="be960-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be960-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="be960-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be960-112">Delegated (work or school account)</span></span>| <span data-ttu-id="be960-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be960-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="be960-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be960-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be960-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be960-115">Not supported.</span></span>|
|<span data-ttu-id="be960-116">Application</span><span class="sxs-lookup"><span data-stu-id="be960-116">Application</span></span>| <span data-ttu-id="be960-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be960-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be960-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be960-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->

```http
DELETE /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="be960-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be960-119">Request headers</span></span>

| <span data-ttu-id="be960-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be960-120">Header</span></span>       | <span data-ttu-id="be960-121">Valor</span><span class="sxs-lookup"><span data-stu-id="be960-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be960-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="be960-122">Authorization</span></span>  | <span data-ttu-id="be960-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be960-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be960-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be960-125">Request body</span></span>

<span data-ttu-id="be960-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be960-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be960-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="be960-127">Response</span></span>

<span data-ttu-id="be960-128">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="be960-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="be960-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be960-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="be960-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be960-130">Request</span></span>

<span data-ttu-id="be960-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be960-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_channel-member"
} -->
```http
DELETE https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```

### <a name="response"></a><span data-ttu-id="be960-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="be960-132">Response</span></span>

<span data-ttu-id="be960-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be960-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="be960-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="be960-134">See also</span></span>

- [<span data-ttu-id="be960-135">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="be960-135">Remove member from team</span></span>](team-delete-members.md)

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
