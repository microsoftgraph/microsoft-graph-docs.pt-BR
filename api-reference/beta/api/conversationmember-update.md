---
title: Atualizar conversationMember
description: Atualizar a função de um conversationMember em uma equipe ou canal.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb67a3ec07a7f22d40beea9d9831ea486e338ebe
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091386"
---
# <a name="update-conversationmember"></a><span data-ttu-id="73f6b-103">Atualizar conversationMember</span><span class="sxs-lookup"><span data-stu-id="73f6b-103">Update conversationMember</span></span>

<span data-ttu-id="73f6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73f6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73f6b-105">Atualizar a função de um [conversationMember](../resources/conversationmember.md) em uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="73f6b-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>
<span data-ttu-id="73f6b-106">ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="73f6b-106">or [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="73f6b-107">Em canais, essa operação só é suportada em canais com um [channelMembershipType](../resources/enums.md#channelmembershiptype-values) de `private` .</span><span class="sxs-lookup"><span data-stu-id="73f6b-107">On channels, this operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="73f6b-108">Chamadas com qualquer outro [channelMembershipType](../resources/enums.md#channelmembershiptype-values) retornará uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="73f6b-108">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="73f6b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="73f6b-109">Permissions</span></span>

<span data-ttu-id="73f6b-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="73f6b-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="73f6b-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73f6b-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73f6b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73f6b-112">Permission Type</span></span>|<span data-ttu-id="73f6b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73f6b-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="73f6b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73f6b-114">Delegated (work or school account)</span></span>| <span data-ttu-id="73f6b-115">No Teams: TeamMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="73f6b-115">In teams: TeamMember.ReadWrite.All.</span></span> <span data-ttu-id="73f6b-116">Em canais: ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="73f6b-116">In channels: ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All.</span></span> |
|<span data-ttu-id="73f6b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73f6b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73f6b-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73f6b-118">Not supported</span></span>|
|<span data-ttu-id="73f6b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73f6b-119">Application</span></span>| <span data-ttu-id="73f6b-120">No Teams: TeamMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="73f6b-120">In teams: TeamMember.ReadWrite.All.</span></span> <span data-ttu-id="73f6b-121">Em canais: ChannelMember. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="73f6b-121">In channels:  ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73f6b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73f6b-122">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="73f6b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73f6b-123">Request headers</span></span>

| <span data-ttu-id="73f6b-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73f6b-124">Header</span></span>       | <span data-ttu-id="73f6b-125">Valor</span><span class="sxs-lookup"><span data-stu-id="73f6b-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73f6b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="73f6b-126">Authorization</span></span>  | <span data-ttu-id="73f6b-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="73f6b-127">Bearer {token}.</span></span> <span data-ttu-id="73f6b-128">Required.</span><span class="sxs-lookup"><span data-stu-id="73f6b-128">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73f6b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73f6b-129">Request body</span></span>

<span data-ttu-id="73f6b-130">No corpo da solicitação, forneça os valores para os campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="73f6b-130">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="73f6b-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="73f6b-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="73f6b-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="73f6b-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="73f6b-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73f6b-133">Property</span></span>   | <span data-ttu-id="73f6b-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="73f6b-134">Type</span></span> |<span data-ttu-id="73f6b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="73f6b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73f6b-136">funções</span><span class="sxs-lookup"><span data-stu-id="73f6b-136">roles</span></span>|<span data-ttu-id="73f6b-137">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73f6b-137">string collection</span></span>|<span data-ttu-id="73f6b-138">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="73f6b-138">The roles for that user.</span></span> <span data-ttu-id="73f6b-139">Deve ser "proprietário" ou vazio.</span><span class="sxs-lookup"><span data-stu-id="73f6b-139">Must be "owner" or empty.</span></span> <span data-ttu-id="73f6b-140">Os usuários convidados devem sempre ter a função "convidado" e não podem ser alterados.</span><span class="sxs-lookup"><span data-stu-id="73f6b-140">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="73f6b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="73f6b-141">Response</span></span>

<span data-ttu-id="73f6b-142">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73f6b-142">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73f6b-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73f6b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="73f6b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73f6b-144">Request</span></span>

<span data-ttu-id="73f6b-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73f6b-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73f6b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="73f6b-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="73f6b-147">C#</span><span class="sxs-lookup"><span data-stu-id="73f6b-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73f6b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73f6b-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73f6b-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73f6b-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73f6b-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="73f6b-150">Response</span></span>

<span data-ttu-id="73f6b-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73f6b-151">Here is an example of the response.</span></span>

><span data-ttu-id="73f6b-152">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="73f6b-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="73f6b-153">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="73f6b-153">All the properties will be returned from an actual call.</span></span>
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
