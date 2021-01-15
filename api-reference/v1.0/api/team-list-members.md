---
title: Listar membros de equipe
description: Obtenha o conversationMembers de uma equipe.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3d55cb5847faee74b10892afd679573998f203f3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872209"
---
# <a name="list-members-of-team"></a><span data-ttu-id="daca2-103">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="daca2-103">List members of team</span></span>
<span data-ttu-id="daca2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daca2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="daca2-105">Obtenha a [conversationMember](../resources/conversationmember.md) coleçãoda [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="daca2-105">Get the [conversationMember](../resources/conversationmember.md) collection of a [team](../resources/team.md).</span></span>

> [!NOTE]
> <span data-ttu-id="daca2-106">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="daca2-106">The membership IDs returned by server must be treated as opaque strings.</span></span> <span data-ttu-id="daca2-107">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="daca2-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
> 
> <span data-ttu-id="daca2-108">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro.</span><span class="sxs-lookup"><span data-stu-id="daca2-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="daca2-109">O cliente não deve presumir que todos os membros são apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="daca2-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="daca2-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="daca2-110">Permissions</span></span>
<span data-ttu-id="daca2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daca2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daca2-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daca2-113">Permission type</span></span>|<span data-ttu-id="daca2-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="daca2-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daca2-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daca2-115">Delegated (work or school account)</span></span>| <span data-ttu-id="daca2-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daca2-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="daca2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daca2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daca2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daca2-118">Not supported.</span></span>    |
|<span data-ttu-id="daca2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daca2-119">Application</span></span>| <span data-ttu-id="daca2-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daca2-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="daca2-121">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="daca2-121">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="daca2-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daca2-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="daca2-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="daca2-123">Optional query parameters</span></span>
<span data-ttu-id="daca2-124">Este método oferece suporte aos parâmetros de consulta `$filter` e `$select`[OData](/graph/query-parameters)para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="daca2-124">This method supports the `$filter` and `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="daca2-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daca2-125">Request headers</span></span>
|<span data-ttu-id="daca2-126">Nome</span><span class="sxs-lookup"><span data-stu-id="daca2-126">Name</span></span>|<span data-ttu-id="daca2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="daca2-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="daca2-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="daca2-128">Authorization</span></span>|<span data-ttu-id="daca2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="daca2-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="daca2-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daca2-131">Request body</span></span>
<span data-ttu-id="daca2-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="daca2-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daca2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="daca2-133">Response</span></span>

<span data-ttu-id="daca2-134">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daca2-134">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="daca2-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="daca2-135">Examples</span></span>

### <a name="example-1-get-list-of-members-in-team"></a><span data-ttu-id="daca2-136">Exemplo 1: obter uma lista de membros da equipe</span><span class="sxs-lookup"><span data-stu-id="daca2-136">Example 1: Get list of members in team</span></span>

#### <a name="request"></a><span data-ttu-id="daca2-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daca2-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="daca2-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="daca2-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
```
# <a name="c"></a>[<span data-ttu-id="daca2-139">C#</span><span class="sxs-lookup"><span data-stu-id="daca2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="daca2-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="daca2-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="daca2-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="daca2-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="daca2-142">Java</span><span class="sxs-lookup"><span data-stu-id="daca2-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="daca2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="daca2-143">Response</span></span>
><span data-ttu-id="daca2-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="daca2-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 3,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyM3NTJmNTBiNy0yNTZmLTQ1MzktYjc3NS1jNGQxMmYyZTQ3MjI=",
            "roles": [],
            "displayName": "Harry Johnson",
            "userId": "752f50b7-256f-4539-b775-c4d12f2e4722",
            "email": "harry@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

### <a name="example-2-find-members-of-a-team-by-their-azure-ad-user-object-id"></a><span data-ttu-id="daca2-145">Exemplo 2: encontrar membros de uma equipe por sua ID de objeto de usuário do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="daca2-145">Example 2: Find members of a team by their Azure AD user object ID</span></span>

<span data-ttu-id="daca2-146">O exemplo a seguir mostra uma solicitação para encontrar os recursos de afiliação com base na `id` do [usuário do Microsoft Azure Active Directory](../resources/user.md) associado ao [aadUserConversationMember](../resources/aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="daca2-146">The following example shows a request to find the membership resources based on `id` of the [Azure AD user](../resources/user.md) associated with the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="daca2-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daca2-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="daca2-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="daca2-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_userid"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')

```
# <a name="c"></a>[<span data-ttu-id="daca2-149">C#</span><span class="sxs-lookup"><span data-stu-id="daca2-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-filter-by-userid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="daca2-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="daca2-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-filter-by-userid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="daca2-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="daca2-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-filter-by-userid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="daca2-152">Java</span><span class="sxs-lookup"><span data-stu-id="daca2-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-filter-by-userid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="daca2-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="daca2-153">Response</span></span>
><span data-ttu-id="daca2-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="daca2-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team_filter_by_userid",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        }
    ]
}
```

### <a name="example-3-find-members-of-a-team-by-their-names-or-email"></a><span data-ttu-id="daca2-155">Exemplo 3: encontrar membros de uma equipe por seus nomes ou email</span><span class="sxs-lookup"><span data-stu-id="daca2-155">Example 3: Find members of a team by their names or email</span></span>

<span data-ttu-id="daca2-156">O exemplo a seguir mostra uma solicitação para localizar os recursos de afiliação com base em `displayName` ou `email` do [aadUserConversationMember](../resources/aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="daca2-156">The following example shows a request to find the membership resources based on `displayName` or `email` of the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="daca2-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daca2-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="daca2-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="daca2-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_username_or_email"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/displayName eq 'Harry Johnson' or microsoft.graph.aadUserConversationMember/email eq 'admin@M365x987948.OnMicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="daca2-159">C#</span><span class="sxs-lookup"><span data-stu-id="daca2-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-filter-by-username-or-email-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="daca2-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="daca2-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-filter-by-username-or-email-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="daca2-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="daca2-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-filter-by-username-or-email-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="daca2-162">Java</span><span class="sxs-lookup"><span data-stu-id="daca2-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-filter-by-username-or-email-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="daca2-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="daca2-163">Response</span></span>
><span data-ttu-id="daca2-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="daca2-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team_filter_by_username_or_email",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyM3NTJmNTBiNy0yNTZmLTQ1MzktYjc3NS1jNGQxMmYyZTQ3MjI=",
            "roles": [],
            "displayName": "Harry Johnson",
            "userId": "752f50b7-256f-4539-b775-c4d12f2e4722",
            "email": "harry@M365x987948.OnMicrosoft.com"
        }
    ]
}
```
## <a name="see-also"></a><span data-ttu-id="daca2-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="daca2-165">See also</span></span>

- [<span data-ttu-id="daca2-166">Listar membros no canal</span><span class="sxs-lookup"><span data-stu-id="daca2-166">List members in channel</span></span>](channel-list-members.md)
