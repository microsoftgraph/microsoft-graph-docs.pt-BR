---
title: Criar synchronizationJob
description: Crie um novo trabalho de sincronização com um esquema de sincronização padrão. O trabalho é criado em um estado desabilitado. Chame o trabalho de início para iniciar a sincronização.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a565a393715edb2379590b225e0569f4397b9b23
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131646"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="ff828-105">Criar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="ff828-105">Create synchronizationJob</span></span>

<span data-ttu-id="ff828-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff828-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff828-107">Crie um novo trabalho de sincronização com um esquema de sincronização padrão.</span><span class="sxs-lookup"><span data-stu-id="ff828-107">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="ff828-108">O trabalho é criado em um estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="ff828-108">The job is created in a disabled state.</span></span> <span data-ttu-id="ff828-109">Chame [o trabalho de início](synchronization-synchronizationjob-start.md) para iniciar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="ff828-109">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff828-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff828-110">Permissions</span></span>
<span data-ttu-id="ff828-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff828-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff828-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff828-113">Permission type</span></span>                        | <span data-ttu-id="ff828-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff828-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff828-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff828-115">Delegated (work or school account)</span></span>     |<span data-ttu-id="ff828-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff828-116">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ff828-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff828-117">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ff828-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff828-118">Not supported.</span></span>|
|<span data-ttu-id="ff828-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff828-119">Application</span></span>                            |<span data-ttu-id="ff828-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff828-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ff828-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff828-121">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="ff828-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff828-122">Request headers</span></span>

| <span data-ttu-id="ff828-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ff828-123">Name</span></span>           | <span data-ttu-id="ff828-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff828-124">Type</span></span>    | <span data-ttu-id="ff828-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff828-125">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ff828-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff828-126">Authorization</span></span>  | <span data-ttu-id="ff828-127">string</span><span class="sxs-lookup"><span data-stu-id="ff828-127">string</span></span>  | <span data-ttu-id="ff828-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff828-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff828-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff828-130">Request body</span></span>

<span data-ttu-id="ff828-131">No corpo da solicitação, fornece uma representação JSON do [objeto synchronizationJob](../resources/synchronization-synchronizationjob.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="ff828-131">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="ff828-132">A única propriedade necessária é `templateId` .</span><span class="sxs-lookup"><span data-stu-id="ff828-132">The only required property is `templateId`.</span></span> <span data-ttu-id="ff828-133">A `templateId` propriedade deve corresponder a um dos modelos criados para este aplicativo/entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="ff828-133">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="ff828-134">Para encontrar modelos disponíveis, use [modelos de lista.](synchronization-synchronizationtemplate-list.md)</span><span class="sxs-lookup"><span data-stu-id="ff828-134">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="ff828-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff828-135">Response</span></span>

<span data-ttu-id="ff828-136">Se bem-sucedido, retorna `201 Created` um código de resposta e um objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff828-136">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff828-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff828-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ff828-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff828-138">Request</span></span>
<span data-ttu-id="ff828-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff828-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff828-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff828-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ff828-141">C#</span><span class="sxs-lookup"><span data-stu-id="ff828-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationjob-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff828-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff828-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationjob-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff828-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff828-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationjob-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff828-144">Java</span><span class="sxs-lookup"><span data-stu-id="ff828-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationjob-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff828-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff828-145">Response</span></span>
<span data-ttu-id="ff828-146">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ff828-146">The following is an example of a response.</span></span> 

><span data-ttu-id="ff828-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff828-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


