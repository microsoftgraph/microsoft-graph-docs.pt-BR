---
title: Criar synchronizationJob
description: Crie um novo trabalho de sincronização com um esquema de sincronização padrão. O trabalho é criado em um estado desabilitado. Inicie o trabalho de início de chamada para iniciar a sincronização.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 85dcda5bee9941a6fe7885a5ddc8464b680586b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452992"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="c5bb6-105">Criar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="c5bb6-105">Create synchronizationJob</span></span>

<span data-ttu-id="c5bb6-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c5bb6-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5bb6-107">Crie um novo trabalho de sincronização com um esquema de sincronização padrão.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-107">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="c5bb6-108">O trabalho é criado em um estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-108">The job is created in a disabled state.</span></span> <span data-ttu-id="c5bb6-109">[Inicie o trabalho de início](synchronization-synchronizationjob-start.md) de chamada para iniciar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-109">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5bb6-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5bb6-110">Permissions</span></span>
<span data-ttu-id="c5bb6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5bb6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5bb6-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5bb6-113">Permission type</span></span>                        | <span data-ttu-id="c5bb6-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5bb6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5bb6-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5bb6-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="c5bb6-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5bb6-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c5bb6-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5bb6-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c5bb6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-118">Not supported.</span></span>|
|<span data-ttu-id="c5bb6-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5bb6-119">Application</span></span>                            |<span data-ttu-id="c5bb6-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c5bb6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5bb6-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="c5bb6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5bb6-122">Request headers</span></span>

| <span data-ttu-id="c5bb6-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c5bb6-123">Name</span></span>           | <span data-ttu-id="c5bb6-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5bb6-124">Type</span></span>    | <span data-ttu-id="c5bb6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5bb6-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c5bb6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5bb6-126">Authorization</span></span>  | <span data-ttu-id="c5bb6-127">string</span><span class="sxs-lookup"><span data-stu-id="c5bb6-127">string</span></span>  | <span data-ttu-id="c5bb6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5bb6-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5bb6-130">Request body</span></span>

<span data-ttu-id="c5bb6-131">No corpo da solicitação, forneça uma representação JSON do objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-131">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="c5bb6-132">A única propriedade Required é `templateId`.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-132">The only required property is `templateId`.</span></span> <span data-ttu-id="c5bb6-133">A `templateId` propriedade deve corresponder a um dos modelos criados para esta entidade de serviço/aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-133">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="c5bb6-134">Para localizar os modelos disponíveis, use [modelos de lista](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="c5bb6-134">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="c5bb6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5bb6-135">Response</span></span>

<span data-ttu-id="c5bb6-136">Se bem-sucedido, retorna um `201 Created` código de resposta e um objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-136">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5bb6-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5bb6-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c5bb6-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5bb6-138">Request</span></span>
<span data-ttu-id="c5bb6-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5bb6-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5bb6-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c5bb6-141">C#</span><span class="sxs-lookup"><span data-stu-id="c5bb6-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5bb6-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5bb6-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5bb6-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5bb6-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c5bb6-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5bb6-144">Response</span></span>
<span data-ttu-id="c5bb6-145">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-145">The following is an example of a response.</span></span> 

><span data-ttu-id="c5bb6-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5bb6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
