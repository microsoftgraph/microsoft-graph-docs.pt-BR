---
title: 'synchronizationJob: pausar'
description: Interromper temporariamente a sincronização. Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada inicial é feita.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3049b771bda224162be3614e14309610928e810c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409776"
---
# <a name="synchronizationjob-pause"></a><span data-ttu-id="ee46e-104">synchronizationJob: pausar</span><span class="sxs-lookup"><span data-stu-id="ee46e-104">synchronizationJob: pause</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee46e-105">Interromper temporariamente a sincronização.</span><span class="sxs-lookup"><span data-stu-id="ee46e-105">Temporarily stop synchronization.</span></span> <span data-ttu-id="ee46e-106">Todo o progresso, incluindo o estado do trabalho, é mantido e o trabalho continuará de onde parou quando uma chamada [inicial](../api/synchronization-synchronizationjob-start.md) é feita.</span><span class="sxs-lookup"><span data-stu-id="ee46e-106">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee46e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee46e-107">Permissions</span></span>
<span data-ttu-id="ee46e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee46e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee46e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee46e-110">Permission type</span></span>                        | <span data-ttu-id="ee46e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee46e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee46e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee46e-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="ee46e-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee46e-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ee46e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee46e-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ee46e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee46e-115">Not supported.</span></span>  |
|<span data-ttu-id="ee46e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee46e-116">Application</span></span>                            |<span data-ttu-id="ee46e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee46e-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ee46e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee46e-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```

## <a name="request-headers"></a><span data-ttu-id="ee46e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee46e-119">Request headers</span></span>

| <span data-ttu-id="ee46e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ee46e-120">Name</span></span>           | <span data-ttu-id="ee46e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee46e-121">Type</span></span>    | <span data-ttu-id="ee46e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee46e-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ee46e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee46e-123">Authorization</span></span>  | <span data-ttu-id="ee46e-124">string</span><span class="sxs-lookup"><span data-stu-id="ee46e-124">string</span></span>  | <span data-ttu-id="ee46e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee46e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee46e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee46e-127">Request body</span></span>

<span data-ttu-id="ee46e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee46e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee46e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee46e-129">Response</span></span>

<span data-ttu-id="ee46e-130">Se tiver êxito, retornará `204 No Content` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ee46e-130">If successful, returns a `204 No Content` response.</span></span> <span data-ttu-id="ee46e-131">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee46e-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee46e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee46e-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee46e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee46e-133">Request</span></span>
<span data-ttu-id="ee46e-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee46e-134">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ee46e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee46e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_pause"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ee46e-136">C#</span><span class="sxs-lookup"><span data-stu-id="ee46e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-pause-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee46e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee46e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-pause-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ee46e-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ee46e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-pause-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee46e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee46e-139">Response</span></span>
<span data-ttu-id="ee46e-140">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ee46e-140">The following is an example of a response.</span></span>
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
  "description": "synchronizationJob: pause",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
