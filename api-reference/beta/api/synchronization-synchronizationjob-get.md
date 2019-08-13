---
title: Obter synchronizationJob
description: Recupere o trabalho de sincronização existente e suas propriedades.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 72411858f8faee96b1bdd89e8da6e170d6d16b41
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363561"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="cd81f-103">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="cd81f-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd81f-104">Recupere o trabalho de sincronização existente e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cd81f-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd81f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd81f-105">Permissions</span></span>
<span data-ttu-id="cd81f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd81f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd81f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd81f-108">Permission type</span></span>                        | <span data-ttu-id="cd81f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd81f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd81f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd81f-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="cd81f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd81f-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="cd81f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd81f-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="cd81f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd81f-113">Not supported.</span></span>  |
|<span data-ttu-id="cd81f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd81f-114">Application</span></span>                            |<span data-ttu-id="cd81f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd81f-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cd81f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd81f-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="cd81f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd81f-117">Request headers</span></span>

| <span data-ttu-id="cd81f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cd81f-118">Name</span></span>           | <span data-ttu-id="cd81f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd81f-119">Type</span></span>    | <span data-ttu-id="cd81f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd81f-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="cd81f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd81f-121">Authorization</span></span>  | <span data-ttu-id="cd81f-122">string</span><span class="sxs-lookup"><span data-stu-id="cd81f-122">string</span></span>  | <span data-ttu-id="cd81f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd81f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd81f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd81f-125">Request body</span></span>

<span data-ttu-id="cd81f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd81f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd81f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd81f-127">Response</span></span>

<span data-ttu-id="cd81f-128">Se tiver êxito, retornará `200 OK` uma resposta com um [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd81f-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd81f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd81f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cd81f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd81f-130">Request</span></span>
<span data-ttu-id="cd81f-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd81f-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cd81f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd81f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cd81f-133">C#</span><span class="sxs-lookup"><span data-stu-id="cd81f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd81f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd81f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cd81f-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="cd81f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cd81f-136">Java</span><span class="sxs-lookup"><span data-stu-id="cd81f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cd81f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd81f-137">Response</span></span>
<span data-ttu-id="cd81f-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="cd81f-138">The following is an example of a response.</span></span> 

><span data-ttu-id="cd81f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd81f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2577

{
    "id": "{jobId}",
    "templateId": "BoxOutDelta",
    "schedule": {
        "expiration": null,
        "interval": "P10675199DT2H48M5.4775807S",
        "state": "Disabled"
    },
    "status": {
        "countSuccessiveCompleteFailures": 0,
        "escrowsPruned": false,
        "synchronizedEntryCountByType": [],
        "code": "Paused",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
        "progress": [],
        "lastSuccessfulExecutionWithExports": null,
        "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
        "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
        "quarantine": null,
        "troubleshootingUrl": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
