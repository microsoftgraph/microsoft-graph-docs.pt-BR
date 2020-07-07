---
title: Remover membros da equipe
description: Remover um conversationMember de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8ad51fddf0acf4499271ffeb3c02e0433e52dedb
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051013"
---
# <a name="delete-members"></a><span data-ttu-id="ddc46-103">Excluir Membros</span><span class="sxs-lookup"><span data-stu-id="ddc46-103">Delete members</span></span>
<span data-ttu-id="ddc46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddc46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ddc46-105">Remover um novo [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ddc46-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddc46-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddc46-106">Permissions</span></span>
<span data-ttu-id="ddc46-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ddc46-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ddc46-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddc46-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddc46-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddc46-109">Permission type</span></span>|<span data-ttu-id="ddc46-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ddc46-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddc46-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddc46-111">Delegated (work or school account)</span></span>| <span data-ttu-id="ddc46-112">TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ddc46-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="ddc46-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddc46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddc46-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddc46-114">Not supported.</span></span>    |
|<span data-ttu-id="ddc46-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddc46-115">Application</span></span>| <span data-ttu-id="ddc46-116">TeamMember. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ddc46-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddc46-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddc46-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{teamsId}/members
```

## <a name="request-headers"></a><span data-ttu-id="ddc46-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc46-118">Request headers</span></span>
|<span data-ttu-id="ddc46-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ddc46-119">Name</span></span>|<span data-ttu-id="ddc46-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddc46-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ddc46-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddc46-121">Authorization</span></span>|<span data-ttu-id="ddc46-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ddc46-122">Bearer {token}.</span></span> <span data-ttu-id="ddc46-123">Required.</span><span class="sxs-lookup"><span data-stu-id="ddc46-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddc46-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc46-124">Request body</span></span>
<span data-ttu-id="ddc46-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddc46-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddc46-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddc46-126">Response</span></span>

<span data-ttu-id="ddc46-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ddc46-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ddc46-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddc46-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddc46-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddc46-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```


### <a name="response"></a><span data-ttu-id="ddc46-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddc46-130">Response</span></span>
<span data-ttu-id="ddc46-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ddc46-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

