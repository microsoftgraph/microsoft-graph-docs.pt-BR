---
title: Adicionar membros à equipe
description: Adicionar um novo membro à equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 70b067b16438fb869f0c84932c5a9568f2fd0232
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968996"
---
# <a name="create-members"></a><span data-ttu-id="a71ea-103">Criar membros</span><span class="sxs-lookup"><span data-stu-id="a71ea-103">Create members</span></span>
<span data-ttu-id="a71ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a71ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a71ea-105">Adicione um novo [conversationMember](../resources/conversationmember.md) à uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a71ea-105">Add a new [conversationMember](../resources/conversationmember.md) to a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a71ea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a71ea-106">Permissions</span></span>
<span data-ttu-id="a71ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a71ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a71ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a71ea-109">Permission type</span></span>|<span data-ttu-id="a71ea-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a71ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a71ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a71ea-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a71ea-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a71ea-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="a71ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a71ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a71ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a71ea-114">Not supported.</span></span>    |
|<span data-ttu-id="a71ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a71ea-115">Application</span></span>| <span data-ttu-id="a71ea-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a71ea-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a71ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a71ea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="a71ea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a71ea-118">Request headers</span></span>
|<span data-ttu-id="a71ea-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a71ea-119">Name</span></span>|<span data-ttu-id="a71ea-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a71ea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a71ea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a71ea-121">Authorization</span></span>|<span data-ttu-id="a71ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a71ea-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a71ea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a71ea-124">Content-Type</span></span>|<span data-ttu-id="a71ea-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a71ea-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a71ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a71ea-127">Request body</span></span>
<span data-ttu-id="a71ea-128">No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="a71ea-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a71ea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a71ea-129">Response</span></span>

<span data-ttu-id="a71ea-130">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a71ea-130">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a71ea-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a71ea-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a71ea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a71ea-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a71ea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a71ea-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a71ea-134">C#</span><span class="sxs-lookup"><span data-stu-id="a71ea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a71ea-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a71ea-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a71ea-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a71ea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a71ea-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a71ea-137">Response</span></span>
<span data-ttu-id="a71ea-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a71ea-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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


