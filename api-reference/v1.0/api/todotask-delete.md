---
title: Excluir todoTask
description: Exclui um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ca86b2344e67c86418c8bc5d2d3914148994f1e9
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797214"
---
# <a name="delete-todotask"></a><span data-ttu-id="299b5-103">Excluir todoTask</span><span class="sxs-lookup"><span data-stu-id="299b5-103">Delete todoTask</span></span>
<span data-ttu-id="299b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="299b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="299b5-105">Exclui um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="299b5-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="299b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="299b5-106">Permissions</span></span>
<span data-ttu-id="299b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="299b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="299b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="299b5-109">Permission type</span></span>|<span data-ttu-id="299b5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="299b5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="299b5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="299b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="299b5-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="299b5-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="299b5-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="299b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="299b5-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="299b5-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="299b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="299b5-115">Application</span></span>|<span data-ttu-id="299b5-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="299b5-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="299b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="299b5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="299b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="299b5-118">Request headers</span></span>
|<span data-ttu-id="299b5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="299b5-119">Name</span></span>|<span data-ttu-id="299b5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="299b5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="299b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="299b5-121">Authorization</span></span>|<span data-ttu-id="299b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="299b5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="299b5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="299b5-124">Request body</span></span>
<span data-ttu-id="299b5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="299b5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="299b5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="299b5-126">Response</span></span>

<span data-ttu-id="299b5-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="299b5-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="299b5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="299b5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="299b5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="299b5-129">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```


### <a name="response"></a><span data-ttu-id="299b5-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="299b5-130">Response</span></span>
<span data-ttu-id="299b5-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="299b5-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



