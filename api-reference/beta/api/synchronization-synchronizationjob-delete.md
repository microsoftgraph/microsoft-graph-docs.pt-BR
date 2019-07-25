---
title: Excluir synchronizationJob
description: Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele. As contas sincronizadas são deixadas como estão.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 43378dccfb17777b15d06f5d8ffdcedcdb386dd9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869383"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="95bba-104">Excluir synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="95bba-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95bba-105">Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.</span><span class="sxs-lookup"><span data-stu-id="95bba-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="95bba-106">As contas sincronizadas são deixadas como estão.</span><span class="sxs-lookup"><span data-stu-id="95bba-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="95bba-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="95bba-107">Permissions</span></span>
<span data-ttu-id="95bba-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95bba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95bba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95bba-110">Permission type</span></span>                        | <span data-ttu-id="95bba-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95bba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="95bba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95bba-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="95bba-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95bba-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="95bba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95bba-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="95bba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95bba-115">Not supported.</span></span>  |
|<span data-ttu-id="95bba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95bba-116">Application</span></span>                            |<span data-ttu-id="95bba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95bba-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="95bba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95bba-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="95bba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95bba-119">Request headers</span></span>

| <span data-ttu-id="95bba-120">Nome</span><span class="sxs-lookup"><span data-stu-id="95bba-120">Name</span></span>           | <span data-ttu-id="95bba-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="95bba-121">Type</span></span>    | <span data-ttu-id="95bba-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="95bba-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="95bba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95bba-123">Authorization</span></span>  | <span data-ttu-id="95bba-124">string</span><span class="sxs-lookup"><span data-stu-id="95bba-124">string</span></span>  | <span data-ttu-id="95bba-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95bba-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95bba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95bba-127">Request body</span></span>

<span data-ttu-id="95bba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="95bba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95bba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="95bba-129">Response</span></span>

<span data-ttu-id="95bba-130">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="95bba-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="95bba-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95bba-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95bba-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95bba-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="95bba-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95bba-133">Request</span></span>
<span data-ttu-id="95bba-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="95bba-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="95bba-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="95bba-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="95bba-136">C#</span><span class="sxs-lookup"><span data-stu-id="95bba-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95bba-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="95bba-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95bba-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="95bba-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="95bba-139">Java</span><span class="sxs-lookup"><span data-stu-id="95bba-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="95bba-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="95bba-140">Response</span></span>
<span data-ttu-id="95bba-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="95bba-141">The following is an example of the response.</span></span> 

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
