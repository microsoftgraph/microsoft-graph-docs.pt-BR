---
title: Obter synchronizationJob
description: Recupere o trabalho de sincronização existente e suas propriedades.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b7f08a5af94c2d03e21230430d58952fa81cc6bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453011"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="afaeb-103">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="afaeb-103">Get synchronizationJob</span></span>

<span data-ttu-id="afaeb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="afaeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afaeb-105">Recupere o trabalho de sincronização existente e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="afaeb-105">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="afaeb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="afaeb-106">Permissions</span></span>
<span data-ttu-id="afaeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afaeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afaeb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afaeb-109">Permission type</span></span>                        | <span data-ttu-id="afaeb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="afaeb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="afaeb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afaeb-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="afaeb-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afaeb-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="afaeb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afaeb-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="afaeb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afaeb-114">Not supported.</span></span>  |
|<span data-ttu-id="afaeb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afaeb-115">Application</span></span>                            |<span data-ttu-id="afaeb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afaeb-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="afaeb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afaeb-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="afaeb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afaeb-118">Request headers</span></span>

| <span data-ttu-id="afaeb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="afaeb-119">Name</span></span>           | <span data-ttu-id="afaeb-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="afaeb-120">Type</span></span>    | <span data-ttu-id="afaeb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="afaeb-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="afaeb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="afaeb-122">Authorization</span></span>  | <span data-ttu-id="afaeb-123">string</span><span class="sxs-lookup"><span data-stu-id="afaeb-123">string</span></span>  | <span data-ttu-id="afaeb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afaeb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afaeb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afaeb-126">Request body</span></span>

<span data-ttu-id="afaeb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="afaeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afaeb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="afaeb-128">Response</span></span>

<span data-ttu-id="afaeb-129">Se tiver êxito, retornará `200 OK` uma resposta com um [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afaeb-129">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afaeb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afaeb-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="afaeb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afaeb-131">Request</span></span>
<span data-ttu-id="afaeb-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="afaeb-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="afaeb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="afaeb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="afaeb-134">C#</span><span class="sxs-lookup"><span data-stu-id="afaeb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afaeb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afaeb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afaeb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afaeb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="afaeb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="afaeb-137">Response</span></span>
<span data-ttu-id="afaeb-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="afaeb-138">The following is an example of a response.</span></span> 

><span data-ttu-id="afaeb-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afaeb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "quarantine": {
            "currentBegan": "",
            "nextAttempt": "",
            "reason": "",
            "seriesBegan": "",
            "seriesCount": 2,
            "error": {
                "code": "SalesforceInvalidCredentials",
                "message": "Your Salesforce.com credentials are invalid.  Please obtain a current Salesforce.com administrative user name, password and security token, and enter those in the screen for configuring user provisioning",
                "tenantActionable": true
            }
        },
        "troubleshootingUrl": null
    },
    "synchronizationJobSettings": [
      {
          "name": "QuarantineTooManyDeletesThreshold",
          "value": "500"
      }
    ]
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
