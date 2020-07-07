---
title: Adicionar conversationMember
description: Adicionar um conversationMember a um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 40ed8afa7700bc2fa1639986c336d15130b03a57
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050751"
---
# <a name="add-conversationmember"></a><span data-ttu-id="1d4da-103">Adicionar conversationMember</span><span class="sxs-lookup"><span data-stu-id="1d4da-103">Add conversationMember</span></span>

<span data-ttu-id="1d4da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d4da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d4da-105">Adicionar um [conversationMember](../resources/conversationmember.md) a um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="1d4da-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

> [!NOTE]
><span data-ttu-id="1d4da-106">Essa operação só é suportada em canais com [channelMembershipType](../resources/enums.md#channelmembershiptype-values) de `private` .</span><span class="sxs-lookup"><span data-stu-id="1d4da-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="1d4da-107">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma resposta de solicitação inválida 400.</span><span class="sxs-lookup"><span data-stu-id="1d4da-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a 400 Bad Request response.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d4da-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d4da-108">Permissions</span></span>

<span data-ttu-id="1d4da-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1d4da-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1d4da-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d4da-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d4da-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d4da-111">Permission Type</span></span>|<span data-ttu-id="1d4da-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d4da-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="1d4da-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d4da-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1d4da-114">ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1d4da-114">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1d4da-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d4da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d4da-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d4da-116">Not supported.</span></span>|
|<span data-ttu-id="1d4da-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d4da-117">Application</span></span>| <span data-ttu-id="1d4da-118">ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1d4da-118">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d4da-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d4da-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="1d4da-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4da-120">Request headers</span></span>

| <span data-ttu-id="1d4da-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d4da-121">Header</span></span>       | <span data-ttu-id="1d4da-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1d4da-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1d4da-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d4da-123">Authorization</span></span>  | <span data-ttu-id="1d4da-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="1d4da-124">Bearer {token}.</span></span> <span data-ttu-id="1d4da-125">Required.</span><span class="sxs-lookup"><span data-stu-id="1d4da-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d4da-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4da-126">Request body</span></span>

<span data-ttu-id="1d4da-127">Inclua as propriedades a seguir no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d4da-127">Include the following properties in the request body.</span></span>

| <span data-ttu-id="1d4da-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d4da-128">Property</span></span>   | <span data-ttu-id="1d4da-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d4da-129">Type</span></span> |<span data-ttu-id="1d4da-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d4da-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d4da-131">funções</span><span class="sxs-lookup"><span data-stu-id="1d4da-131">roles</span></span>|<span data-ttu-id="1d4da-132">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4da-132">string collection</span></span>|<span data-ttu-id="1d4da-133">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="1d4da-133">The roles for that user.</span></span>|
|<span data-ttu-id="1d4da-134">usuário</span><span class="sxs-lookup"><span data-stu-id="1d4da-134">user</span></span>|[<span data-ttu-id="1d4da-135">usuário</span><span class="sxs-lookup"><span data-stu-id="1d4da-135">user</span></span>](../resources/user.md)|<span data-ttu-id="1d4da-136">O usuário a ser adicionado ao canal.</span><span class="sxs-lookup"><span data-stu-id="1d4da-136">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="1d4da-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d4da-137">Response</span></span>

<span data-ttu-id="1d4da-138">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d4da-138">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d4da-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d4da-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d4da-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4da-140">Request</span></span>

<span data-ttu-id="1d4da-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d4da-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d4da-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d4da-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="1d4da-143">C#</span><span class="sxs-lookup"><span data-stu-id="1d4da-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d4da-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d4da-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d4da-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d4da-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1d4da-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d4da-146">Response</span></span>

<span data-ttu-id="1d4da-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d4da-147">Here is an example of the response.</span></span>

><span data-ttu-id="1d4da-148">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="1d4da-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1d4da-149">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1d4da-149">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
