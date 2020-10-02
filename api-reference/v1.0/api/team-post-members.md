---
title: Adicionar membros à equipe
description: Adicionar um novo membro à equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eb59f85ed355d61b15a937cd66b8e3e3d4589849
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48329994"
---
# <a name="create-members"></a><span data-ttu-id="05c2c-103">Criar membros</span><span class="sxs-lookup"><span data-stu-id="05c2c-103">Create members</span></span>
<span data-ttu-id="05c2c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05c2c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05c2c-105">Adicione um novo [conversationMember](../resources/conversationmember.md) à uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="05c2c-105">Add a new [conversationMember](../resources/conversationmember.md) to a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05c2c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05c2c-106">Permissions</span></span>
<span data-ttu-id="05c2c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05c2c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05c2c-109">Permission type</span></span>|<span data-ttu-id="05c2c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05c2c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05c2c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05c2c-111">Delegated (work or school account)</span></span>| <span data-ttu-id="05c2c-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c2c-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="05c2c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05c2c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05c2c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c2c-114">Not supported.</span></span>    |
|<span data-ttu-id="05c2c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05c2c-115">Application</span></span>| <span data-ttu-id="05c2c-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c2c-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05c2c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05c2c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/members
POST /teams/{teamsId}/channels/{channelId}/members
```

## <a name="request-headers"></a><span data-ttu-id="05c2c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05c2c-118">Request headers</span></span>
|<span data-ttu-id="05c2c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="05c2c-119">Name</span></span>|<span data-ttu-id="05c2c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c2c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="05c2c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="05c2c-121">Authorization</span></span>|<span data-ttu-id="05c2c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05c2c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05c2c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05c2c-124">Content-Type</span></span>|<span data-ttu-id="05c2c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05c2c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05c2c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05c2c-127">Request body</span></span>
<span data-ttu-id="05c2c-128">No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="05c2c-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="05c2c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c2c-129">Response</span></span>

<span data-ttu-id="05c2c-130">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05c2c-130">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05c2c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="05c2c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05c2c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c2c-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="05c2c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="05c2c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversationmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{id}/members
Content-type: application/json
Content-length: 26

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": ["owner"],
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```
# <a name="c"></a>[<span data-ttu-id="05c2c-134">C#</span><span class="sxs-lookup"><span data-stu-id="05c2c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05c2c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05c2c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05c2c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05c2c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05c2c-137">Java</span><span class="sxs-lookup"><span data-stu-id="05c2c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="05c2c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c2c-138">Response</span></span>
<span data-ttu-id="05c2c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="05c2c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
