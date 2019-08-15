---
title: Criar synchronizationJob
description: Crie um novo trabalho de sincronização com um esquema de sincronização padrão. O trabalho é criado em um estado desabilitado. Inicie o trabalho de início de chamada para iniciar a sincronização.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9af5006f078e6fc0673ccc69e239a0b904044ac
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409769"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="64b07-105">Criar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="64b07-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64b07-106">Crie um novo trabalho de sincronização com um esquema de sincronização padrão.</span><span class="sxs-lookup"><span data-stu-id="64b07-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="64b07-107">O trabalho é criado em um estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="64b07-107">The job is created in a disabled state.</span></span> <span data-ttu-id="64b07-108">[Inicie o trabalho de início](synchronization-synchronizationjob-start.md) de chamada para iniciar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="64b07-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="64b07-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="64b07-109">Permissions</span></span>
<span data-ttu-id="64b07-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b07-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b07-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64b07-112">Permission type</span></span>                        | <span data-ttu-id="64b07-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64b07-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="64b07-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64b07-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="64b07-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b07-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="64b07-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64b07-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="64b07-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64b07-117">Not supported.</span></span>|
|<span data-ttu-id="64b07-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64b07-118">Application</span></span>                            |<span data-ttu-id="64b07-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64b07-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="64b07-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64b07-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="64b07-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64b07-121">Request headers</span></span>

| <span data-ttu-id="64b07-122">Nome</span><span class="sxs-lookup"><span data-stu-id="64b07-122">Name</span></span>           | <span data-ttu-id="64b07-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="64b07-123">Type</span></span>    | <span data-ttu-id="64b07-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="64b07-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="64b07-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="64b07-125">Authorization</span></span>  | <span data-ttu-id="64b07-126">string</span><span class="sxs-lookup"><span data-stu-id="64b07-126">string</span></span>  | <span data-ttu-id="64b07-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64b07-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64b07-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64b07-129">Request body</span></span>

<span data-ttu-id="64b07-130">No corpo da solicitação, forneça uma representação JSON do objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="64b07-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="64b07-131">A única propriedade Required é `templateId`.</span><span class="sxs-lookup"><span data-stu-id="64b07-131">The only required property is `templateId`.</span></span> <span data-ttu-id="64b07-132">A `templateId` propriedade deve corresponder a um dos modelos criados para esta entidade de serviço/aplicativo.</span><span class="sxs-lookup"><span data-stu-id="64b07-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="64b07-133">Para localizar os modelos disponíveis, use [modelos de lista](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="64b07-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="64b07-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b07-134">Response</span></span>

<span data-ttu-id="64b07-135">Se bem-sucedido, retorna um `201 Created` código de resposta e um objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64b07-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64b07-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64b07-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64b07-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64b07-137">Request</span></span>
<span data-ttu-id="64b07-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="64b07-138">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="64b07-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="64b07-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
Content-type: application/json

{ 
    "templateId": "BoxOutDelta"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64b07-140">C#</span><span class="sxs-lookup"><span data-stu-id="64b07-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64b07-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64b07-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64b07-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="64b07-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64b07-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b07-143">Response</span></span>
<span data-ttu-id="64b07-144">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="64b07-144">The following is an example of a response.</span></span> 

><span data-ttu-id="64b07-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64b07-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
        "code": "NotConfigured",
        "lastExecution": null,
        "lastSuccessfulExecution": null,
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
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
