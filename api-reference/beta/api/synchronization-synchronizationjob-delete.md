---
title: Excluir synchronizationJob
description: Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele. As contas sincronizadas são deixadas como estão.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2c346b1020250cb1e46aa9f3c2b57f9fd5b1f1ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453020"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="9bcbd-104">Excluir synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="9bcbd-104">Delete synchronizationJob</span></span>

<span data-ttu-id="9bcbd-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9bcbd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bcbd-106">Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-106">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="9bcbd-107">As contas sincronizadas são deixadas como estão.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-107">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bcbd-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9bcbd-108">Permissions</span></span>
<span data-ttu-id="9bcbd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bcbd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bcbd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bcbd-111">Permission type</span></span>                        | <span data-ttu-id="9bcbd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9bcbd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bcbd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bcbd-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="9bcbd-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bcbd-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9bcbd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bcbd-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9bcbd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-116">Not supported.</span></span>  |
|<span data-ttu-id="9bcbd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bcbd-117">Application</span></span>                            |<span data-ttu-id="9bcbd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9bcbd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bcbd-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="9bcbd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bcbd-120">Request headers</span></span>

| <span data-ttu-id="9bcbd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9bcbd-121">Name</span></span>           | <span data-ttu-id="9bcbd-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bcbd-122">Type</span></span>    | <span data-ttu-id="9bcbd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bcbd-123">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="9bcbd-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bcbd-124">Authorization</span></span>  | <span data-ttu-id="9bcbd-125">string</span><span class="sxs-lookup"><span data-stu-id="9bcbd-125">string</span></span>  | <span data-ttu-id="9bcbd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bcbd-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bcbd-128">Request body</span></span>

<span data-ttu-id="9bcbd-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bcbd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bcbd-130">Response</span></span>

<span data-ttu-id="9bcbd-131">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-131">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="9bcbd-132">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bcbd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bcbd-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9bcbd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bcbd-134">Request</span></span>
<span data-ttu-id="9bcbd-135">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bcbd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bcbd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="9bcbd-137">C#</span><span class="sxs-lookup"><span data-stu-id="9bcbd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bcbd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bcbd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bcbd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bcbd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9bcbd-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bcbd-140">Response</span></span>
<span data-ttu-id="9bcbd-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9bcbd-141">The following is an example of the response.</span></span> 

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
