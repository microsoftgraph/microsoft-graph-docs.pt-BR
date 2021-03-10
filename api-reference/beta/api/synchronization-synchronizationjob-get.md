---
title: Obter synchronizationJob
description: Recupere o trabalho de sincronização existente e suas propriedades.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 64d5b801b7529b94cbc6a02bf20315cf4374eff4
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625980"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="ec779-103">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="ec779-103">Get synchronizationJob</span></span>

<span data-ttu-id="ec779-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec779-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec779-105">Recupere o trabalho de sincronização existente e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ec779-105">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec779-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec779-106">Permissions</span></span>
<span data-ttu-id="ec779-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec779-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec779-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec779-109">Permission type</span></span>                        | <span data-ttu-id="ec779-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec779-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec779-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec779-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="ec779-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec779-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="ec779-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec779-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ec779-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec779-114">Not supported.</span></span>  |
|<span data-ttu-id="ec779-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec779-115">Application</span></span>                            |<span data-ttu-id="ec779-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec779-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ec779-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec779-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="ec779-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec779-118">Request headers</span></span>

| <span data-ttu-id="ec779-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ec779-119">Name</span></span>           | <span data-ttu-id="ec779-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec779-120">Type</span></span>    | <span data-ttu-id="ec779-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec779-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ec779-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec779-122">Authorization</span></span>  | <span data-ttu-id="ec779-123">string</span><span class="sxs-lookup"><span data-stu-id="ec779-123">string</span></span>  | <span data-ttu-id="ec779-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec779-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec779-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec779-126">Request body</span></span>

<span data-ttu-id="ec779-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec779-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec779-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec779-128">Response</span></span>

<span data-ttu-id="ec779-129">Se tiver êxito, retornará `200 OK` uma resposta com uma [sincronizaçãoJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec779-129">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec779-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec779-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ec779-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec779-131">Request</span></span>
<span data-ttu-id="ec779-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec779-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec779-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec779-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```
# <a name="c"></a>[<span data-ttu-id="ec779-134">C#</span><span class="sxs-lookup"><span data-stu-id="ec779-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec779-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec779-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec779-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec779-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec779-137">Java</span><span class="sxs-lookup"><span data-stu-id="ec779-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ec779-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec779-138">Response</span></span>
<span data-ttu-id="ec779-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ec779-139">The following is an example of a response.</span></span> 

><span data-ttu-id="ec779-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec779-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


