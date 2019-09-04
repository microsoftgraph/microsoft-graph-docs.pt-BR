---
title: Listar trabalhos de sincronização
description: Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: adf545d4be30810f82bf0a8ed0ecb5b7a2adfa5b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724467"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="6958c-103">Listar trabalhos de sincronização</span><span class="sxs-lookup"><span data-stu-id="6958c-103">List synchronization jobs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6958c-104">Listar trabalhos existentes para uma determinada instância de aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="6958c-104">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="6958c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6958c-105">Permissions</span></span>
<span data-ttu-id="6958c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6958c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6958c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6958c-108">Permission type</span></span>                        | <span data-ttu-id="6958c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6958c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6958c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6958c-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="6958c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6958c-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="6958c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6958c-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="6958c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6958c-113">Not supported.</span></span> |
|<span data-ttu-id="6958c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6958c-114">Application</span></span>                            |<span data-ttu-id="6958c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6958c-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6958c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6958c-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="6958c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6958c-117">Request headers</span></span>

| <span data-ttu-id="6958c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6958c-118">Name</span></span>           | <span data-ttu-id="6958c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6958c-119">Type</span></span>    | <span data-ttu-id="6958c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6958c-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6958c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6958c-121">Authorization</span></span>  | <span data-ttu-id="6958c-122">string</span><span class="sxs-lookup"><span data-stu-id="6958c-122">string</span></span>  | <span data-ttu-id="6958c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6958c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6958c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6958c-125">Request body</span></span>

<span data-ttu-id="6958c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6958c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6958c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6958c-127">Response</span></span>

<span data-ttu-id="6958c-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6958c-128">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6958c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6958c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6958c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6958c-130">Request</span></span>
<span data-ttu-id="6958c-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6958c-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6958c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6958c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6958c-133">C#</span><span class="sxs-lookup"><span data-stu-id="6958c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6958c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6958c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6958c-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6958c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6958c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6958c-136">Response</span></span>
<span data-ttu-id="6958c-137">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="6958c-137">The following is an example of a response.</span></span> 

><span data-ttu-id="6958c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6958c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
