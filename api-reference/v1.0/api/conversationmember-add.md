---
title: Adicionar conversationMember
description: Adicionar conversationMember a um canal.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ad99b8906a5ad71b7fa77b1d19bf32e5b01757a0
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060614"
---
# <a name="add-conversationmember"></a><span data-ttu-id="567cf-103">Adicionar conversationMember</span><span class="sxs-lookup"><span data-stu-id="567cf-103">Add conversationMember</span></span>

<span data-ttu-id="567cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="567cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="567cf-105">Adicionar uma [conversaMember](../resources/conversationmember.md) a um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="567cf-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="567cf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="567cf-106">Permissions</span></span>

<span data-ttu-id="567cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="567cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="567cf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="567cf-109">Permission Type</span></span>|<span data-ttu-id="567cf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="567cf-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="567cf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="567cf-111">Delegated (work or school account)</span></span>| <span data-ttu-id="567cf-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="567cf-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="567cf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="567cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="567cf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="567cf-114">Not supported.</span></span>|
|<span data-ttu-id="567cf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="567cf-115">Application</span></span>| <span data-ttu-id="567cf-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="567cf-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="567cf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="567cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="567cf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="567cf-118">Request headers</span></span>

| <span data-ttu-id="567cf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="567cf-119">Header</span></span>       | <span data-ttu-id="567cf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="567cf-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="567cf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="567cf-121">Authorization</span></span>  | <span data-ttu-id="567cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="567cf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="567cf-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="567cf-124">Request body</span></span>

<span data-ttu-id="567cf-125">Inclua as propriedades a seguir no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="567cf-125">Include the following properties in the request body.</span></span>

| <span data-ttu-id="567cf-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="567cf-126">Property</span></span>   | <span data-ttu-id="567cf-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="567cf-127">Type</span></span> |<span data-ttu-id="567cf-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="567cf-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="567cf-129">funções</span><span class="sxs-lookup"><span data-stu-id="567cf-129">roles</span></span>|<span data-ttu-id="567cf-130">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="567cf-130">string collection</span></span>|<span data-ttu-id="567cf-131">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="567cf-131">The roles for that user.</span></span>|
|<span data-ttu-id="567cf-132">usuário</span><span class="sxs-lookup"><span data-stu-id="567cf-132">user</span></span>|[<span data-ttu-id="567cf-133">user</span><span class="sxs-lookup"><span data-stu-id="567cf-133">user</span></span>](../resources/user.md)|<span data-ttu-id="567cf-134">O usuário a ser acrescentado ao canal.</span><span class="sxs-lookup"><span data-stu-id="567cf-134">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="567cf-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="567cf-135">Response</span></span>

<span data-ttu-id="567cf-136">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="567cf-136">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="567cf-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="567cf-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="567cf-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="567cf-138">Request</span></span>

<span data-ttu-id="567cf-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="567cf-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="567cf-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="567cf-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="567cf-141">C#</span><span class="sxs-lookup"><span data-stu-id="567cf-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="567cf-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="567cf-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="567cf-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="567cf-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="567cf-144">Java</span><span class="sxs-lookup"><span data-stu-id="567cf-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="567cf-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="567cf-145">Response</span></span>

<span data-ttu-id="567cf-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="567cf-146">Here is an example of the response.</span></span>

><span data-ttu-id="567cf-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="567cf-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/V1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
