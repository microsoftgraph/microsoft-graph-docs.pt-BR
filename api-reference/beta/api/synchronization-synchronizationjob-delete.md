---
title: Excluir synchronizationJob
description: Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele. As contas sincronizadas são deixadas como estão.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 45e0f9f44aa87efac3f03a05cbc3fbad22a6cb86
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621162"
---
# <a name="delete-synchronizationjob"></a><span data-ttu-id="a5f8c-104">Excluir synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="a5f8c-104">Delete synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5f8c-105">Interrompa o trabalho de sincronização e exclua permanentemente todo o estado associado a ele.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-105">Stop the synchronization job, and permanently delete all the state associated with it.</span></span> <span data-ttu-id="a5f8c-106">As contas sincronizadas são deixadas como estão.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-106">Synchronized accounts are left as-is.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5f8c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5f8c-107">Permissions</span></span>
<span data-ttu-id="a5f8c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5f8c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5f8c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5f8c-110">Permission type</span></span>                        | <span data-ttu-id="a5f8c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5f8c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5f8c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5f8c-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="a5f8c-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f8c-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a5f8c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5f8c-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a5f8c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-115">Not supported.</span></span>  |
|<span data-ttu-id="a5f8c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5f8c-116">Application</span></span>                            |<span data-ttu-id="a5f8c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a5f8c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5f8c-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="a5f8c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f8c-119">Request headers</span></span>

| <span data-ttu-id="a5f8c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a5f8c-120">Name</span></span>           | <span data-ttu-id="a5f8c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5f8c-121">Type</span></span>    | <span data-ttu-id="a5f8c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5f8c-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a5f8c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5f8c-123">Authorization</span></span>  | <span data-ttu-id="a5f8c-124">string</span><span class="sxs-lookup"><span data-stu-id="a5f8c-124">string</span></span>  | <span data-ttu-id="a5f8c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5f8c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f8c-127">Request body</span></span>

<span data-ttu-id="a5f8c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5f8c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5f8c-129">Response</span></span>

<span data-ttu-id="a5f8c-130">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="a5f8c-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5f8c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5f8c-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5f8c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5f8c-133">Request</span></span>
<span data-ttu-id="a5f8c-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a5f8c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5f8c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_synchronizationjob"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5f8c-136">C#</span><span class="sxs-lookup"><span data-stu-id="a5f8c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5f8c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a5f8c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5f8c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a5f8c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5f8c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5f8c-139">Response</span></span>
<span data-ttu-id="a5f8c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5f8c-140">The following is an example of the response.</span></span> 

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
