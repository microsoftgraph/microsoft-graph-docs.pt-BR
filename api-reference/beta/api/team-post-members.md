---
title: Adicionar membros à equipe
description: Adicionar um novo membro a uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 77c70173dd029c7a92f6e31bffa5d092528aa008
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050987"
---
# <a name="create-members"></a><span data-ttu-id="6f84a-103">Criar membros</span><span class="sxs-lookup"><span data-stu-id="6f84a-103">Create members</span></span>
<span data-ttu-id="6f84a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f84a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f84a-105">Adicione um novo [conversationMember](../resources/conversationmember.md) a uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="6f84a-105">Add a new [conversationMember](../resources/conversationmember.md) to a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f84a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f84a-106">Permissions</span></span>
<span data-ttu-id="6f84a-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6f84a-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6f84a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f84a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f84a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f84a-109">Permission type</span></span>|<span data-ttu-id="6f84a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f84a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f84a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f84a-111">Delegated (work or school account)</span></span>| <span data-ttu-id="6f84a-112">TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6f84a-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="6f84a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f84a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f84a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f84a-114">Not supported.</span></span>    |
|<span data-ttu-id="6f84a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f84a-115">Application</span></span>| <span data-ttu-id="6f84a-116">TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6f84a-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f84a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f84a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="6f84a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f84a-118">Request headers</span></span>
|<span data-ttu-id="6f84a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6f84a-119">Name</span></span>|<span data-ttu-id="6f84a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f84a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f84a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f84a-121">Authorization</span></span>|<span data-ttu-id="6f84a-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6f84a-122">Bearer {token}.</span></span> <span data-ttu-id="6f84a-123">Required.</span><span class="sxs-lookup"><span data-stu-id="6f84a-123">Required.</span></span>|
|<span data-ttu-id="6f84a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f84a-124">Content-Type</span></span>|<span data-ttu-id="6f84a-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="6f84a-125">application/json.</span></span> <span data-ttu-id="6f84a-126">Required.</span><span class="sxs-lookup"><span data-stu-id="6f84a-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f84a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f84a-127">Request body</span></span>
<span data-ttu-id="6f84a-128">No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md) .</span><span class="sxs-lookup"><span data-stu-id="6f84a-128">In the request body, supply a JSON representation of the [conversationMember](../resources/conversationmember.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6f84a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f84a-129">Response</span></span>

<span data-ttu-id="6f84a-130">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f84a-130">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f84a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6f84a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f84a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f84a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{id}/members
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "roles": [
        "owner"
    ],
    "userId": "50dffbae-ad0f-428e-a86f-f53b0acfc641",
    "displayName": "Cameron White",
    "email": "CameronW@M365x987948.OnMicrosoft.com"
}
```


### <a name="response"></a><span data-ttu-id="6f84a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f84a-133">Response</span></span>
<span data-ttu-id="6f84a-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f84a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
