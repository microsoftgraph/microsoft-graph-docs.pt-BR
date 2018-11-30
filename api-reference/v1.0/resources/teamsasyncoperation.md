---
title: tipo de recurso de teamsAsyncOperation
description: 'Uma operação assíncrona de Teams da Microsoft é uma operação que transcende o tempo de vida de uma única solicitação de API. '
ms.openlocfilehash: 4ec60a5f0137c45a9bc0488b31b76f80799e0545
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006195"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="9dbdb-103">tipo de recurso de teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="9dbdb-103">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="9dbdb-104">Uma operação assíncrona de Teams da Microsoft é uma operação que transcende o tempo de vida de uma única solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="9dbdb-105">Essas operações são muito caro concluir dentro do período de tempo de sua solicitação de origem ou de longa execução.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="9dbdb-106">Quando é iniciada uma operação assíncrona, o método retornará um código de resposta 202 aceitos.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="9dbdb-107">A resposta conterá também um cabeçalho de local, que contém a localização do teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="9dbdb-108">Verificar periodicamente o status da operação, tornando uma solicitação GET para este local; Aguarde > 30 segundos entre as verificações.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="9dbdb-109">Quando a solicitação for concluída com êxito, o status será "sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="9dbdb-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9dbdb-110">Properties</span></span>

| <span data-ttu-id="9dbdb-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9dbdb-111">Property</span></span> | <span data-ttu-id="9dbdb-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dbdb-112">Type</span></span>   | <span data-ttu-id="9dbdb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dbdb-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9dbdb-114">id</span><span class="sxs-lookup"><span data-stu-id="9dbdb-114">id</span></span>|<span data-ttu-id="9dbdb-115">string</span><span class="sxs-lookup"><span data-stu-id="9dbdb-115">string</span></span> |<span data-ttu-id="9dbdb-116">Id exclusiva de operação.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-116">Unique operation id.</span></span>|
|<span data-ttu-id="9dbdb-117">operationType</span><span class="sxs-lookup"><span data-stu-id="9dbdb-117">operationType</span></span>|[<span data-ttu-id="9dbdb-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="9dbdb-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="9dbdb-119">Indica qual tipo de operação está sendo descrito.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="9dbdb-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9dbdb-120">createdDateTime</span></span>|<span data-ttu-id="9dbdb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dbdb-121">DateTimeOffset</span></span> |<span data-ttu-id="9dbdb-122">Hora em que a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="9dbdb-123">status</span><span class="sxs-lookup"><span data-stu-id="9dbdb-123">status</span></span>|[<span data-ttu-id="9dbdb-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="9dbdb-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="9dbdb-125">Status de operação.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-125">Operation status.</span></span>|
|<span data-ttu-id="9dbdb-126">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="9dbdb-126">lastActionDateTime</span></span>|<span data-ttu-id="9dbdb-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9dbdb-127">DateTimeOffset</span></span> |<span data-ttu-id="9dbdb-128">Hora de quando a operação assíncrona foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="9dbdb-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="9dbdb-129">attemptsCount</span></span>|<span data-ttu-id="9dbdb-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9dbdb-130">Int32</span></span>|<span data-ttu-id="9dbdb-131">Número de vezes que a operação foi tentada antes de serem marcadas com êxito ou falha.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="9dbdb-132">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="9dbdb-132">targetResourceId</span></span>|<span data-ttu-id="9dbdb-133">GUID</span><span class="sxs-lookup"><span data-stu-id="9dbdb-133">guid</span></span> |<span data-ttu-id="9dbdb-134">A identificação do objeto que tenha criado ou modificado como resultado dessa operação assíncrona, geralmente uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9dbdb-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="9dbdb-135">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="9dbdb-135">targetResourceLocation</span></span>|<span data-ttu-id="9dbdb-136">string</span><span class="sxs-lookup"><span data-stu-id="9dbdb-136">string</span></span>|<span data-ttu-id="9dbdb-137">O local do objeto que tenha criado ou modificado como resultado dessa operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="9dbdb-138">Essa URL deve ser tratado como um valor opaco e não analisado em caminhos de seus componentes.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="9dbdb-139">erro</span><span class="sxs-lookup"><span data-stu-id="9dbdb-139">error</span></span>|[<span data-ttu-id="9dbdb-140">operationError</span><span class="sxs-lookup"><span data-stu-id="9dbdb-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="9dbdb-141">Qualquer erro que faz com que a operação assíncrona falhe.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9dbdb-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9dbdb-142">JSON representation</span></span>

<span data-ttu-id="9dbdb-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9dbdb-143">The following is a JSON representation of the resource.</span></span>

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
