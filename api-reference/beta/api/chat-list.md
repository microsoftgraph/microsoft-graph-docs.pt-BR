---
title: Listar chats
description: Recupere a lista de chats de um usuário.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0416a123b0694b3b2ffcd6756334fcf891da0b82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775763"
---
# <a name="list-chats"></a><span data-ttu-id="8b1ce-103">Listar chats</span><span class="sxs-lookup"><span data-stu-id="8b1ce-103">List chats</span></span>

<span data-ttu-id="8b1ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b1ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b1ce-105">Recupere a lista [de chats](../resources/chat.md) dos que o usuário faz parte.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-105">Retrieve the list of [chats](../resources/chat.md) that the user is part of.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b1ce-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b1ce-106">Permissions</span></span>

<span data-ttu-id="8b1ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b1ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b1ce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b1ce-109">Permission type</span></span>      | <span data-ttu-id="8b1ce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b1ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b1ce-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b1ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8b1ce-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b1ce-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="8b1ce-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b1ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b1ce-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-114">Not supported.</span></span>    |
|<span data-ttu-id="8b1ce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b1ce-115">Application</span></span> | <span data-ttu-id="8b1ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b1ce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{user-id}/chats
GET /chats
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b1ce-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8b1ce-118">Optional query parameters</span></span>

<span data-ttu-id="8b1ce-119">Este método dá suporte aos parâmetros de consulta (somente para a propriedade `$expand` **members)** e `$filter` [OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-119">This method supports the `$expand` (only for the **members** property) and `$filter` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b1ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1ce-120">Request headers</span></span>

| <span data-ttu-id="8b1ce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b1ce-121">Header</span></span>       | <span data-ttu-id="8b1ce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8b1ce-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b1ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b1ce-123">Authorization</span></span>  | <span data-ttu-id="8b1ce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b1ce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1ce-126">Request body</span></span>

<span data-ttu-id="8b1ce-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b1ce-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b1ce-128">Response</span></span>

<span data-ttu-id="8b1ce-129">Se bem sucedido, esse método retorna um código de resposta `200 OK` e uma coleção de objetos de [bate-papo](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-129">If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b1ce-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b1ce-130">Example</span></span>

### <a name="example-1-list-all-the-chats"></a><span data-ttu-id="8b1ce-131">Exemplo 1: Listar todos os chats</span><span class="sxs-lookup"><span data-stu-id="8b1ce-131">Example 1: List all the chats</span></span>

#### <a name="request"></a><span data-ttu-id="8b1ce-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1ce-132">Request</span></span>

<span data-ttu-id="8b1ce-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b1ce-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1ce-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats
```
# <a name="c"></a>[<span data-ttu-id="8b1ce-135">C#</span><span class="sxs-lookup"><span data-stu-id="8b1ce-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-chats-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b1ce-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b1ce-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-chats-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b1ce-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b1ce-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-chats-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b1ce-138">Java</span><span class="sxs-lookup"><span data-stu-id="8b1ce-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-chats-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="8b1ce-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b1ce-139">Response</span></span>

<span data-ttu-id="8b1ce-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-140">Here is an example of the response.</span></span> 

><span data-ttu-id="8b1ce-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats",
    "@odata.count": 3,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting"
        },
        {
            "id": "19:561082c0f3f847a58069deb8eb300807@thread.v2",
            "topic": "Group chat sample",
            "createdDateTime": "2020-12-03T19:41:07.054Z",
            "lastUpdatedDateTime": "2020-12-08T23:53:11.012Z",
            "chatType": "group"
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne"
        }
    ]
}
```

### <a name="example-2-list-all-the-chats-along-with-the-members-of-each-chat"></a><span data-ttu-id="8b1ce-142">Exemplo 2: listar todos os chats juntamente com os membros de cada chat</span><span class="sxs-lookup"><span data-stu-id="8b1ce-142">Example 2: List all the chats along with the members of each chat</span></span>
#### <a name="request"></a><span data-ttu-id="8b1ce-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1ce-143">Request</span></span>

<span data-ttu-id="8b1ce-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b1ce-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1ce-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats_expand_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats?$expand=members
```
# <a name="c"></a>[<span data-ttu-id="8b1ce-146">C#</span><span class="sxs-lookup"><span data-stu-id="8b1ce-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-chats-expand-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b1ce-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b1ce-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-chats-expand-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b1ce-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b1ce-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-chats-expand-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b1ce-149">Java</span><span class="sxs-lookup"><span data-stu-id="8b1ce-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-chats-expand-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="8b1ce-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b1ce-150">Response</span></span>

<span data-ttu-id="8b1ce-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-151">Here is an example of the response.</span></span> 

> [!NOTE]
> <span data-ttu-id="8b1ce-152">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-152">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="8b1ce-153">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-153">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="8b1ce-154">Os resultados da associação podem mapear para usuários de locatários diferentes, conforme indicado na resposta, no futuro.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-154">The membership results can map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="8b1ce-155">O cliente não deve presumir que todos os membros são apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-155">The client should not assume that all members are from the current tenant only.</span></span>

><span data-ttu-id="8b1ce-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats(members())",
    "@odata.count": 3,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ameeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:561082c0f3f847a58069deb8eb300807@thread.v2",
            "topic": "Group chat sample",
            "createdDateTime": "2020-12-03T19:41:07.054Z",
            "lastUpdatedDateTime": "2020-12-08T23:53:11.012Z",
            "chatType": "group",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A561082c0f3f847a58069deb8eb300807%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM312ftMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Bruce Banner",
                    "userId": "48bf9d52-dca7-4a5f-8398-37b95cc7bd83",
                    "email": "bannerb@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWai3MTetN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "TChalla",
                    "userId": "9efb1aea-4f83-4673-bdcd-d3f3c7be28c2",
                    "email": "tchalla@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwamii00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Thor Odinson",
                    "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
                    "email": "odinsont@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWopiLWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Steve Rogers",
                    "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
                    "email": "rogerss@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca%40unq.gbl.spaces')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

### <a name="example-3-list-all-the-chats-that-have-a-member-with-a-specific-display-name"></a><span data-ttu-id="8b1ce-157">Exemplo 3: listar todos os chats que têm um membro com um nome de exibição específico</span><span class="sxs-lookup"><span data-stu-id="8b1ce-157">Example 3: List all the chats that have a member with a specific display name</span></span>

#### <a name="request"></a><span data-ttu-id="8b1ce-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1ce-158">Request</span></span>

<span data-ttu-id="8b1ce-159">Aqui está um exemplo de uma solicitação que filtrará todos os chats com base no nome de exibição de um membro específico.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-159">Here is an example of a request that will filter all the chats based on a specific member's display name.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b1ce-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1ce-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_chats_expand_members_and_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats?$expand=members&$filter=members/any(o: o/displayname eq 'Peter Parker')
```
# <a name="c"></a>[<span data-ttu-id="8b1ce-161">C#</span><span class="sxs-lookup"><span data-stu-id="8b1ce-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-chats-expand-members-and-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b1ce-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b1ce-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-chats-expand-members-and-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b1ce-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b1ce-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-chats-expand-members-and-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b1ce-164">Java</span><span class="sxs-lookup"><span data-stu-id="8b1ce-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-chats-expand-members-and-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="8b1ce-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b1ce-165">Response</span></span>

<span data-ttu-id="8b1ce-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-166">Here is an example of the response.</span></span> 

> [!NOTE]
> <span data-ttu-id="8b1ce-167">A ID de afiliação retornada pelo servidor deve ser tratada como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-167">The membership ID returned by server must be treated as opaque strings.</span></span> <span data-ttu-id="8b1ce-168">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-168">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="8b1ce-169">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-169">The membership results could map to users from different tenants, as indicated in the response, in the future.</span></span> <span data-ttu-id="8b1ce-170">O cliente não deve presumir que todos os membros são apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-170">The client should not assume that all members are from the current tenant only.</span></span>

><span data-ttu-id="8b1ce-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b1ce-171">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats(members())",
    "@odata.count": 2,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ameeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne",
            "members@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca%40unq.gbl.spaces')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
