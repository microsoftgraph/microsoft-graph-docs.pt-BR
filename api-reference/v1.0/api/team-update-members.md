---
title: Atualizar membro na equipe
description: Atualize a função de membro em uma equipe.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0970bc564d23cfaadd7238f25c3afd0a487540f6
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060426"
---
# <a name="update-member-in-team"></a><span data-ttu-id="77457-103">Atualizar membro na equipe</span><span class="sxs-lookup"><span data-stu-id="77457-103">Update member in team</span></span>

<span data-ttu-id="77457-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77457-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77457-105">Atualize a função de [um conversationMember](../resources/conversationmember.md) em uma [equipe.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="77457-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="77457-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="77457-106">Permissions</span></span>

<span data-ttu-id="77457-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77457-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77457-109">Permission Type</span></span>|<span data-ttu-id="77457-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77457-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="77457-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77457-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77457-112">TeamMember.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="77457-112">TeamMember.ReadWrite.All.</span></span> |
|<span data-ttu-id="77457-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77457-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77457-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="77457-114">Not supported</span></span>|
|<span data-ttu-id="77457-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77457-115">Application</span></span>|<span data-ttu-id="77457-116">TeamMember.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="77457-116">TeamMember.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77457-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77457-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="77457-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77457-118">Request headers</span></span>

| <span data-ttu-id="77457-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77457-119">Header</span></span>       | <span data-ttu-id="77457-120">Valor</span><span class="sxs-lookup"><span data-stu-id="77457-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="77457-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="77457-121">Authorization</span></span>  | <span data-ttu-id="77457-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77457-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="77457-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="77457-124">Content-type</span></span> | <span data-ttu-id="77457-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77457-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77457-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77457-127">Request body</span></span>

<span data-ttu-id="77457-128">No corpo da solicitação, fornece os valores para que os campos relevantes atualizem.</span><span class="sxs-lookup"><span data-stu-id="77457-128">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="77457-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="77457-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="77457-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="77457-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="77457-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77457-131">Property</span></span>   | <span data-ttu-id="77457-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="77457-132">Type</span></span> |<span data-ttu-id="77457-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="77457-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77457-134">funções</span><span class="sxs-lookup"><span data-stu-id="77457-134">roles</span></span>|<span data-ttu-id="77457-135">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="77457-135">string collection</span></span>|<span data-ttu-id="77457-136">A função do usuário.</span><span class="sxs-lookup"><span data-stu-id="77457-136">The role for the user.</span></span> <span data-ttu-id="77457-137">Deve estar `owner` ou vazio.</span><span class="sxs-lookup"><span data-stu-id="77457-137">Must be `owner` or empty.</span></span> <span data-ttu-id="77457-138">Os usuários convidados são automaticamente carimbados `guest` com a função e esse valor não pode ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="77457-138">Guest users are automatically stamped with `guest` role and this value cannot be updated.</span></span> |

## <a name="response"></a><span data-ttu-id="77457-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77457-139">Response</span></span>

<span data-ttu-id="77457-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto conversationMember](../resources/conversationmember.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77457-140">If successful, this method returns a `200 OK` response code and an updated [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77457-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77457-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="77457-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77457-142">Request</span></span>

<span data-ttu-id="77457-143">A seguir está uma solicitação para aplicar `owner` a função a um membro existente de uma equipe.</span><span class="sxs-lookup"><span data-stu-id="77457-143">The following is a request to apply the `owner` role to an existing member of a team.</span></span>


# <a name="http"></a>[<span data-ttu-id="77457-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="77457-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_member_2"
} -->
```http
PATCH https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```
# <a name="c"></a>[<span data-ttu-id="77457-145">C#</span><span class="sxs-lookup"><span data-stu-id="77457-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-member-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77457-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77457-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-member-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77457-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77457-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-member-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77457-148">Java</span><span class="sxs-lookup"><span data-stu-id="77457-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-member-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77457-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="77457-149">Response</span></span>

><span data-ttu-id="77457-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="77457-150">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

## <a name="see-also"></a><span data-ttu-id="77457-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="77457-151">See also</span></span>

- [<span data-ttu-id="77457-152">Atualizar membro no canal</span><span class="sxs-lookup"><span data-stu-id="77457-152">Update member in channel</span></span>](channel-update-members.md)

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
