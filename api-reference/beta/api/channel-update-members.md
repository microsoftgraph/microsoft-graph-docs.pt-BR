---
title: Atualizar membro no canal
description: Atualizar a função de membro em um canal.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6f983fd17eca37dbd5008569817787308ec25540
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522031"
---
# <a name="update-member-in-channel"></a><span data-ttu-id="5e592-103">Atualizar membro no canal</span><span class="sxs-lookup"><span data-stu-id="5e592-103">Update member in channel</span></span>

<span data-ttu-id="5e592-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e592-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e592-105">Atualizar a função de um [conversationMember](../resources/conversationmember.md) em um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="5e592-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="5e592-106">Essa operação só é permitida para canais com um valor de **membershiptype** de `private` .</span><span class="sxs-lookup"><span data-stu-id="5e592-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e592-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5e592-107">Permissions</span></span>

<span data-ttu-id="5e592-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e592-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e592-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e592-110">Permission Type</span></span>|<span data-ttu-id="5e592-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e592-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5e592-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e592-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e592-113">ChannelMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="5e592-113">ChannelMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="5e592-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e592-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e592-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e592-115">Not supported</span></span>|
|<span data-ttu-id="5e592-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e592-116">Application</span></span>|<span data-ttu-id="5e592-117">ChannelMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="5e592-117">ChannelMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e592-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e592-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="5e592-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e592-119">Request headers</span></span>

| <span data-ttu-id="5e592-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5e592-120">Header</span></span>       | <span data-ttu-id="5e592-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5e592-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e592-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e592-122">Authorization</span></span>  | <span data-ttu-id="5e592-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e592-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e592-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="5e592-125">Content-type</span></span> | <span data-ttu-id="5e592-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e592-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e592-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e592-128">Request body</span></span>

<span data-ttu-id="5e592-129">No corpo da solicitação, forneça os valores para os campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="5e592-129">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="5e592-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5e592-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5e592-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5e592-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e592-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e592-132">Property</span></span>   | <span data-ttu-id="5e592-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e592-133">Type</span></span> |<span data-ttu-id="5e592-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e592-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e592-135">funções</span><span class="sxs-lookup"><span data-stu-id="5e592-135">roles</span></span>|<span data-ttu-id="5e592-136">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5e592-136">string collection</span></span>|<span data-ttu-id="5e592-137">A função para o usuário.</span><span class="sxs-lookup"><span data-stu-id="5e592-137">The role for the user.</span></span> <span data-ttu-id="5e592-138">Deve ser `owner` ou vazio.</span><span class="sxs-lookup"><span data-stu-id="5e592-138">Must be `owner` or empty.</span></span> <span data-ttu-id="5e592-139">Os usuários convidados são automaticamente carimbados com `guest` a função e esse valor não pode ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="5e592-139">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="5e592-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e592-140">Response</span></span>

<span data-ttu-id="5e592-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [conversationMember](../resources/conversationmember.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e592-141">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e592-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e592-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e592-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e592-143">Request</span></span>

<span data-ttu-id="5e592-144">A seguir está uma solicitação para aplicar a `owner` função a um membro existente de um canal.</span><span class="sxs-lookup"><span data-stu-id="5e592-144">The following is a request to apply the `owner` role to an existing member of a channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="5e592-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e592-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="5e592-146">C#</span><span class="sxs-lookup"><span data-stu-id="5e592-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e592-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e592-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e592-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e592-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e592-149">Java</span><span class="sxs-lookup"><span data-stu-id="5e592-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5e592-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e592-150">Response</span></span>

><span data-ttu-id="5e592-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e592-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="5e592-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="5e592-152">See also</span></span>

- [<span data-ttu-id="5e592-153">Atualizar a função do membro em uma equipe</span><span class="sxs-lookup"><span data-stu-id="5e592-153">Update member's role in a team</span></span>](team-update-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "update role of channel member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
