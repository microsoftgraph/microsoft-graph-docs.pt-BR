---
title: Obter synchronizationJob
description: Recupere o trabalho de sincronização existentes e suas propriedades.
localization_priority: Normal
ms.openlocfilehash: 5e6be3cc707fdb70b80c6bd2ebe924232aaa674c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850313"
---
# <a name="get-synchronizationjob"></a><span data-ttu-id="25445-103">Obter synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="25445-103">Get synchronizationJob</span></span>

> <span data-ttu-id="25445-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="25445-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25445-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="25445-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25445-106">Recupere o trabalho de sincronização existentes e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="25445-106">Retrieve the existing synchronization job and its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="25445-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="25445-107">Permissions</span></span>
<span data-ttu-id="25445-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25445-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25445-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25445-110">Permission type</span></span>                        | <span data-ttu-id="25445-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25445-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="25445-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25445-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="25445-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25445-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="25445-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25445-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="25445-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25445-115">Not supported.</span></span>  |
|<span data-ttu-id="25445-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25445-116">Application</span></span>                            |<span data-ttu-id="25445-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25445-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="25445-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25445-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

## <a name="request-headers"></a><span data-ttu-id="25445-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25445-119">Request headers</span></span>

| <span data-ttu-id="25445-120">Nome</span><span class="sxs-lookup"><span data-stu-id="25445-120">Name</span></span>           | <span data-ttu-id="25445-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="25445-121">Type</span></span>    | <span data-ttu-id="25445-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="25445-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="25445-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="25445-123">Authorization</span></span>  | <span data-ttu-id="25445-124">string</span><span class="sxs-lookup"><span data-stu-id="25445-124">string</span></span>  | <span data-ttu-id="25445-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25445-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25445-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25445-127">Request body</span></span>

<span data-ttu-id="25445-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25445-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25445-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="25445-129">Response</span></span>

<span data-ttu-id="25445-130">Se tiver êxito, retorna um `200 OK` resposta com um [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25445-130">If successful, returns a `200 OK` response with a [synchronizationJob](../resources/synchronization-synchronizationjob.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25445-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25445-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25445-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25445-132">Request</span></span>
<span data-ttu-id="25445-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="25445-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationjob"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/
```

##### <a name="response"></a><span data-ttu-id="25445-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="25445-134">Response</span></span>
<span data-ttu-id="25445-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="25445-135">The following is an example of a response.</span></span> 

><span data-ttu-id="25445-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25445-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
