---
title: Obter membro da equipe
description: Obter membro da equipe.
author: akjo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6a12455b9fb2d51c13dc725ec509542136affa1e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060322"
---
# <a name="get-member-of-team"></a><span data-ttu-id="5aaf5-103">Obter membro da equipe</span><span class="sxs-lookup"><span data-stu-id="5aaf5-103">Get member of team</span></span>

<span data-ttu-id="5aaf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aaf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aaf5-105">Obter um [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="5aaf5-105">Get a [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5aaf5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5aaf5-106">Permissions</span></span>

<span data-ttu-id="5aaf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aaf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5aaf5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5aaf5-109">Permission Type</span></span>|<span data-ttu-id="5aaf5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5aaf5-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5aaf5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5aaf5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="5aaf5-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5aaf5-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="5aaf5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5aaf5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aaf5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aaf5-114">Not supported.</span></span>    |
|<span data-ttu-id="5aaf5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5aaf5-115">Application</span></span>| <span data-ttu-id="5aaf5-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5aaf5-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="5aaf5-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="5aaf5-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="5aaf5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aaf5-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
GET /teams/{team-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5aaf5-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5aaf5-119">Optional query parameters</span></span>

<span data-ttu-id="5aaf5-120">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5aaf5-120">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5aaf5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aaf5-121">Request headers</span></span>

| <span data-ttu-id="5aaf5-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5aaf5-122">Header</span></span>       | <span data-ttu-id="5aaf5-123">Valor</span><span class="sxs-lookup"><span data-stu-id="5aaf5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5aaf5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5aaf5-124">Authorization</span></span>  | <span data-ttu-id="5aaf5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aaf5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5aaf5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5aaf5-127">Request body</span></span>

<span data-ttu-id="5aaf5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5aaf5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5aaf5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aaf5-129">Response</span></span>

<span data-ttu-id="5aaf5-130">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aaf5-130">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5aaf5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aaf5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5aaf5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aaf5-132">Request</span></span>

<span data-ttu-id="5aaf5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aaf5-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5aaf5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aaf5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-get_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members//ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="5aaf5-135">C#</span><span class="sxs-lookup"><span data-stu-id="5aaf5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-get-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aaf5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aaf5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-get-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aaf5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aaf5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-get-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5aaf5-138">Java</span><span class="sxs-lookup"><span data-stu-id="5aaf5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-get-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5aaf5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aaf5-139">Response</span></span>

<span data-ttu-id="5aaf5-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aaf5-140">Here is an example of the response.</span></span>

><span data-ttu-id="5aaf5-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5aaf5-141">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
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

## <a name="see-also"></a><span data-ttu-id="5aaf5-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="5aaf5-142">See also</span></span>

- [<span data-ttu-id="5aaf5-143">Obter membro do canal</span><span class="sxs-lookup"><span data-stu-id="5aaf5-143">Get member of channel</span></span>](channel-get-members.md)

