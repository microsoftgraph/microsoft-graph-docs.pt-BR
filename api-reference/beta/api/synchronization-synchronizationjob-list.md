---
title: Trabalhos de sincronização de lista
description: Lista os trabalhos existentes para uma instância de determinado aplicativo (entidade de serviço).
localization_priority: Normal
ms.openlocfilehash: daf486ed8da41be2e13be622bc18b81711de3ff7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846953"
---
# <a name="list-synchronization-jobs"></a><span data-ttu-id="2f620-103">Trabalhos de sincronização de lista</span><span class="sxs-lookup"><span data-stu-id="2f620-103">List synchronization jobs</span></span>

> <span data-ttu-id="2f620-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2f620-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f620-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2f620-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f620-106">Lista os trabalhos existentes para uma instância de determinado aplicativo (entidade de serviço).</span><span class="sxs-lookup"><span data-stu-id="2f620-106">List existing jobs for a given application instance (service principal).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f620-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="2f620-107">Permissions</span></span>
<span data-ttu-id="2f620-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f620-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f620-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f620-110">Permission type</span></span>                        | <span data-ttu-id="2f620-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f620-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f620-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f620-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="2f620-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f620-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2f620-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f620-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2f620-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f620-115">Not supported.</span></span> |
|<span data-ttu-id="2f620-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f620-116">Application</span></span>                            |<span data-ttu-id="2f620-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f620-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f620-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f620-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="2f620-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f620-119">Request headers</span></span>

| <span data-ttu-id="2f620-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2f620-120">Name</span></span>           | <span data-ttu-id="2f620-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f620-121">Type</span></span>    | <span data-ttu-id="2f620-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f620-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2f620-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f620-123">Authorization</span></span>  | <span data-ttu-id="2f620-124">string</span><span class="sxs-lookup"><span data-stu-id="2f620-124">string</span></span>  | <span data-ttu-id="2f620-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f620-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f620-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f620-127">Request body</span></span>

<span data-ttu-id="2f620-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2f620-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f620-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f620-129">Response</span></span>

<span data-ttu-id="2f620-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f620-130">If successful, this method returns a `200 OK` response code and a collection of [synchronizationJob](../resources/synchronization-synchronizationjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f620-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f620-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2f620-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f620-132">Request</span></span>
<span data-ttu-id="2f620-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f620-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/
```

##### <a name="response"></a><span data-ttu-id="2f620-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f620-134">Response</span></span>
<span data-ttu-id="2f620-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="2f620-135">The following is an example of a response.</span></span> 

><span data-ttu-id="2f620-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f620-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
