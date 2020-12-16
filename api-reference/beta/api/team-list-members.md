---
title: Listar membros de equipe
description: Obtenha o conversationMembers de uma equipe.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f2ef0fb65fea23451da13b355ac1aa194554f5a
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690815"
---
# <a name="list-members-of-team"></a><span data-ttu-id="51496-103">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="51496-103">List members of team</span></span>
<span data-ttu-id="51496-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51496-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51496-105">Obtenha a [conversationMember](../resources/conversationmember.md) coleçãoda [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="51496-105">Get the [conversationMember](../resources/conversationmember.md) collection of a [team](../resources/team.md).</span></span>

> [!NOTE]
> <span data-ttu-id="51496-106">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="51496-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="51496-107">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="51496-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="51496-108">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro.</span><span class="sxs-lookup"><span data-stu-id="51496-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="51496-109">O cliente não deve presumir que todos os membros são apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="51496-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="51496-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="51496-110">Permissions</span></span>
<span data-ttu-id="51496-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51496-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51496-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51496-113">Permission type</span></span>|<span data-ttu-id="51496-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51496-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51496-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51496-115">Delegated (work or school account)</span></span>| <span data-ttu-id="51496-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51496-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="51496-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51496-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51496-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51496-118">Not supported.</span></span>    |
|<span data-ttu-id="51496-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51496-119">Application</span></span>| <span data-ttu-id="51496-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51496-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="51496-121">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="51496-121">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="51496-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51496-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51496-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="51496-123">Optional query parameters</span></span>
<span data-ttu-id="51496-124">Este método oferece suporte aos parâmetros de consulta `$filter` e `$select`[OData](/graph/query-parameters)para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="51496-124">This method supports the `$filter` and `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51496-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51496-125">Request headers</span></span>
|<span data-ttu-id="51496-126">Nome</span><span class="sxs-lookup"><span data-stu-id="51496-126">Name</span></span>|<span data-ttu-id="51496-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="51496-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="51496-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="51496-128">Authorization</span></span>|<span data-ttu-id="51496-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51496-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51496-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51496-131">Request body</span></span>
<span data-ttu-id="51496-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51496-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51496-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="51496-133">Response</span></span>

<span data-ttu-id="51496-134">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51496-134">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51496-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="51496-135">Examples</span></span>

### <a name="example-1-get-list-of-members-in-team"></a><span data-ttu-id="51496-136">Exemplo 1: obter uma lista de membros da equipe</span><span class="sxs-lookup"><span data-stu-id="51496-136">Example 1: Get list of members in team</span></span>

#### <a name="request"></a><span data-ttu-id="51496-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51496-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51496-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="51496-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
```
# <a name="c"></a>[<span data-ttu-id="51496-139">C#</span><span class="sxs-lookup"><span data-stu-id="51496-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51496-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51496-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51496-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51496-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51496-142">Java</span><span class="sxs-lookup"><span data-stu-id="51496-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51496-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="51496-143">Response</span></span>
><span data-ttu-id="51496-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="51496-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
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

### <a name="example-2-find-members-of-a-team-by-their-azure-ad-user-object-id"></a><span data-ttu-id="51496-145">Exemplo 2: encontrar membros de uma equipe por sua ID de objeto de usuário do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="51496-145">Example 2: Find members of a team by their Azure AD user object ID</span></span>

<span data-ttu-id="51496-146">O exemplo a seguir mostra uma solicitação para encontrar os recursos de afiliação com base na `id` do [usuário do Microsoft Azure Active Directory](../resources/user.md) associado ao [aadUserConversationMember](../resources/aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="51496-146">The following example shows a request to find the membership resources based on `id` of the [Azure AD user](../resources/user.md) associated with the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="51496-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51496-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51496-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="51496-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_userid"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')

```
# <a name="c"></a>[<span data-ttu-id="51496-149">C#</span><span class="sxs-lookup"><span data-stu-id="51496-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-filter-by-userid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51496-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51496-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-filter-by-userid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51496-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51496-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-filter-by-userid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51496-152">Java</span><span class="sxs-lookup"><span data-stu-id="51496-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-filter-by-userid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51496-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="51496-153">Response</span></span>
><span data-ttu-id="51496-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="51496-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
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

### <a name="example-3-find-members-of-a-team-by-their-names-or-email"></a><span data-ttu-id="51496-155">Exemplo 3: encontrar membros de uma equipe por seus nomes ou email</span><span class="sxs-lookup"><span data-stu-id="51496-155">Example 3: Find members of a team by their names or email</span></span>

<span data-ttu-id="51496-156">O exemplo a seguir mostra uma solicitação para localizar os recursos de afiliação com base em `displayName` ou `email` do [aadUserConversationMember](../resources/aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="51496-156">The following example shows a request to find the membership resources based on `displayName` or `email` of the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="51496-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51496-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51496-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="51496-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_username_or_email"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/displayName eq 'Harry Johnson' or microsoft.graph.aadUserConversationMember/email eq 'admin@M365x987948.OnMicrosoft.com')
```
# <a name="c"></a>[<span data-ttu-id="51496-159">C#</span><span class="sxs-lookup"><span data-stu-id="51496-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-filter-by-username-or-email-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51496-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51496-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-filter-by-username-or-email-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51496-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51496-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-filter-by-username-or-email-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51496-162">Java</span><span class="sxs-lookup"><span data-stu-id="51496-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-filter-by-username-or-email-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51496-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="51496-163">Response</span></span>
><span data-ttu-id="51496-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="51496-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
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

### <a name="example-4-list-only-those-members-who-are-owners-of-the-team"></a><span data-ttu-id="51496-165">Exemplo 4: Listar apenas os membros que são *proprietários* da equipe</span><span class="sxs-lookup"><span data-stu-id="51496-165">Example 4: List only those members who are *owners* of the team</span></span>

<span data-ttu-id="51496-166">O exemplo a seguir mostra uma solicitação para localizar todos os membros que possuem a função de *proprietário* anexada a eles.</span><span class="sxs-lookup"><span data-stu-id="51496-166">The following example shows a request to find all the members who are have *owner* role attached to them.</span></span>

> [!NOTE]
> <span data-ttu-id="51496-167">Há alguns problemas conhecidos com essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="51496-167">There are some known issues with this functionality.</span></span> <span data-ttu-id="51496-168">Para saber mais, confira [problemas conhecidos](/graph/known-issues.md#unable-to-filter-team-members-by-roles).</span><span class="sxs-lookup"><span data-stu-id="51496-168">For details, see [known issues](/graph/known-issues.md#unable-to-filter-team-members-by-roles).</span></span>

#### <a name="request"></a><span data-ttu-id="51496-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51496-169">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51496-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="51496-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_owner_role"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=roles/any(r:r eq 'owner')
```
# <a name="c"></a>[<span data-ttu-id="51496-171">C#</span><span class="sxs-lookup"><span data-stu-id="51496-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-members-in-team-filter-by-owner-role-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51496-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51496-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-members-in-team-filter-by-owner-role-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51496-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51496-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-members-in-team-filter-by-owner-role-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51496-174">Java</span><span class="sxs-lookup"><span data-stu-id="51496-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-members-in-team-filter-by-owner-role-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51496-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="51496-175">Response</span></span>
><span data-ttu-id="51496-176">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="51496-176">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_members_in_team_filter_by_owner_role",
  "@odata.type": "collection(microsoft.graph.conversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 1,
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
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="51496-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="51496-177">See also</span></span>

- [<span data-ttu-id="51496-178">Listar membros no canal</span><span class="sxs-lookup"><span data-stu-id="51496-178">List members in channel</span></span>](channel-list-members.md)
