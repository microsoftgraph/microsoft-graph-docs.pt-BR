---
title: Excluir todoTaskList
description: Exclui um objeto todoTaskList.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fed835f834b7bd65816613c2d37666294db6be62
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058512"
---
# <a name="delete-todotasklist"></a><span data-ttu-id="eaf97-103">Excluir todoTaskList</span><span class="sxs-lookup"><span data-stu-id="eaf97-103">Delete todoTaskList</span></span>
<span data-ttu-id="eaf97-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="eaf97-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="eaf97-105">Exclui um objeto [todoTaskList](../resources/todotasklist.md) .</span><span class="sxs-lookup"><span data-stu-id="eaf97-105">Deletes a [todoTaskList](../resources/todotasklist.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaf97-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaf97-106">Permissions</span></span>
<span data-ttu-id="eaf97-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf97-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaf97-109">Permission type</span></span>|<span data-ttu-id="eaf97-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eaf97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaf97-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaf97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eaf97-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="eaf97-112">Tasks.Read</span></span>|
|<span data-ttu-id="eaf97-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eaf97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaf97-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="eaf97-114">Tasks.Read</span></span>|
|<span data-ttu-id="eaf97-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaf97-115">Application</span></span>|<span data-ttu-id="eaf97-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="eaf97-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaf97-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaf97-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}
```

## <a name="request-headers"></a><span data-ttu-id="eaf97-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf97-118">Request headers</span></span>
|<span data-ttu-id="eaf97-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eaf97-119">Name</span></span>|<span data-ttu-id="eaf97-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf97-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eaf97-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaf97-121">Authorization</span></span>|<span data-ttu-id="eaf97-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaf97-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaf97-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf97-124">Request body</span></span>
<span data-ttu-id="eaf97-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eaf97-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaf97-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaf97-126">Response</span></span>

<span data-ttu-id="eaf97-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eaf97-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="eaf97-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eaf97-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eaf97-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eaf97-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eaf97-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="eaf97-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADIyAAAhrbPXAAA="],
  "name": "delete_todotasklist"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="eaf97-131">C#</span><span class="sxs-lookup"><span data-stu-id="eaf97-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-todotasklist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eaf97-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eaf97-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-todotasklist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eaf97-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eaf97-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-todotasklist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eaf97-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaf97-134">Response</span></span>
<span data-ttu-id="eaf97-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaf97-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



