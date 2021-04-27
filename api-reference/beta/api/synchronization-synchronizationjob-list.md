---
title: Listar trabalhos de sincronização
description: Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c236b4bbd7afff7065932537c534aeb2d69dd57e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054823"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="23e2d-103">Listar trabalhos de sincronização</span><span class="sxs-lookup"><span data-stu-id="23e2d-103">List synchronization jobs</span></span>

<span data-ttu-id="23e2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23e2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23e2d-105">Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="23e2d-105">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="23e2d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="23e2d-106">Permissions</span></span>
<span data-ttu-id="23e2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23e2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23e2d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23e2d-109">Permission type</span></span>                        | <span data-ttu-id="23e2d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23e2d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="23e2d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23e2d-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="23e2d-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e2d-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="23e2d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23e2d-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="23e2d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23e2d-114">Not supported.</span></span> |
|<span data-ttu-id="23e2d-115">Application</span><span class="sxs-lookup"><span data-stu-id="23e2d-115">Application</span></span>                            |<span data-ttu-id="23e2d-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e2d-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="23e2d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23e2d-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="23e2d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23e2d-118">Request headers</span></span>

| <span data-ttu-id="23e2d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="23e2d-119">Name</span></span>           | <span data-ttu-id="23e2d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="23e2d-120">Type</span></span>    | <span data-ttu-id="23e2d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="23e2d-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="23e2d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23e2d-122">Authorization</span></span>  | <span data-ttu-id="23e2d-123">string</span><span class="sxs-lookup"><span data-stu-id="23e2d-123">string</span></span>  | <span data-ttu-id="23e2d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23e2d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23e2d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23e2d-126">Request body</span></span>

<span data-ttu-id="23e2d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23e2d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23e2d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="23e2d-128">Response</span></span>

<span data-ttu-id="23e2d-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23e2d-129">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23e2d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23e2d-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="23e2d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23e2d-131">Request</span></span>
<span data-ttu-id="23e2d-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="23e2d-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23e2d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="23e2d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="c"></a>[<span data-ttu-id="23e2d-134">C#</span><span class="sxs-lookup"><span data-stu-id="23e2d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23e2d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23e2d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23e2d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23e2d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23e2d-137">Java</span><span class="sxs-lookup"><span data-stu-id="23e2d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23e2d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="23e2d-138">Response</span></span>
<span data-ttu-id="23e2d-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="23e2d-139">The following is an example of a response.</span></span> 

><span data-ttu-id="23e2d-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="23e2d-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


