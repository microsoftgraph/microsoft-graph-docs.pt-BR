---
title: Adicionar membros à equipe
description: Adicionar um novo membro à equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fd4c02b3b981394edfafd389eb7adf2afc9e52d9
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123810"
---
# <a name="create-members"></a><span data-ttu-id="861b4-103">Criar membros</span><span class="sxs-lookup"><span data-stu-id="861b4-103">Create members</span></span>
<span data-ttu-id="861b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="861b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="861b4-105">Adicione um novo [conversationMember](../resources/conversationmember.md) à uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="861b4-105">Add a new [conversationMember](../resources/conversationmember.md) to a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="861b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="861b4-106">Permissions</span></span>
<span data-ttu-id="861b4-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="861b4-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="861b4-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861b4-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="861b4-109">Permission type</span></span>|<span data-ttu-id="861b4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="861b4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="861b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="861b4-111">Delegated (work or school account)</span></span>| <span data-ttu-id="861b4-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861b4-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="861b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="861b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="861b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="861b4-114">Not supported.</span></span>    |
|<span data-ttu-id="861b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="861b4-115">Application</span></span>| <span data-ttu-id="861b4-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861b4-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="861b4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="861b4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="861b4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="861b4-118">Request headers</span></span>
|<span data-ttu-id="861b4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="861b4-119">Name</span></span>|<span data-ttu-id="861b4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="861b4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="861b4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="861b4-121">Authorization</span></span>|<span data-ttu-id="861b4-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="861b4-122">Bearer {token}.</span></span> <span data-ttu-id="861b4-123">Required.</span><span class="sxs-lookup"><span data-stu-id="861b4-123">Required.</span></span>|
|<span data-ttu-id="861b4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="861b4-124">Content-Type</span></span>|<span data-ttu-id="861b4-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="861b4-125">application/json.</span></span> <span data-ttu-id="861b4-126">Required.</span><span class="sxs-lookup"><span data-stu-id="861b4-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="861b4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="861b4-127">Request body</span></span>
<span data-ttu-id="861b4-128">No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="861b4-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="861b4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="861b4-129">Response</span></span>

<span data-ttu-id="861b4-130">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="861b4-130">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="861b4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="861b4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="861b4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="861b4-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="861b4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="861b4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{id}/members
Content-type: application/json
Content-length: 26

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="861b4-134">C#</span><span class="sxs-lookup"><span data-stu-id="861b4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="861b4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="861b4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="861b4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="861b4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="861b4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="861b4-137">Response</span></span>
<span data-ttu-id="861b4-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="861b4-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "3c02af05-9312-4966-bc84-c1a0818791c4",
    "roles": [
        "owner"
    ],
    "userId": "50dffbae-ad0f-428e-a86f-f53b0acfc641",
    "displayName": "Cameron White",
    "email": "CameronW@M365x987948.OnMicrosoft.com"
}
```
