---
title: Obter membro da equipe
description: Obter membro da equipe.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5ee28e588be74979259f1cf7dfa63cc5635d441f
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060512"
---
# <a name="get-member-of-team"></a><span data-ttu-id="1f2df-103">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="1f2df-103">Get member of team</span></span>

<span data-ttu-id="1f2df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f2df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f2df-105">Obter um [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1f2df-105">Get a [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f2df-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1f2df-106">Permissions</span></span>

<span data-ttu-id="1f2df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f2df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f2df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f2df-109">Permission Type</span></span>|<span data-ttu-id="1f2df-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f2df-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="1f2df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f2df-111">Delegated (work or school account)</span></span>| <span data-ttu-id="1f2df-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2df-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="1f2df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f2df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f2df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f2df-114">Not supported.</span></span>    |
|<span data-ttu-id="1f2df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f2df-115">Application</span></span>| <span data-ttu-id="1f2df-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2df-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="1f2df-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1f2df-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="1f2df-118">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f2df-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="1f2df-119">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="1f2df-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="1f2df-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f2df-120">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
GET /teams/{team-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f2df-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f2df-121">Optional query parameters</span></span>

<span data-ttu-id="1f2df-122">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f2df-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f2df-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f2df-123">Request headers</span></span>

| <span data-ttu-id="1f2df-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f2df-124">Header</span></span>       | <span data-ttu-id="1f2df-125">Valor</span><span class="sxs-lookup"><span data-stu-id="1f2df-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1f2df-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f2df-126">Authorization</span></span>  | <span data-ttu-id="1f2df-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f2df-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1f2df-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f2df-129">Request body</span></span>

<span data-ttu-id="1f2df-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f2df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f2df-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f2df-131">Response</span></span>

<span data-ttu-id="1f2df-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f2df-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f2df-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f2df-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f2df-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f2df-134">Request</span></span>

<span data-ttu-id="1f2df-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f2df-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1f2df-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f2df-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-get_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="1f2df-137">C#</span><span class="sxs-lookup"><span data-stu-id="1f2df-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-get-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f2df-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f2df-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-get-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f2df-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f2df-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-get-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f2df-140">Java</span><span class="sxs-lookup"><span data-stu-id="1f2df-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-get-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f2df-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f2df-141">Response</span></span>

<span data-ttu-id="1f2df-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f2df-142">Here is an example of the response.</span></span>

><span data-ttu-id="1f2df-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f2df-143">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
   "@odata.type":"#microsoft.graph.aadUserConversationMember",
   "id":"/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
   "roles":[
      "owner"
   ],
   "displayName":"John Doe",
   "userId":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
   "email":null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "get_team_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="1f2df-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="1f2df-144">See also</span></span>

- [<span data-ttu-id="1f2df-145">Obter membro do canal</span><span class="sxs-lookup"><span data-stu-id="1f2df-145">Get member of channel</span></span>](channel-get-members.md)

