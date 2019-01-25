---
title: Trabalhos de sincronização de lista
description: Lista os trabalhos existentes para uma instância de determinado aplicativo (entidade de serviço).
localization_priority: Normal
ms.openlocfilehash: 265b1f5a32239173154ef51077d59f3104ad03b3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518958"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="f9f79-103">Trabalhos de sincronização de lista</span><span class="sxs-lookup"><span data-stu-id="f9f79-103">List synchronization jobs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9f79-104">Lista os trabalhos existentes para uma instância de determinado aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="f9f79-104">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9f79-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9f79-105">Permissions</span></span>
<span data-ttu-id="f9f79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9f79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9f79-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9f79-108">Permission type</span></span>                        | <span data-ttu-id="f9f79-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9f79-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9f79-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9f79-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="f9f79-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f79-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f9f79-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9f79-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f9f79-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f79-113">Not supported.</span></span> |
|<span data-ttu-id="f9f79-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9f79-114">Application</span></span>                            |<span data-ttu-id="f9f79-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9f79-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f9f79-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9f79-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="f9f79-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f79-117">Request headers</span></span>

| <span data-ttu-id="f9f79-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f9f79-118">Name</span></span>           | <span data-ttu-id="f9f79-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9f79-119">Type</span></span>    | <span data-ttu-id="f9f79-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9f79-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f9f79-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9f79-121">Authorization</span></span>  | <span data-ttu-id="f9f79-122">string</span><span class="sxs-lookup"><span data-stu-id="f9f79-122">string</span></span>  | <span data-ttu-id="f9f79-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9f79-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9f79-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f79-125">Request body</span></span>

<span data-ttu-id="f9f79-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9f79-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9f79-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f79-127">Response</span></span>

<span data-ttu-id="f9f79-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f79-128">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9f79-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9f79-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f9f79-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9f79-130">Request</span></span>
<span data-ttu-id="f9f79-131">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9f79-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="f9f79-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9f79-132">Response</span></span>
<span data-ttu-id="f9f79-133">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f9f79-133">The following is an example of a response.</span></span> 

><span data-ttu-id="f9f79-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9f79-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
