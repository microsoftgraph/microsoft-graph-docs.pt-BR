---
title: Iniciar synchronizationJob
description: Inicie um trabalho de sincronização existente. Se o trabalho estiver em um estado pausado, ele continuará processando as alterações do ponto em que foi pausado. Se o trabalho estiver em quarentena, o status da quarentena será limpo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8135c81c0046dfd67b830e0c8c8a075e4550ef74
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044288"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="0cead-105">Iniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="0cead-105">Start synchronizationJob</span></span>

<span data-ttu-id="0cead-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cead-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cead-107">Inicie um trabalho de sincronização existente.</span><span class="sxs-lookup"><span data-stu-id="0cead-107">Start an existing synchronization job.</span></span> <span data-ttu-id="0cead-108">Se o trabalho estiver em um estado pausado, ele continuará processando as alterações do ponto em que foi pausado.</span><span class="sxs-lookup"><span data-stu-id="0cead-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="0cead-109">Se o trabalho estiver em quarentena, o status da quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="0cead-109">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cead-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cead-110">Permissions</span></span>
<span data-ttu-id="0cead-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cead-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cead-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cead-113">Permission type</span></span>                        | <span data-ttu-id="0cead-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cead-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cead-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cead-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="0cead-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cead-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0cead-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cead-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0cead-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cead-118">Not supported.</span></span> |
|<span data-ttu-id="0cead-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cead-119">Application</span></span>                            |<span data-ttu-id="0cead-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cead-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0cead-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cead-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="0cead-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cead-122">Request headers</span></span>

| <span data-ttu-id="0cead-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0cead-123">Name</span></span>           | <span data-ttu-id="0cead-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cead-124">Type</span></span>    | <span data-ttu-id="0cead-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cead-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0cead-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cead-126">Authorization</span></span>  | <span data-ttu-id="0cead-127">string</span><span class="sxs-lookup"><span data-stu-id="0cead-127">string</span></span>  | <span data-ttu-id="0cead-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cead-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cead-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cead-130">Request body</span></span>

<span data-ttu-id="0cead-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0cead-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="0cead-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cead-132">Response</span></span>

<span data-ttu-id="0cead-133">Se tiver êxito, retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="0cead-133">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="0cead-134">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cead-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cead-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cead-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0cead-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cead-136">Request</span></span>
<span data-ttu-id="0cead-137">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cead-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cead-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cead-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="0cead-139">C#</span><span class="sxs-lookup"><span data-stu-id="0cead-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cead-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cead-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cead-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cead-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0cead-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cead-142">Response</span></span>
<span data-ttu-id="0cead-143">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0cead-143">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: start",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


