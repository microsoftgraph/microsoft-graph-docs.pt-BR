---
title: tipo de recurso de teamsAsyncOperation
description: 'Uma operação assíncrona de Teams da Microsoft é uma operação que transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 20a616d3c09337b96c50cc008e4f56021c61e593
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885572"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="13577-103">tipo de recurso de teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="13577-103">teamsAsyncOperation resource type</span></span>

> <span data-ttu-id="13577-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="13577-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13577-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13577-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13577-106">Uma operação assíncrona de Teams da Microsoft é uma operação que transcende o tempo de vida de uma única solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="13577-106">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="13577-107">Essas operações são muito caro concluir dentro do período de tempo de sua solicitação de origem ou de longa execução.</span><span class="sxs-lookup"><span data-stu-id="13577-107">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="13577-108">Quando é iniciada uma operação assíncrona, o método retornará um código de resposta 202 aceitos.</span><span class="sxs-lookup"><span data-stu-id="13577-108">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="13577-109">A resposta conterá também um cabeçalho de local, que contém a localização do teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="13577-109">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="13577-110">Verificar periodicamente o status da operação, tornando uma solicitação GET para este local; Aguarde > 30 segundos entre as verificações.</span><span class="sxs-lookup"><span data-stu-id="13577-110">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="13577-111">Quando a solicitação for concluída com êxito, o status será "sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.</span><span class="sxs-lookup"><span data-stu-id="13577-111">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="13577-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13577-112">Properties</span></span>

| <span data-ttu-id="13577-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13577-113">Property</span></span> | <span data-ttu-id="13577-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="13577-114">Type</span></span>   | <span data-ttu-id="13577-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="13577-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="13577-116">id</span><span class="sxs-lookup"><span data-stu-id="13577-116">id</span></span>|<span data-ttu-id="13577-117">string</span><span class="sxs-lookup"><span data-stu-id="13577-117">string</span></span> |<span data-ttu-id="13577-118">Id exclusiva de operação.</span><span class="sxs-lookup"><span data-stu-id="13577-118">Unique operation id.</span></span>|
|<span data-ttu-id="13577-119">operationType</span><span class="sxs-lookup"><span data-stu-id="13577-119">operationType</span></span>|[<span data-ttu-id="13577-120">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="13577-120">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="13577-121">Indica qual tipo de operação está sendo descrito.</span><span class="sxs-lookup"><span data-stu-id="13577-121">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="13577-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13577-122">createdDateTime</span></span>|<span data-ttu-id="13577-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13577-123">DateTimeOffset</span></span> |<span data-ttu-id="13577-124">Hora em que a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="13577-124">Time when the operation was created.</span></span>|
|<span data-ttu-id="13577-125">status</span><span class="sxs-lookup"><span data-stu-id="13577-125">status</span></span>|[<span data-ttu-id="13577-126">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="13577-126">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="13577-127">Status de operação.</span><span class="sxs-lookup"><span data-stu-id="13577-127">Operation status.</span></span>|
|<span data-ttu-id="13577-128">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="13577-128">lastActionDateTime</span></span>|<span data-ttu-id="13577-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13577-129">DateTimeOffset</span></span> |<span data-ttu-id="13577-130">Hora de quando a operação assíncrona foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="13577-130">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="13577-131">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="13577-131">attemptsCount</span></span>|<span data-ttu-id="13577-132">Int32</span><span class="sxs-lookup"><span data-stu-id="13577-132">Int32</span></span>|<span data-ttu-id="13577-133">Número de vezes que a operação foi tentada antes de serem marcadas com êxito ou falha.</span><span class="sxs-lookup"><span data-stu-id="13577-133">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="13577-134">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="13577-134">targetResourceId</span></span>|<span data-ttu-id="13577-135">GUID</span><span class="sxs-lookup"><span data-stu-id="13577-135">guid</span></span> |<span data-ttu-id="13577-136">A identificação do objeto que tenha criado ou modificado como resultado dessa operação assíncrona, geralmente uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="13577-136">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="13577-137">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="13577-137">targetResourceLocation</span></span>|<span data-ttu-id="13577-138">string</span><span class="sxs-lookup"><span data-stu-id="13577-138">string</span></span>|<span data-ttu-id="13577-139">O local do objeto que tenha criado ou modificado como resultado dessa operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="13577-139">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="13577-140">Essa URL deve ser tratado como um valor opaco e não analisado em caminhos de seus componentes.</span><span class="sxs-lookup"><span data-stu-id="13577-140">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="13577-141">erro</span><span class="sxs-lookup"><span data-stu-id="13577-141">error</span></span>|[<span data-ttu-id="13577-142">operationError</span><span class="sxs-lookup"><span data-stu-id="13577-142">operationError</span></span>](operationerror.md)|<span data-ttu-id="13577-143">Qualquer erro que faz com que a operação assíncrona falhe.</span><span class="sxs-lookup"><span data-stu-id="13577-143">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13577-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13577-144">JSON representation</span></span>

<span data-ttu-id="13577-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13577-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
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
