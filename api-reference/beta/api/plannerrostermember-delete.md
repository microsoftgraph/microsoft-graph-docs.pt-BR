---
title: Excluir plannerRosterMember
description: Exclui um objeto plannerRosterMember.
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: d6101b5c82bc2eb7a631d01df00f447398f87715
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272064"
---
# <a name="delete-plannerrostermember"></a><span data-ttu-id="a3e1c-103">Excluir plannerRosterMember</span><span class="sxs-lookup"><span data-stu-id="a3e1c-103">Delete plannerRosterMember</span></span>
<span data-ttu-id="a3e1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3e1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3e1c-105">[Exclua um objeto plannerRosterMember.](../resources/plannerrostermember.md)</span><span class="sxs-lookup"><span data-stu-id="a3e1c-105">Delete a [plannerRosterMember](../resources/plannerrostermember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3e1c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a3e1c-106">Permissions</span></span>
<span data-ttu-id="a3e1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3e1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3e1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3e1c-109">Permission type</span></span>|<span data-ttu-id="a3e1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3e1c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3e1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3e1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3e1c-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3e1c-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="a3e1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3e1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3e1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3e1c-114">Not supported.</span></span>|
|<span data-ttu-id="a3e1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3e1c-115">Application</span></span>|<span data-ttu-id="a3e1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3e1c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3e1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3e1c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /planner/rosters/{plannerRosterId}/members/{plannerRosterMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="a3e1c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e1c-118">Request headers</span></span>
|<span data-ttu-id="a3e1c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a3e1c-119">Name</span></span>|<span data-ttu-id="a3e1c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3e1c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a3e1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3e1c-121">Authorization</span></span>|<span data-ttu-id="a3e1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3e1c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3e1c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e1c-124">Request body</span></span>
<span data-ttu-id="a3e1c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3e1c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3e1c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3e1c-126">Response</span></span>

<span data-ttu-id="a3e1c-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a3e1c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a3e1c-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a3e1c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3e1c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3e1c-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a3e1c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3e1c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerrostermember"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/planner/rosters/523a9d5a-f9d5-45c1-929f-b8525393515c/members/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38
```
# <a name="c"></a>[<span data-ttu-id="a3e1c-131">C#</span><span class="sxs-lookup"><span data-stu-id="a3e1c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerrostermember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3e1c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3e1c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerrostermember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3e1c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3e1c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerrostermember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3e1c-134">Java</span><span class="sxs-lookup"><span data-stu-id="a3e1c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerrostermember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a3e1c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3e1c-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

