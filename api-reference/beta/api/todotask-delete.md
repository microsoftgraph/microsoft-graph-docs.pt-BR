---
title: Excluir todoTask
description: Exclui um objeto todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bdf26a600f64891e3db90d55ff31f47d2df4eee7
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849852"
---
# <a name="delete-todotask"></a><span data-ttu-id="92bd0-103">Excluir todoTask</span><span class="sxs-lookup"><span data-stu-id="92bd0-103">Delete todoTask</span></span>
<span data-ttu-id="92bd0-104">Namespace: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="92bd0-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="92bd0-105">Exclui um objeto [todoTask](../resources/todotask.md) .</span><span class="sxs-lookup"><span data-stu-id="92bd0-105">Deletes a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="92bd0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92bd0-106">Permissions</span></span>
<span data-ttu-id="92bd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92bd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92bd0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92bd0-109">Permission type</span></span>|<span data-ttu-id="92bd0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92bd0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92bd0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92bd0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="92bd0-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92bd0-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="92bd0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92bd0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92bd0-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92bd0-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="92bd0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92bd0-115">Application</span></span>|<span data-ttu-id="92bd0-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="92bd0-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="92bd0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92bd0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="92bd0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92bd0-118">Request headers</span></span>
|<span data-ttu-id="92bd0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="92bd0-119">Name</span></span>|<span data-ttu-id="92bd0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="92bd0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="92bd0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="92bd0-121">Authorization</span></span>|<span data-ttu-id="92bd0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92bd0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92bd0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92bd0-124">Request body</span></span>
<span data-ttu-id="92bd0-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92bd0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92bd0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="92bd0-126">Response</span></span>

<span data-ttu-id="92bd0-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="92bd0-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="92bd0-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="92bd0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="92bd0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92bd0-129">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "name": "delete_todotask"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
```


### <a name="response"></a><span data-ttu-id="92bd0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="92bd0-130">Response</span></span>
<span data-ttu-id="92bd0-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="92bd0-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

