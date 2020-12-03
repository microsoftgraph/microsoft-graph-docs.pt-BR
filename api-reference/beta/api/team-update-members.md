---
title: Atualizar membro no Team
description: Atualizar a função de membro em uma equipe.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7bafea4c6082f77e247d290b35d778f34cdd18a6
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523862"
---
# <a name="update-member-in-team"></a><span data-ttu-id="fd4ee-103">Atualizar membro no Team</span><span class="sxs-lookup"><span data-stu-id="fd4ee-103">Update member in team</span></span>

<span data-ttu-id="fd4ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd4ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd4ee-105">Atualizar a função de um [conversationMember](../resources/conversationmember.md) em uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="fd4ee-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd4ee-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fd4ee-106">Permissions</span></span>

<span data-ttu-id="fd4ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd4ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd4ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd4ee-109">Permission Type</span></span>|<span data-ttu-id="fd4ee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd4ee-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="fd4ee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd4ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd4ee-112">TeamMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-112">TeamMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="fd4ee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd4ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd4ee-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fd4ee-114">Not supported</span></span>|
|<span data-ttu-id="fd4ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd4ee-115">Application</span></span>|<span data-ttu-id="fd4ee-116">TeamMember. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-116">TeamMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd4ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd4ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="fd4ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd4ee-118">Request headers</span></span>

| <span data-ttu-id="fd4ee-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd4ee-119">Header</span></span>       | <span data-ttu-id="fd4ee-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fd4ee-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd4ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd4ee-121">Authorization</span></span>  | <span data-ttu-id="fd4ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd4ee-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="fd4ee-124">Content-type</span></span> | <span data-ttu-id="fd4ee-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd4ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd4ee-127">Request body</span></span>

<span data-ttu-id="fd4ee-128">No corpo da solicitação, forneça os valores para os campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-128">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="fd4ee-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fd4ee-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fd4ee-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd4ee-131">Property</span></span>   | <span data-ttu-id="fd4ee-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd4ee-132">Type</span></span> |<span data-ttu-id="fd4ee-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd4ee-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd4ee-134">funções</span><span class="sxs-lookup"><span data-stu-id="fd4ee-134">roles</span></span>|<span data-ttu-id="fd4ee-135">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd4ee-135">string collection</span></span>|<span data-ttu-id="fd4ee-136">A função para o usuário.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-136">The role for the user.</span></span> <span data-ttu-id="fd4ee-137">Deve ser `owner` ou vazio.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-137">Must be `owner` or empty.</span></span> <span data-ttu-id="fd4ee-138">Os usuários convidados são automaticamente carimbados com `guest` a função e esse valor não pode ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-138">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="fd4ee-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd4ee-139">Response</span></span>

<span data-ttu-id="fd4ee-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [conversationMember](../resources/conversationmember.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-140">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd4ee-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd4ee-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd4ee-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd4ee-142">Request</span></span>

<span data-ttu-id="fd4ee-143">A seguir está uma solicitação para aplicar a `owner` função a um membro existente de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-143">The following is a request to apply the `owner` role to an existing member of a team.</span></span>


# <a name="http"></a>[<span data-ttu-id="fd4ee-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd4ee-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_member"
} -->
```http
PATCH https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="fd4ee-145">C#</span><span class="sxs-lookup"><span data-stu-id="fd4ee-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd4ee-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd4ee-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd4ee-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd4ee-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd4ee-148">Java</span><span class="sxs-lookup"><span data-stu-id="fd4ee-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fd4ee-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd4ee-149">Response</span></span>

><span data-ttu-id="fd4ee-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fd4ee-150">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="fd4ee-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="fd4ee-151">See also</span></span>

- [<span data-ttu-id="fd4ee-152">Atualizar membro no canal</span><span class="sxs-lookup"><span data-stu-id="fd4ee-152">Update member in channel</span></span>](channel-update-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "update role of team member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
