---
title: tipo de recurso teamsAsyncOperation
description: 'Uma operação assíncrona do Microsoft Teams transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c11527f5a05018f02b4f3113ffa52e10e8929cfd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078966"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="eb09c-103">tipo de recurso teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="eb09c-103">teamsAsyncOperation resource type</span></span>

<span data-ttu-id="eb09c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb09c-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="eb09c-105">Uma operação assíncrona do Microsoft Teams é uma operação que transcende o tempo de vida de uma única solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="eb09c-105">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="eb09c-106">Essas operações são de longa duração ou muito caras para concluir dentro do prazo de sua solicitação de origem.</span><span class="sxs-lookup"><span data-stu-id="eb09c-106">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="eb09c-107">Quando uma operação assíncrona é iniciada, o método retorna um código de resposta aceito 202.</span><span class="sxs-lookup"><span data-stu-id="eb09c-107">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="eb09c-108">A resposta também conterá um cabeçalho de local, que contém o local do teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="eb09c-108">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="eb09c-109">Verifique periodicamente o status da operação fazendo uma solicitação GET para este local; Aguarde >30 segundos entre as verificações.</span><span class="sxs-lookup"><span data-stu-id="eb09c-109">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="eb09c-110">Quando a solicitação for concluída com êxito, o status será "bem-sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.</span><span class="sxs-lookup"><span data-stu-id="eb09c-110">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="eb09c-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb09c-111">Properties</span></span>

| <span data-ttu-id="eb09c-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb09c-112">Property</span></span> | <span data-ttu-id="eb09c-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb09c-113">Type</span></span>   | <span data-ttu-id="eb09c-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb09c-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="eb09c-115">id</span><span class="sxs-lookup"><span data-stu-id="eb09c-115">id</span></span>|<span data-ttu-id="eb09c-116">string</span><span class="sxs-lookup"><span data-stu-id="eb09c-116">string</span></span> |<span data-ttu-id="eb09c-117">ID de operação exclusiva.</span><span class="sxs-lookup"><span data-stu-id="eb09c-117">Unique operation id.</span></span>|
|<span data-ttu-id="eb09c-118">OperationType</span><span class="sxs-lookup"><span data-stu-id="eb09c-118">operationType</span></span>|[<span data-ttu-id="eb09c-119">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="eb09c-119">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="eb09c-120">Indica o tipo de operação que está sendo descrito.</span><span class="sxs-lookup"><span data-stu-id="eb09c-120">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="eb09c-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb09c-121">createdDateTime</span></span>|<span data-ttu-id="eb09c-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb09c-122">DateTimeOffset</span></span> |<span data-ttu-id="eb09c-123">Hora em que a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="eb09c-123">Time when the operation was created.</span></span>|
|<span data-ttu-id="eb09c-124">status</span><span class="sxs-lookup"><span data-stu-id="eb09c-124">status</span></span>|[<span data-ttu-id="eb09c-125">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="eb09c-125">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="eb09c-126">Status da operação.</span><span class="sxs-lookup"><span data-stu-id="eb09c-126">Operation status.</span></span>|
|<span data-ttu-id="eb09c-127">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="eb09c-127">lastActionDateTime</span></span>|<span data-ttu-id="eb09c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb09c-128">DateTimeOffset</span></span> |<span data-ttu-id="eb09c-129">Hora em que a operação assíncrona foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="eb09c-129">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="eb09c-130">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="eb09c-130">attemptsCount</span></span>|<span data-ttu-id="eb09c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="eb09c-131">Int32</span></span>|<span data-ttu-id="eb09c-132">Número de vezes em que a operação foi tentada antes de ser marcada com êxito ou falhou.</span><span class="sxs-lookup"><span data-stu-id="eb09c-132">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="eb09c-133">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="eb09c-133">targetResourceId</span></span>|<span data-ttu-id="eb09c-134">#c0</span><span class="sxs-lookup"><span data-stu-id="eb09c-134">guid</span></span> |<span data-ttu-id="eb09c-135">A ID do objeto que é criado ou modificado como resultado dessa operação assíncrona, normalmente uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="eb09c-135">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="eb09c-136">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="eb09c-136">targetResourceLocation</span></span>|<span data-ttu-id="eb09c-137">string</span><span class="sxs-lookup"><span data-stu-id="eb09c-137">string</span></span>|<span data-ttu-id="eb09c-138">O local do objeto que é criado ou modificado como resultado dessa operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="eb09c-138">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="eb09c-139">Essa URL deve ser tratada como um valor opaco e não analisada em seus caminhos de componente.</span><span class="sxs-lookup"><span data-stu-id="eb09c-139">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="eb09c-140">erro</span><span class="sxs-lookup"><span data-stu-id="eb09c-140">error</span></span>|[<span data-ttu-id="eb09c-141">operationError</span><span class="sxs-lookup"><span data-stu-id="eb09c-141">operationError</span></span>](operationerror.md)|<span data-ttu-id="eb09c-142">Qualquer erro que causa falha na operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="eb09c-142">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb09c-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb09c-143">JSON representation</span></span>

<span data-ttu-id="eb09c-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb09c-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

