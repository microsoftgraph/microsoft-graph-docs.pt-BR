---
title: Obter synchronizationJob
description: Recupere o trabalho de sincronização existente e suas propriedades.
localization_priority: Normal
ms.openlocfilehash: 967f151890fa9f7787e2f05246d9bacc445738d9
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638050"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="093cf-103">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="093cf-103">Get synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="093cf-104">Recupere o trabalho de sincronização existente e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="093cf-104">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="093cf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="093cf-105">Permissions</span></span>
<span data-ttu-id="093cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="093cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="093cf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="093cf-108">Permission type</span></span>                        | <span data-ttu-id="093cf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="093cf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="093cf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="093cf-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="093cf-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="093cf-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="093cf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="093cf-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="093cf-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="093cf-113">Not supported.</span></span>  |
|<span data-ttu-id="093cf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="093cf-114">Application</span></span>                            |<span data-ttu-id="093cf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="093cf-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="093cf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="093cf-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="093cf-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="093cf-117">Request headers</span></span>

| <span data-ttu-id="093cf-118">Nome</span><span class="sxs-lookup"><span data-stu-id="093cf-118">Name</span></span>           | <span data-ttu-id="093cf-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="093cf-119">Type</span></span>    | <span data-ttu-id="093cf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="093cf-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="093cf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="093cf-121">Authorization</span></span>  | <span data-ttu-id="093cf-122">string</span><span class="sxs-lookup"><span data-stu-id="093cf-122">string</span></span>  | <span data-ttu-id="093cf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="093cf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="093cf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="093cf-125">Request body</span></span>

<span data-ttu-id="093cf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="093cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="093cf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="093cf-127">Response</span></span>

<span data-ttu-id="093cf-128">Se tiver êxito, retornará `200 OK` uma resposta com um [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="093cf-128">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="093cf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="093cf-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="093cf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="093cf-130">Request</span></span>
<span data-ttu-id="093cf-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="093cf-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="093cf-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="093cf-132">Response</span></span>
<span data-ttu-id="093cf-133">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="093cf-133">The following is an example of a response.</span></span> 

><span data-ttu-id="093cf-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="093cf-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="093cf-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="093cf-135">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="093cf-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="093cf-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="093cf-137">Basic</span><span class="sxs-lookup"><span data-stu-id="093cf-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationjob-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="093cf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="093cf-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationjob-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
