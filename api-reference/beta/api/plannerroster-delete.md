---
title: Excluir plannerRoster
description: Exclui um objeto plannerRoster .
author: tarkansevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: e6159e9a5f4a230e3bb60f04fca6abdee1ee3a97
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271915"
---
# <a name="delete-plannerroster"></a><span data-ttu-id="48e70-103">Excluir plannerRoster</span><span class="sxs-lookup"><span data-stu-id="48e70-103">Delete plannerRoster</span></span>
<span data-ttu-id="48e70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48e70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48e70-105">Exclua [um objeto plannerRoster.](../resources/plannerroster.md)</span><span class="sxs-lookup"><span data-stu-id="48e70-105">Delete a [plannerRoster](../resources/plannerroster.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48e70-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="48e70-106">Permissions</span></span>
<span data-ttu-id="48e70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48e70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48e70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48e70-109">Permission type</span></span>|<span data-ttu-id="48e70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48e70-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48e70-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48e70-111">Delegated (work or school account)</span></span>|<span data-ttu-id="48e70-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48e70-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="48e70-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48e70-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48e70-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48e70-114">Not supported.</span></span>|
|<span data-ttu-id="48e70-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48e70-115">Application</span></span>|<span data-ttu-id="48e70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48e70-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48e70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48e70-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /planner/rosters/{plannerRosterId}
```

## <a name="request-headers"></a><span data-ttu-id="48e70-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48e70-118">Request headers</span></span>
|<span data-ttu-id="48e70-119">Nome</span><span class="sxs-lookup"><span data-stu-id="48e70-119">Name</span></span>|<span data-ttu-id="48e70-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e70-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="48e70-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="48e70-121">Authorization</span></span>|<span data-ttu-id="48e70-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48e70-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48e70-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48e70-124">Request body</span></span>
<span data-ttu-id="48e70-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48e70-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48e70-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="48e70-126">Response</span></span>

<span data-ttu-id="48e70-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="48e70-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="48e70-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="48e70-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48e70-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48e70-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="48e70-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="48e70-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_plannerroster"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/planner/rosters/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38
```
# <a name="c"></a>[<span data-ttu-id="48e70-131">C#</span><span class="sxs-lookup"><span data-stu-id="48e70-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-plannerroster-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48e70-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48e70-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-plannerroster-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48e70-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48e70-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-plannerroster-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="48e70-134">Java</span><span class="sxs-lookup"><span data-stu-id="48e70-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-plannerroster-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="48e70-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="48e70-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

