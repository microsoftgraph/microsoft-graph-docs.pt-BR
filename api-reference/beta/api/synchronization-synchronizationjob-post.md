---
title: Criar synchronizationJob
description: Crie um novo trabalho de sincronização com um esquema de sincronização padrão. O trabalho é criado em um estado desabilitado. Inicie o trabalho de início de chamada para iniciar a sincronização.
localization_priority: Normal
ms.openlocfilehash: fa0c3e539d73ff9496a0d4d0e3af8ebeda75e839
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638029"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="eb189-105">Criar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="eb189-105">Create synchronizationJob</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb189-106">Crie um novo trabalho de sincronização com um esquema de sincronização padrão.</span><span class="sxs-lookup"><span data-stu-id="eb189-106">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="eb189-107">O trabalho é criado em um estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="eb189-107">The job is created in a disabled state.</span></span> <span data-ttu-id="eb189-108">[Inicie o trabalho de início](synchronization-synchronizationjob-start.md) de chamada para iniciar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="eb189-108">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb189-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb189-109">Permissions</span></span>
<span data-ttu-id="eb189-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb189-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb189-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb189-112">Permission type</span></span>                        | <span data-ttu-id="eb189-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb189-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb189-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb189-114">Delegated (work or school account)</span></span>     |<span data-ttu-id="eb189-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb189-115">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="eb189-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb189-116">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="eb189-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb189-117">Not supported.</span></span>|
|<span data-ttu-id="eb189-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb189-118">Application</span></span>                            |<span data-ttu-id="eb189-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb189-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="eb189-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb189-120">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="eb189-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb189-121">Request headers</span></span>

| <span data-ttu-id="eb189-122">Nome</span><span class="sxs-lookup"><span data-stu-id="eb189-122">Name</span></span>           | <span data-ttu-id="eb189-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb189-123">Type</span></span>    | <span data-ttu-id="eb189-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb189-124">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="eb189-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb189-125">Authorization</span></span>  | <span data-ttu-id="eb189-126">string</span><span class="sxs-lookup"><span data-stu-id="eb189-126">string</span></span>  | <span data-ttu-id="eb189-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb189-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb189-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb189-129">Request body</span></span>

<span data-ttu-id="eb189-130">No corpo da solicitação, forneça uma representação JSON do objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="eb189-130">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="eb189-131">A única propriedade Required é `templateId`.</span><span class="sxs-lookup"><span data-stu-id="eb189-131">The only required property is `templateId`.</span></span> <span data-ttu-id="eb189-132">A `templateId` propriedade deve corresponder a um dos modelos criados para esta entidade de serviço/aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eb189-132">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="eb189-133">Para localizar os modelos disponíveis, use [modelos de lista](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="eb189-133">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="eb189-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb189-134">Response</span></span>

<span data-ttu-id="eb189-135">Se bem-sucedido, retorna um `201 Created` código de resposta e um objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb189-135">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb189-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb189-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb189-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb189-137">Request</span></span>
<span data-ttu-id="eb189-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb189-138">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eb189-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb189-139">Response</span></span>
<span data-ttu-id="eb189-140">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="eb189-140">The following is an example of a response.</span></span> 

><span data-ttu-id="eb189-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb189-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="eb189-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb189-142">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb189-143">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="eb189-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb189-144">Basic</span><span class="sxs-lookup"><span data-stu-id="eb189-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb189-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb189-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_synchronizationjob_from_synchronization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
