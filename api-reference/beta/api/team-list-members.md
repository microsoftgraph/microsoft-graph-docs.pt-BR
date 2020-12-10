---
title: Listar membros de equipe
description: Obtenha o conversationMembers de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4685e277f386d6ecaa51565778529ac812ba1c65
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387588"
---
# <a name="list-members-of-team"></a><span data-ttu-id="3d4c8-103">Listar membros de equipe</span><span class="sxs-lookup"><span data-stu-id="3d4c8-103">List members of team</span></span>
<span data-ttu-id="3d4c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d4c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d4c8-105">Obtenha a [conversationMember](../resources/conversationmember.md) coleçãoda [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="3d4c8-105">Get the [conversationMember](../resources/conversationmember.md) collection of a [team](../resources/team.md).</span></span>

> [!NOTE]
> <span data-ttu-id="3d4c8-106">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="3d4c8-107">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="3d4c8-108">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-108">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="3d4c8-109">O cliente não deve presumir que todos os membros são apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-109">The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d4c8-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="3d4c8-110">Permissions</span></span>
<span data-ttu-id="3d4c8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d4c8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d4c8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d4c8-113">Permission type</span></span>|<span data-ttu-id="3d4c8-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d4c8-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d4c8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d4c8-115">Delegated (work or school account)</span></span>| <span data-ttu-id="3d4c8-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4c8-116">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="3d4c8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d4c8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d4c8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-118">Not supported.</span></span>    |
|<span data-ttu-id="3d4c8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d4c8-119">Application</span></span>| <span data-ttu-id="3d4c8-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4c8-120">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="3d4c8-121">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="3d4c8-121">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="3d4c8-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d4c8-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{team-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d4c8-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3d4c8-123">Optional query parameters</span></span>
<span data-ttu-id="3d4c8-124">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-124">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3d4c8-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3d4c8-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d4c8-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d4c8-126">Request headers</span></span>
|<span data-ttu-id="3d4c8-127">Nome</span><span class="sxs-lookup"><span data-stu-id="3d4c8-127">Name</span></span>|<span data-ttu-id="3d4c8-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d4c8-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3d4c8-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d4c8-129">Authorization</span></span>|<span data-ttu-id="3d4c8-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d4c8-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d4c8-132">Request body</span></span>
<span data-ttu-id="3d4c8-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d4c8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d4c8-134">Response</span></span>

<span data-ttu-id="3d4c8-135">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-135">If successful, this method returns a `200 OK` response code and a collection of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d4c8-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3d4c8-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d4c8-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d4c8-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3d4c8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d4c8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members
```
# <a name="c"></a>[<span data-ttu-id="3d4c8-139">C#</span><span class="sxs-lookup"><span data-stu-id="3d4c8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d4c8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d4c8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d4c8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d4c8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d4c8-142">Java</span><span class="sxs-lookup"><span data-stu-id="3d4c8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3d4c8-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d4c8-143">Response</span></span>
<span data-ttu-id="3d4c8-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3d4c8-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_conversationmember",
  "@odata.type": "collection(microsoft.graph.aadUserConversationMember)"
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
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="3d4c8-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="3d4c8-145">See also</span></span>

- [<span data-ttu-id="3d4c8-146">Listar membros no canal</span><span class="sxs-lookup"><span data-stu-id="3d4c8-146">List members in channel</span></span>](channel-list-members.md)
