---
title: Listar membros de equipe
description: Obtenha o conversationMembers de uma equipe.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8afc1f6cadb6f8fc7227d279c8effe8e5b92ee2f
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660118"
---
# <a name="list-members-of-team"></a><span data-ttu-id="28d07-103">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="28d07-103">List members of team</span></span>
<span data-ttu-id="28d07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28d07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28d07-105">Obtenha a [conversationMember](../resources/conversationmember.md) coleçãoda [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="28d07-105">Get the [conversationMember](../resources/conversationmember.md) collection of a [team](../resources/team.md).</span></span>

> [!NOTE]
> <span data-ttu-id="28d07-106">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="28d07-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="28d07-107">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="28d07-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="28d07-108">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro.</span><span class="sxs-lookup"><span data-stu-id="28d07-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="28d07-109">O cliente não deve presumir que todos os membros são apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="28d07-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="28d07-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="28d07-110">Permissions</span></span>
<span data-ttu-id="28d07-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d07-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d07-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28d07-113">Permission type</span></span>|<span data-ttu-id="28d07-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28d07-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28d07-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28d07-115">Delegated (work or school account)</span></span>| <span data-ttu-id="28d07-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d07-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="28d07-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28d07-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28d07-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28d07-118">Not supported.</span></span>    |
|<span data-ttu-id="28d07-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28d07-119">Application</span></span>| <span data-ttu-id="28d07-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28d07-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="28d07-121">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="28d07-121">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="28d07-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28d07-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28d07-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28d07-123">Optional query parameters</span></span>
<span data-ttu-id="28d07-124">Este método oferece suporte aos parâmetros de consulta `$filter` e `$select` [OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28d07-124">This method supports the `$filter` and `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28d07-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28d07-125">Request headers</span></span>
|<span data-ttu-id="28d07-126">Nome</span><span class="sxs-lookup"><span data-stu-id="28d07-126">Name</span></span>|<span data-ttu-id="28d07-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="28d07-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="28d07-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="28d07-128">Authorization</span></span>|<span data-ttu-id="28d07-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28d07-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28d07-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28d07-131">Request body</span></span>
<span data-ttu-id="28d07-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28d07-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28d07-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d07-133">Response</span></span>

<span data-ttu-id="28d07-134">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28d07-134">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28d07-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28d07-135">Examples</span></span>

### <a name="example-1-get-list-of-members-in-team"></a><span data-ttu-id="28d07-136">Exemplo 1: obter uma lista de membros da equipe</span><span class="sxs-lookup"><span data-stu-id="28d07-136">Example 1: Get list of members in team</span></span>

#### <a name="request"></a><span data-ttu-id="28d07-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28d07-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members_in_team"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
```

#### <a name="response"></a><span data-ttu-id="28d07-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d07-138">Response</span></span>
><span data-ttu-id="28d07-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28d07-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-find-members-of-a-team-by-their-azure-ad-user-object-id"></a><span data-ttu-id="28d07-140">Exemplo 2: encontrar membros de uma equipe por sua ID de objeto de usuário do Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="28d07-140">Example 2: Find members of a team by their Azure AD user object ID</span></span>

<span data-ttu-id="28d07-141">O exemplo a seguir mostra uma solicitação para encontrar os recursos de afiliação com base na `id` do [usuário do Microsoft Azure Active Directory](../resources/user.md) associado ao [aadUserConversationMember](../resources/aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="28d07-141">The following example shows a request to find the membership resources based on `id` of the [Azure AD user](../resources/user.md) associated with the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="28d07-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28d07-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_userid"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/userId eq '73761f06-2ac9-469c-9f10-279a8cc267f9')

```

#### <a name="response"></a><span data-ttu-id="28d07-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d07-143">Response</span></span>
><span data-ttu-id="28d07-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28d07-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3-find-members-of-a-team-by-their-names-or-email"></a><span data-ttu-id="28d07-145">Exemplo 3: encontrar membros de uma equipe por seus nomes ou email</span><span class="sxs-lookup"><span data-stu-id="28d07-145">Example 3: Find members of a team by their names or email</span></span>

<span data-ttu-id="28d07-146">O exemplo a seguir mostra uma solicitação para localizar os recursos de afiliação com base em `displayName` ou `email` do [aadUserConversationMember](../resources/aaduserconversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="28d07-146">The following example shows a request to find the membership resources based on `displayName` or `email` of the [aadUserConversationMember](../resources/aaduserconversationmember.md).</span></span>

#### <a name="request"></a><span data-ttu-id="28d07-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28d07-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_username_or_email"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=(microsoft.graph.aadUserConversationMember/displayName eq 'Harry Johnson' or microsoft.graph.aadUserConversationMember/email eq 'admin@M365x987948.OnMicrosoft.com')
```

#### <a name="response"></a><span data-ttu-id="28d07-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d07-148">Response</span></span>
><span data-ttu-id="28d07-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28d07-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-4-list-only-those-members-who-are-owners-of-the-team"></a><span data-ttu-id="28d07-150">Exemplo 4: Listar apenas os membros que são *proprietários* da equipe</span><span class="sxs-lookup"><span data-stu-id="28d07-150">Example 4: List only those members who are *owners* of the team</span></span>

<span data-ttu-id="28d07-151">O exemplo a seguir mostra uma solicitação para localizar todos os membros que possuem a função de *proprietário* anexada a eles.</span><span class="sxs-lookup"><span data-stu-id="28d07-151">The following example shows a request to find all the members who are have *owner* role attached to them.</span></span>

> [!NOTE]
> <span data-ttu-id="28d07-152">Há alguns problemas conhecidos com essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="28d07-152">There are some known issues with this functionality.</span></span> <span data-ttu-id="28d07-153">Para saber mais, confira [problemas conhecidos](/graph/known-issues.md#unable-to-filter-team-members-by-roles).</span><span class="sxs-lookup"><span data-stu-id="28d07-153">For details, see [known issues](/graph/known-issues.md#unable-to-filter-team-members-by-roles).</span></span>

#### <a name="request"></a><span data-ttu-id="28d07-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28d07-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members_in_team_filter_by_owner_role"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members?$filter=roles/any(r:r eq 'owner')
```

#### <a name="response"></a><span data-ttu-id="28d07-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="28d07-155">Response</span></span>
><span data-ttu-id="28d07-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="28d07-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="28d07-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="28d07-157">See also</span></span>

- [<span data-ttu-id="28d07-158">Listar membros no canal</span><span class="sxs-lookup"><span data-stu-id="28d07-158">List members in channel</span></span>](channel-list-members.md)
