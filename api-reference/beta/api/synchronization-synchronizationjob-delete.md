---
title: Excluir synchronizationJob
description: Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd732200b8ab02be3bffc443272a45f2da8a9a77
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466431"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="3514b-103">Excluir synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="3514b-103">Delete synchronizationJob</span></span>

<span data-ttu-id="3514b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3514b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3514b-105">Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.</span><span class="sxs-lookup"><span data-stu-id="3514b-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="3514b-106">As contas sincronizadas são deixadas como estão.</span><span class="sxs-lookup"><span data-stu-id="3514b-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="3514b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3514b-107">Permissions</span></span>
<span data-ttu-id="3514b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3514b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3514b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3514b-110">Permission type</span></span>                        | <span data-ttu-id="3514b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3514b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3514b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3514b-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="3514b-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3514b-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3514b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3514b-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3514b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3514b-115">Not supported.</span></span>  |
|<span data-ttu-id="3514b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3514b-116">Application</span></span>                            |<span data-ttu-id="3514b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3514b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3514b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3514b-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="3514b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3514b-119">Request headers</span></span>

| <span data-ttu-id="3514b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3514b-120">Name</span></span>           | <span data-ttu-id="3514b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3514b-121">Type</span></span>    | <span data-ttu-id="3514b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3514b-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3514b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3514b-123">Authorization</span></span>  | <span data-ttu-id="3514b-124">string</span><span class="sxs-lookup"><span data-stu-id="3514b-124">string</span></span>  | <span data-ttu-id="3514b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3514b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3514b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3514b-127">Request body</span></span>

<span data-ttu-id="3514b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3514b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3514b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3514b-129">Response</span></span>

<span data-ttu-id="3514b-130">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3514b-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="3514b-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3514b-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3514b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3514b-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3514b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3514b-133">Request</span></span>
<span data-ttu-id="3514b-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3514b-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3514b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3514b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="3514b-136">C#</span><span class="sxs-lookup"><span data-stu-id="3514b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3514b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3514b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3514b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3514b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3514b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3514b-139">Response</span></span>
<span data-ttu-id="3514b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3514b-140">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
