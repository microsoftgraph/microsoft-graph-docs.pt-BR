---
title: Iniciar synchronizationJob
description: Inicie um trabalho de sincronização existente. Se o trabalho estiver em um estado pausado, ele continuará a processar as alterações do ponto em que foi pausado. Se o trabalho estiver em quarentena, o status da quarentena será limpo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1fae704446d35c7a93d850f25f31355f50d332e0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132756"
---
# <a name="start-synchronizationjob"></a><span data-ttu-id="5d029-105">Iniciar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="5d029-105">Start synchronizationJob</span></span>

<span data-ttu-id="5d029-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d029-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d029-107">Inicie um trabalho de sincronização existente.</span><span class="sxs-lookup"><span data-stu-id="5d029-107">Start an existing synchronization job.</span></span> <span data-ttu-id="5d029-108">Se o trabalho estiver em um estado pausado, ele continuará a processar as alterações do ponto em que foi pausado.</span><span class="sxs-lookup"><span data-stu-id="5d029-108">If the job is in a paused state, it will continue processing changes from the point where it was paused.</span></span> <span data-ttu-id="5d029-109">Se o trabalho estiver em quarentena, o status da quarentena será limpo.</span><span class="sxs-lookup"><span data-stu-id="5d029-109">If the job is in quarantine, the quarantine status will be cleared.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d029-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d029-110">Permissions</span></span>
<span data-ttu-id="5d029-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d029-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d029-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d029-113">Permission type</span></span>                        | <span data-ttu-id="5d029-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d029-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d029-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d029-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="5d029-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d029-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5d029-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d029-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5d029-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d029-118">Not supported.</span></span> |
|<span data-ttu-id="5d029-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d029-119">Application</span></span>                            |<span data-ttu-id="5d029-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d029-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5d029-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d029-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```

## <a name="request-headers"></a><span data-ttu-id="5d029-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d029-122">Request headers</span></span>

| <span data-ttu-id="5d029-123">Nome</span><span class="sxs-lookup"><span data-stu-id="5d029-123">Name</span></span>           | <span data-ttu-id="5d029-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d029-124">Type</span></span>    | <span data-ttu-id="5d029-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d029-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5d029-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d029-126">Authorization</span></span>  | <span data-ttu-id="5d029-127">string</span><span class="sxs-lookup"><span data-stu-id="5d029-127">string</span></span>  | <span data-ttu-id="5d029-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d029-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d029-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d029-130">Request body</span></span>

<span data-ttu-id="5d029-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d029-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="5d029-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d029-132">Response</span></span>

<span data-ttu-id="5d029-133">Se tiver êxito, retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="5d029-133">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="5d029-134">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d029-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d029-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d029-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5d029-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d029-136">Request</span></span>
<span data-ttu-id="5d029-137">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d029-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5d029-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d029-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_start"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/start
```
# <a name="c"></a>[<span data-ttu-id="5d029-139">C#</span><span class="sxs-lookup"><span data-stu-id="5d029-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d029-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d029-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d029-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d029-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d029-142">Java</span><span class="sxs-lookup"><span data-stu-id="5d029-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5d029-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d029-143">Response</span></span>
<span data-ttu-id="5d029-144">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5d029-144">The following is an example of a response.</span></span>
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


