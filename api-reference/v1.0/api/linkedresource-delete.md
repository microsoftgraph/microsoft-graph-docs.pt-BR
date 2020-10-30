---
title: Excluir linkedResource
description: Exclui um objeto linkedResource.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 67ad5dedf3f5e8f94d2923320a9407cee67f35ff
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797174"
---
# <a name="delete-linkedresource"></a><span data-ttu-id="7bf50-103">Excluir linkedResource</span><span class="sxs-lookup"><span data-stu-id="7bf50-103">Delete linkedResource</span></span>
<span data-ttu-id="7bf50-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bf50-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bf50-105">Exclui um objeto [linkedResource](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="7bf50-105">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bf50-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bf50-106">Permissions</span></span>
<span data-ttu-id="7bf50-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bf50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bf50-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bf50-109">Permission type</span></span>|<span data-ttu-id="7bf50-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7bf50-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bf50-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bf50-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7bf50-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bf50-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="7bf50-113">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="7bf50-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bf50-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7bf50-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="7bf50-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bf50-115">Application</span></span>|<span data-ttu-id="7bf50-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7bf50-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bf50-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf50-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
DELETE /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/linkedResources/{linkedResourcesId}
```

## <a name="request-headers"></a><span data-ttu-id="7bf50-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf50-118">Request headers</span></span>
|<span data-ttu-id="7bf50-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7bf50-119">Name</span></span>|<span data-ttu-id="7bf50-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bf50-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7bf50-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bf50-121">Authorization</span></span>|<span data-ttu-id="7bf50-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bf50-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bf50-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf50-124">Request body</span></span>
<span data-ttu-id="7bf50-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bf50-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bf50-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf50-126">Response</span></span>

<span data-ttu-id="7bf50-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7bf50-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7bf50-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7bf50-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bf50-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf50-129">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["dfsdc-f9dfdfs-dcsda9", "e2dc-f9cce2-dce29", "f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9"],
  "name": "delete_linkedresource"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9
```


### <a name="response"></a><span data-ttu-id="7bf50-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf50-130">Response</span></span>
<span data-ttu-id="7bf50-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7bf50-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```



