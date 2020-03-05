---
title: Atualizar conversationMember
description: Atualizar a função de um conversationMember em um canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b380d6c274c2d0ca2771cd44a7015f84f7d9a0e7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436416"
---
# <a name="update-conversationmember"></a><span data-ttu-id="2e24d-103">Atualizar conversationMember</span><span class="sxs-lookup"><span data-stu-id="2e24d-103">Update conversationMember</span></span>

<span data-ttu-id="2e24d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2e24d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e24d-105">Atualizar a função de um [conversationMember](../resources/conversationmember.md) em um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="2e24d-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="2e24d-106">Essa operação só é suportada em canais [](../resources/enums.md#channelmembershiptype-values) com channelMembershipType `private`de.</span><span class="sxs-lookup"><span data-stu-id="2e24d-106">This operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="2e24d-107">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="2e24d-107">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e24d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e24d-108">Permissions</span></span>

<span data-ttu-id="2e24d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e24d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e24d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e24d-111">Permission Type</span></span>|<span data-ttu-id="2e24d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e24d-112">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="2e24d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e24d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e24d-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e24d-114">Group.ReadWrite.All</span></span>|
|<span data-ttu-id="2e24d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e24d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e24d-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2e24d-116">Not supported</span></span>|
|<span data-ttu-id="2e24d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e24d-117">Application</span></span>|<span data-ttu-id="2e24d-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e24d-118">Group.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e24d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e24d-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e24d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e24d-120">Request headers</span></span>

| <span data-ttu-id="2e24d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e24d-121">Header</span></span>       | <span data-ttu-id="2e24d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2e24d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e24d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e24d-123">Authorization</span></span>  | <span data-ttu-id="2e24d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e24d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e24d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e24d-126">Request body</span></span>

<span data-ttu-id="2e24d-127">No corpo da solicitação, forneça os valores para os campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="2e24d-127">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="2e24d-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2e24d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2e24d-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2e24d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e24d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e24d-130">Property</span></span>   | <span data-ttu-id="2e24d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e24d-131">Type</span></span> |<span data-ttu-id="2e24d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e24d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e24d-133">funções</span><span class="sxs-lookup"><span data-stu-id="2e24d-133">roles</span></span>|<span data-ttu-id="2e24d-134">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e24d-134">string collection</span></span>|<span data-ttu-id="2e24d-135">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="2e24d-135">The roles for that user.</span></span> <span data-ttu-id="2e24d-136">Deve ser "proprietário" ou vazio.</span><span class="sxs-lookup"><span data-stu-id="2e24d-136">Must be "owner" or empty.</span></span> <span data-ttu-id="2e24d-137">Os usuários convidados devem sempre ter a função "convidado" e não podem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="2e24d-137">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="2e24d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e24d-138">Response</span></span>

<span data-ttu-id="2e24d-139">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e24d-139">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e24d-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e24d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e24d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e24d-141">Request</span></span>

<span data-ttu-id="2e24d-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e24d-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e24d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e24d-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2e24d-144">C#</span><span class="sxs-lookup"><span data-stu-id="2e24d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e24d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e24d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e24d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e24d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e24d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e24d-147">Response</span></span>

<span data-ttu-id="2e24d-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e24d-148">Here is an example of the response.</span></span>

><span data-ttu-id="2e24d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e24d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
