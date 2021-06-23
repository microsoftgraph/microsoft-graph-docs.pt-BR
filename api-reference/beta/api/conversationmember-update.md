---
title: Atualizar conversationMember
description: Atualize a função de um conversationMember em uma equipe ou canal.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 01f477c74e46876eae38c8d8d622a1a179671a5d
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059902"
---
# <a name="update-conversationmember"></a><span data-ttu-id="1c27d-103">Atualizar conversationMember</span><span class="sxs-lookup"><span data-stu-id="1c27d-103">Update conversationMember</span></span>

<span data-ttu-id="1c27d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c27d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c27d-105">Atualize a função de [um conversationMember](../resources/conversationmember.md) em uma [equipe.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="1c27d-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>
<span data-ttu-id="1c27d-106">ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="1c27d-106">or [channel](../resources/channel.md).</span></span>

> [!NOTE]
> <span data-ttu-id="1c27d-107">Nos canais, essa operação só é suportada em canais com [um channelMembershipType](../resources/enums.md#channelmembershiptype-values) de `private` .</span><span class="sxs-lookup"><span data-stu-id="1c27d-107">On channels, this operation is only supported on channels with a [channelMembershipType](../resources/enums.md#channelmembershiptype-values) of `private`.</span></span> <span data-ttu-id="1c27d-108">Chamadas com qualquer outro [canalMembershipType](../resources/enums.md#channelmembershiptype-values) retornarão uma `400 Bad Request` resposta.</span><span class="sxs-lookup"><span data-stu-id="1c27d-108">Calls with any other [channelMembershipType](../resources/enums.md#channelmembershiptype-values) will return a `400 Bad Request` response.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c27d-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c27d-109">Permissions</span></span>

<span data-ttu-id="1c27d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c27d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c27d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c27d-112">Permission Type</span></span>|<span data-ttu-id="1c27d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c27d-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="1c27d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c27d-114">Delegated (work or school account)</span></span>| <span data-ttu-id="1c27d-115">Em equipes: TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c27d-115">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="1c27d-116">Em canais: ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c27d-116">In channels: ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="1c27d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c27d-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c27d-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1c27d-118">Not supported</span></span>|
|<span data-ttu-id="1c27d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c27d-119">Application</span></span>| <span data-ttu-id="1c27d-120">Em equipes: TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c27d-120">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="1c27d-121">Em canais: ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c27d-121">In channels:  ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c27d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c27d-122">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/members/{id}
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1c27d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c27d-123">Request headers</span></span>

| <span data-ttu-id="1c27d-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c27d-124">Header</span></span>       | <span data-ttu-id="1c27d-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1c27d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1c27d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c27d-126">Authorization</span></span>  | <span data-ttu-id="1c27d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c27d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c27d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c27d-129">Request body</span></span>

<span data-ttu-id="1c27d-130">No corpo da solicitação, fornece os valores para que os campos relevantes atualizem.</span><span class="sxs-lookup"><span data-stu-id="1c27d-130">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="1c27d-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1c27d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1c27d-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1c27d-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c27d-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c27d-133">Property</span></span>   | <span data-ttu-id="1c27d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c27d-134">Type</span></span> |<span data-ttu-id="1c27d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c27d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c27d-136">funções</span><span class="sxs-lookup"><span data-stu-id="1c27d-136">roles</span></span>|<span data-ttu-id="1c27d-137">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c27d-137">string collection</span></span>|<span data-ttu-id="1c27d-138">As funções desse usuário.</span><span class="sxs-lookup"><span data-stu-id="1c27d-138">The roles for that user.</span></span> <span data-ttu-id="1c27d-139">Deve ser "proprietário" ou vazio.</span><span class="sxs-lookup"><span data-stu-id="1c27d-139">Must be "owner" or empty.</span></span> <span data-ttu-id="1c27d-140">Os usuários convidados sempre devem ter a função "convidado" e não podem mudar.</span><span class="sxs-lookup"><span data-stu-id="1c27d-140">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="1c27d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c27d-141">Response</span></span>

<span data-ttu-id="1c27d-142">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c27d-142">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c27d-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c27d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c27d-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c27d-144">Request</span></span>

<span data-ttu-id="1c27d-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c27d-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c27d-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c27d-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1c27d-147">C#</span><span class="sxs-lookup"><span data-stu-id="1c27d-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c27d-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c27d-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c27d-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c27d-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c27d-150">Java</span><span class="sxs-lookup"><span data-stu-id="1c27d-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c27d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c27d-151">Response</span></span>

<span data-ttu-id="1c27d-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c27d-152">Here is an example of the response.</span></span>

><span data-ttu-id="1c27d-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c27d-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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


