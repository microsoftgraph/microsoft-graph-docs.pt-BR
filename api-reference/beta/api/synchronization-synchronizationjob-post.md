---
title: Criar synchronizationJob
description: Crie novo trabalho de sincronização com um esquema de sincronização padrão. O trabalho é criado em um estado desabilitado. Trabalho de início de chamada para iniciar a sincronização.
ms.openlocfilehash: 3c7e3c3a9c89f95b031cd45d38848e0f2f451de7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040268"
---
# <a name="create-synchronizationjob"></a><span data-ttu-id="f00a3-105">Criar synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="f00a3-105">Create synchronizationJob</span></span>

> <span data-ttu-id="f00a3-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f00a3-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f00a3-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f00a3-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f00a3-108">Crie novo trabalho de sincronização com um esquema de sincronização padrão.</span><span class="sxs-lookup"><span data-stu-id="f00a3-108">Create new synchronization job with a default synchronization schema.</span></span> <span data-ttu-id="f00a3-109">O trabalho é criado em um estado desabilitado.</span><span class="sxs-lookup"><span data-stu-id="f00a3-109">The job is created in a disabled state.</span></span> <span data-ttu-id="f00a3-110">Chame [Iniciar trabalho](synchronization-synchronizationjob-start.md) para iniciar a sincronização.</span><span class="sxs-lookup"><span data-stu-id="f00a3-110">Call [Start job](synchronization-synchronizationjob-start.md) to start synchronization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f00a3-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="f00a3-111">Permissions</span></span>
<span data-ttu-id="f00a3-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f00a3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f00a3-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f00a3-114">Permission type</span></span>                        | <span data-ttu-id="f00a3-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f00a3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f00a3-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f00a3-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="f00a3-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f00a3-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f00a3-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f00a3-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f00a3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f00a3-119">Not supported.</span></span>|
|<span data-ttu-id="f00a3-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f00a3-120">Application</span></span>                            |<span data-ttu-id="f00a3-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f00a3-121">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f00a3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f00a3-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/
```

## <a name="request-headers"></a><span data-ttu-id="f00a3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f00a3-123">Request headers</span></span>

| <span data-ttu-id="f00a3-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f00a3-124">Name</span></span>           | <span data-ttu-id="f00a3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="f00a3-125">Type</span></span>    | <span data-ttu-id="f00a3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f00a3-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f00a3-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f00a3-127">Authorization</span></span>  | <span data-ttu-id="f00a3-128">string</span><span class="sxs-lookup"><span data-stu-id="f00a3-128">string</span></span>  | <span data-ttu-id="f00a3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f00a3-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f00a3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f00a3-131">Request body</span></span>

<span data-ttu-id="f00a3-132">No corpo da solicitação, fornece uma representação JSON do objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="f00a3-132">In the request body, supply a JSON representation of the [synchronizationJob](../resources/synchronization-synchronizationjob.md) object to be created.</span></span> <span data-ttu-id="f00a3-133">É a única propriedade exigida `templateId`.</span><span class="sxs-lookup"><span data-stu-id="f00a3-133">The only required property is `templateId`.</span></span> <span data-ttu-id="f00a3-134">O `templateId` propriedade deve corresponder a um dos modelos criados para essa entidade de serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f00a3-134">The `templateId` property must match one of the templates created for this application/service principal.</span></span> <span data-ttu-id="f00a3-135">Para localizar os modelos disponíveis, use os [modelos de lista](synchronization-synchronizationtemplate-list.md).</span><span class="sxs-lookup"><span data-stu-id="f00a3-135">To find available templates, use [List templates](synchronization-synchronizationtemplate-list.md).</span></span>

## <a name="response"></a><span data-ttu-id="f00a3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f00a3-136">Response</span></span>

<span data-ttu-id="f00a3-137">Se tiver êxito, retorna um `201 Created` código de resposta e um objeto [synchronizationJob](../resources/synchronization-synchronizationjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f00a3-137">If successful, returns a `201 Created` response code and a [synchronizationJob](../resources/synchronization-synchronizationjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f00a3-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f00a3-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f00a3-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f00a3-139">Request</span></span>
<span data-ttu-id="f00a3-140">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f00a3-140">The following is an example of a request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f00a3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f00a3-141">Response</span></span>
<span data-ttu-id="f00a3-142">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f00a3-142">The following is an example of a response.</span></span> 

><span data-ttu-id="f00a3-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f00a3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->