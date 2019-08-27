---
title: Atualizar conversationMember
description: Atualizar a função de um conversationMember em um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d1fad235333e968317d3e4681f56b501016d6352
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633866"
---
# <a name="update-conversationmember"></a><span data-ttu-id="3b557-103">Atualizar conversationMember</span><span class="sxs-lookup"><span data-stu-id="3b557-103">Update conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b557-104">Atualizar a função de um [conversationMember](../resources/conversationmember.md) em um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="3b557-104">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="3b557-105">Essa operação só é suportada em canais [](../resources/enums.md#channelmembershiptype-values) com channelMembershipType `private`de.</span><span class="sxs-lookup"><span data-stu-id="3b557-105">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="3b557-106">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="3b557-106">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b557-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b557-107">Permissions</span></span>

<span data-ttu-id="3b557-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b557-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b557-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b557-110">Permission Type</span></span>|<span data-ttu-id="3b557-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b557-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3b557-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b557-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b557-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b557-113">Group.ReadWrite.All</span></span>|
|<span data-ttu-id="3b557-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b557-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b557-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="3b557-115">Not supported</span></span>|
|<span data-ttu-id="3b557-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b557-116">Application</span></span>|<span data-ttu-id="3b557-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b557-117">Group.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b557-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b557-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3b557-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b557-119">Request headers</span></span>

| <span data-ttu-id="3b557-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b557-120">Header</span></span>       | <span data-ttu-id="3b557-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3b557-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3b557-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b557-122">Authorization</span></span>  | <span data-ttu-id="3b557-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b557-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3b557-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b557-125">Request body</span></span>

<span data-ttu-id="3b557-126">No corpo da solicitação, forneça os valores para os campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="3b557-126">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="3b557-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="3b557-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="3b557-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="3b557-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3b557-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b557-129">Property</span></span>   | <span data-ttu-id="3b557-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b557-130">Type</span></span> |<span data-ttu-id="3b557-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b557-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b557-132">funções</span><span class="sxs-lookup"><span data-stu-id="3b557-132">roles</span></span>|<span data-ttu-id="3b557-133">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b557-133">string collection</span></span>|<span data-ttu-id="3b557-134">As funções para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="3b557-134">The roles for that user.</span></span> <span data-ttu-id="3b557-135">Deve ser "proprietário" ou vazio.</span><span class="sxs-lookup"><span data-stu-id="3b557-135">Must be "owner" or empty.</span></span> <span data-ttu-id="3b557-136">Os usuários convidados devem sempre ter a função "convidado" e não podem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="3b557-136">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="3b557-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b557-137">Response</span></span>

<span data-ttu-id="3b557-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b557-138">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b557-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b557-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b557-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b557-140">Request</span></span>

<span data-ttu-id="3b557-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b557-141">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3b557-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b557-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "roles": ["owner"]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b557-143">C#</span><span class="sxs-lookup"><span data-stu-id="3b557-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b557-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b557-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b557-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3b557-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3b557-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b557-146">Response</span></span>

<span data-ttu-id="3b557-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b557-147">Here is an example of the response.</span></span>

><span data-ttu-id="3b557-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b557-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 475

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
