---
title: Adicionar membros à equipe
description: Adicionar um novo membro à equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 32a9cceb77c142f31fbaac44ab4f8e782f89e560
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974564"
---
# <a name="create-members"></a><span data-ttu-id="00fd3-103">Criar membros</span><span class="sxs-lookup"><span data-stu-id="00fd3-103">Create members</span></span>
<span data-ttu-id="00fd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00fd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00fd3-105">Adicione um novo [conversationMember](../resources/conversationmember.md) à uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="00fd3-105">Add a new [conversationMember](../resources/conversationmember.md) to a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="00fd3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="00fd3-106">Permissions</span></span>
<span data-ttu-id="00fd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00fd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00fd3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00fd3-109">Permission type</span></span>|<span data-ttu-id="00fd3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00fd3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00fd3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00fd3-111">Delegated (work or school account)</span></span>| <span data-ttu-id="00fd3-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00fd3-112">TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="00fd3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00fd3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00fd3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00fd3-114">Not supported.</span></span>    |
|<span data-ttu-id="00fd3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00fd3-115">Application</span></span>| <span data-ttu-id="00fd3-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00fd3-116">TeamMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00fd3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00fd3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/members
POST /teams/{teamsId}/channels/{channelId}/members
```

## <a name="request-headers"></a><span data-ttu-id="00fd3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00fd3-118">Request headers</span></span>
|<span data-ttu-id="00fd3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="00fd3-119">Name</span></span>|<span data-ttu-id="00fd3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="00fd3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="00fd3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="00fd3-121">Authorization</span></span>|<span data-ttu-id="00fd3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00fd3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="00fd3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00fd3-124">Content-Type</span></span>|<span data-ttu-id="00fd3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00fd3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00fd3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00fd3-127">Request body</span></span>
<span data-ttu-id="00fd3-128">No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md).</span><span class="sxs-lookup"><span data-stu-id="00fd3-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00fd3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="00fd3-129">Response</span></span>

<span data-ttu-id="00fd3-130">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00fd3-130">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span> <span data-ttu-id="00fd3-131">Para obter melhores resultados, coordene chamadas com 2 segundos de buffer.</span><span class="sxs-lookup"><span data-stu-id="00fd3-131">For best results, stagger calls with 2 seconds of buffer.</span></span>

<span data-ttu-id="00fd3-132">Para obter melhores resultados, coordene chamadas com 2 segundos de buffer.</span><span class="sxs-lookup"><span data-stu-id="00fd3-132">For best results, stagger calls with a 2 second buffer.</span></span>

## <a name="examples"></a><span data-ttu-id="00fd3-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="00fd3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="00fd3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00fd3-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="00fd3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="00fd3-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="00fd3-136">C#</span><span class="sxs-lookup"><span data-stu-id="00fd3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversationmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00fd3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00fd3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversationmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00fd3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00fd3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversationmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00fd3-139">Java</span><span class="sxs-lookup"><span data-stu-id="00fd3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversationmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="00fd3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="00fd3-140">Response</span></span>
<span data-ttu-id="00fd3-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="00fd3-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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


