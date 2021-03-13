---
title: Excluir sincronizaçãoJob
description: Pare o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d4b154cca11b46c53d6929ea9522a7ff36c3b908
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50773575"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="b52c3-103">Excluir sincronizaçãoJob</span><span class="sxs-lookup"><span data-stu-id="b52c3-103">Delete synchronizationJob</span></span>

<span data-ttu-id="b52c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b52c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b52c3-105">Pare o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.</span><span class="sxs-lookup"><span data-stu-id="b52c3-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="b52c3-106">Contas sincronizadas são deixadas como estão.</span><span class="sxs-lookup"><span data-stu-id="b52c3-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="b52c3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b52c3-107">Permissions</span></span>
<span data-ttu-id="b52c3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b52c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b52c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b52c3-110">Permission type</span></span>                        | <span data-ttu-id="b52c3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b52c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b52c3-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b52c3-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="b52c3-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52c3-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b52c3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b52c3-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b52c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b52c3-115">Not supported.</span></span>  |
|<span data-ttu-id="b52c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b52c3-116">Application</span></span>                            |<span data-ttu-id="b52c3-117">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52c3-117">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b52c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b52c3-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="b52c3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b52c3-119">Request headers</span></span>

| <span data-ttu-id="b52c3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b52c3-120">Name</span></span>           | <span data-ttu-id="b52c3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b52c3-121">Type</span></span>    | <span data-ttu-id="b52c3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b52c3-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b52c3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b52c3-123">Authorization</span></span>  | <span data-ttu-id="b52c3-124">string</span><span class="sxs-lookup"><span data-stu-id="b52c3-124">string</span></span>  | <span data-ttu-id="b52c3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b52c3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b52c3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b52c3-127">Request body</span></span>

<span data-ttu-id="b52c3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b52c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b52c3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b52c3-129">Response</span></span>

<span data-ttu-id="b52c3-130">Se tiver êxito, retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="b52c3-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="b52c3-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b52c3-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b52c3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b52c3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b52c3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b52c3-133">Request</span></span>
<span data-ttu-id="b52c3-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b52c3-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b52c3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b52c3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="b52c3-136">C#</span><span class="sxs-lookup"><span data-stu-id="b52c3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b52c3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b52c3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b52c3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b52c3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b52c3-139">Java</span><span class="sxs-lookup"><span data-stu-id="b52c3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b52c3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b52c3-140">Response</span></span>
<span data-ttu-id="b52c3-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b52c3-141">The following is an example of the response.</span></span> 

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


