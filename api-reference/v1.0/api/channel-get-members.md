---
title: Obter membro de um canal
description: Obter membro de um canal.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6aeb2f24822995e9e2a9d9e153182842b8d99ff
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060559"
---
# <a name="get-member-of-channel"></a><span data-ttu-id="8cf30-103">Obter membro de um canal</span><span class="sxs-lookup"><span data-stu-id="8cf30-103">Get member of channel</span></span>

<span data-ttu-id="8cf30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cf30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8cf30-105">Obter um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8cf30-105">Get a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8cf30-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8cf30-106">Permissions</span></span>

<span data-ttu-id="8cf30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cf30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cf30-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cf30-109">Permission Type</span></span>|<span data-ttu-id="8cf30-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cf30-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="8cf30-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cf30-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8cf30-112">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cf30-112">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="8cf30-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cf30-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cf30-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cf30-114">Not supported.</span></span>|
|<span data-ttu-id="8cf30-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cf30-115">Application</span></span>|<span data-ttu-id="8cf30-116">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cf30-116">ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="8cf30-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cf30-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
GET /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8cf30-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8cf30-118">Optional query parameters</span></span>

<span data-ttu-id="8cf30-119">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8cf30-119">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cf30-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf30-120">Request headers</span></span>

| <span data-ttu-id="8cf30-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cf30-121">Header</span></span>       | <span data-ttu-id="8cf30-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8cf30-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8cf30-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cf30-123">Authorization</span></span>  | <span data-ttu-id="8cf30-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cf30-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8cf30-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf30-126">Request body</span></span>

<span data-ttu-id="8cf30-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8cf30-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cf30-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cf30-128">Response</span></span>

<span data-ttu-id="8cf30-129">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cf30-129">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cf30-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cf30-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cf30-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf30-131">Request</span></span>

<span data-ttu-id="8cf30-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cf30-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8cf30-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cf30-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "channel-get_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="8cf30-134">C#</span><span class="sxs-lookup"><span data-stu-id="8cf30-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-get-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cf30-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cf30-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-get-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cf30-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cf30-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-get-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cf30-137">Java</span><span class="sxs-lookup"><span data-stu-id="8cf30-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-get-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8cf30-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cf30-138">Response</span></span>

<span data-ttu-id="8cf30-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cf30-139">Here is an example of the response.</span></span>

><span data-ttu-id="8cf30-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8cf30-140">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
   "@odata.type":"#microsoft.graph.aadUserConversationMember",
   "id":"ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
   "roles":[
      "owner"
   ],
   "displayName":"John Doe",
   "userId":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
   "email":null
}
```

## <a name="see-also"></a><span data-ttu-id="8cf30-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="8cf30-141">See also</span></span>

- [<span data-ttu-id="8cf30-142">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="8cf30-142">Get member of team</span></span>](team-get-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "get_channel_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
