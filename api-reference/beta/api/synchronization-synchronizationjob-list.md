---
title: Listar trabalhos de sincronização
description: Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 29d4e2747ea37cd8555521e6edba97df7764bed4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074105"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="f3824-103">Listar trabalhos de sincronização</span><span class="sxs-lookup"><span data-stu-id="f3824-103">List synchronization jobs</span></span>

<span data-ttu-id="f3824-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3824-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3824-105">Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="f3824-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="f3824-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3824-106">Permissions</span></span>
<span data-ttu-id="f3824-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3824-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3824-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3824-109">Permission type</span></span>                        | <span data-ttu-id="f3824-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3824-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3824-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3824-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="f3824-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3824-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f3824-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3824-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f3824-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3824-114">Not supported.</span></span> |
|<span data-ttu-id="f3824-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3824-115">Application</span></span>                            |<span data-ttu-id="f3824-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3824-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f3824-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3824-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="f3824-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3824-118">Request headers</span></span>

| <span data-ttu-id="f3824-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f3824-119">Name</span></span>           | <span data-ttu-id="f3824-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3824-120">Type</span></span>    | <span data-ttu-id="f3824-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3824-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f3824-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3824-122">Authorization</span></span>  | <span data-ttu-id="f3824-123">string</span><span class="sxs-lookup"><span data-stu-id="f3824-123">string</span></span>  | <span data-ttu-id="f3824-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3824-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3824-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3824-126">Request body</span></span>

<span data-ttu-id="f3824-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3824-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3824-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3824-128">Response</span></span>

<span data-ttu-id="f3824-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3824-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3824-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3824-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f3824-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3824-131">Request</span></span>
<span data-ttu-id="f3824-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3824-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3824-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3824-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="f3824-134">C#</span><span class="sxs-lookup"><span data-stu-id="f3824-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3824-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3824-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3824-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3824-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f3824-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3824-137">Response</span></span>
<span data-ttu-id="f3824-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f3824-138">The following is an example of a response.</span></span> 

><span data-ttu-id="f3824-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3824-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2958

{
    "value": [
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
                "lastSuccessfulExecutionWithExports": null,
                "steadyStateFirstAchievedTime": "0001-01-01T00:00:00Z",
                "steadyStateLastAchievedTime": "0001-01-01T00:00:00Z",
                "quarantine": null,
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


