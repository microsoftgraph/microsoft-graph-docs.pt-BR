---
title: Atualizar membro no canal
description: Atualize a função de membro em um canal.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 35bc88f95fa279c5a49d81de9a66005a0e3cc66f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948217"
---
# <a name="update-member-in-channel"></a><span data-ttu-id="9de65-103">Atualizar membro no canal</span><span class="sxs-lookup"><span data-stu-id="9de65-103">Update member in channel</span></span>

<span data-ttu-id="9de65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9de65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9de65-105">Atualize a função de [um conversationMember](../resources/conversationmember.md) em um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9de65-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="9de65-106">Essa operação só é permitida para canais com **um valor membershipType** de `private` .</span><span class="sxs-lookup"><span data-stu-id="9de65-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>

## <a name="permissions"></a><span data-ttu-id="9de65-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9de65-107">Permissions</span></span>

<span data-ttu-id="9de65-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9de65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9de65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9de65-110">Permission Type</span></span>|<span data-ttu-id="9de65-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9de65-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9de65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9de65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9de65-113">ChannelMember.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="9de65-113">ChannelMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="9de65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9de65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9de65-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9de65-115">Not supported</span></span>|
|<span data-ttu-id="9de65-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9de65-116">Application</span></span>|<span data-ttu-id="9de65-117">ChannelMember.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="9de65-117">ChannelMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9de65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9de65-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="9de65-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9de65-119">Request headers</span></span>

| <span data-ttu-id="9de65-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9de65-120">Header</span></span>       | <span data-ttu-id="9de65-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9de65-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9de65-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9de65-122">Authorization</span></span>  | <span data-ttu-id="9de65-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9de65-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9de65-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="9de65-125">Content-type</span></span> | <span data-ttu-id="9de65-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9de65-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9de65-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9de65-128">Request body</span></span>

<span data-ttu-id="9de65-129">No corpo da solicitação, fornece os valores para que os campos relevantes atualizem.</span><span class="sxs-lookup"><span data-stu-id="9de65-129">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="9de65-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="9de65-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9de65-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9de65-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9de65-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9de65-132">Property</span></span>   | <span data-ttu-id="9de65-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9de65-133">Type</span></span> |<span data-ttu-id="9de65-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9de65-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9de65-135">funções</span><span class="sxs-lookup"><span data-stu-id="9de65-135">roles</span></span>|<span data-ttu-id="9de65-136">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9de65-136">string collection</span></span>|<span data-ttu-id="9de65-137">A função do usuário.</span><span class="sxs-lookup"><span data-stu-id="9de65-137">The role for the user.</span></span> <span data-ttu-id="9de65-138">Deve estar `owner` ou vazio.</span><span class="sxs-lookup"><span data-stu-id="9de65-138">Must be `owner` or empty.</span></span> <span data-ttu-id="9de65-139">Os usuários convidados são automaticamente carimbados `guest` com a função e esse valor não pode ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="9de65-139">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="9de65-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9de65-140">Response</span></span>

<span data-ttu-id="9de65-141">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto conversationMember](../resources/conversationmember.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9de65-141">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9de65-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9de65-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="9de65-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9de65-143">Request</span></span>

<span data-ttu-id="9de65-144">A seguir está uma solicitação para aplicar `owner` a função a um membro existente de um canal.</span><span class="sxs-lookup"><span data-stu-id="9de65-144">The following is a request to apply the `owner` role to an existing member of a channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="9de65-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9de65-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_member_1"
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
# <a name="c"></a>[<span data-ttu-id="9de65-146">C#</span><span class="sxs-lookup"><span data-stu-id="9de65-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-member-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9de65-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9de65-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-member-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9de65-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9de65-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-member-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9de65-149">Java</span><span class="sxs-lookup"><span data-stu-id="9de65-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-member-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9de65-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9de65-150">Response</span></span>

><span data-ttu-id="9de65-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9de65-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

## <a name="see-also"></a><span data-ttu-id="9de65-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="9de65-152">See also</span></span>

- [<span data-ttu-id="9de65-153">Atualizar a função do membro em uma equipe</span><span class="sxs-lookup"><span data-stu-id="9de65-153">Update member's role in a team</span></span>](team-update-members.md)

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
