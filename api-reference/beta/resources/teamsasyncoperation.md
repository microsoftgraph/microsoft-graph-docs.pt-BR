---
title: tipo de recurso teamsAsyncOperation
description: 'Uma operação assíncrona do Microsoft Teams é uma operação que transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a3a0e74d936282edb58f166ca7b4c8e5a51ff116
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964484"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="c7967-103">tipo de recurso teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="c7967-103">teamsAsyncOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7967-104">Uma operação assíncrona do Microsoft Teams é uma operação que transcende o tempo de vida de uma única solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="c7967-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="c7967-105">Essas operações são de longa duração ou muito caras para concluir dentro do prazo de sua solicitação de origem.</span><span class="sxs-lookup"><span data-stu-id="c7967-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="c7967-106">Quando uma operação assíncrona é iniciada, o método retorna um código de resposta aceito 202.</span><span class="sxs-lookup"><span data-stu-id="c7967-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="c7967-107">A resposta também conterá um cabeçalho de local, que contém o local do teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="c7967-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="c7967-108">Verifique periodicamente o status da operação fazendo uma solicitação GET para este local; Aguarde >30 segundos entre as verificações.</span><span class="sxs-lookup"><span data-stu-id="c7967-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="c7967-109">Quando a solicitação for concluída com êxito, o status será "bem-sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.</span><span class="sxs-lookup"><span data-stu-id="c7967-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="c7967-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7967-110">Properties</span></span>

| <span data-ttu-id="c7967-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7967-111">Property</span></span> | <span data-ttu-id="c7967-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7967-112">Type</span></span>   | <span data-ttu-id="c7967-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7967-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c7967-114">id</span><span class="sxs-lookup"><span data-stu-id="c7967-114">id</span></span>|<span data-ttu-id="c7967-115">string</span><span class="sxs-lookup"><span data-stu-id="c7967-115">string</span></span> |<span data-ttu-id="c7967-116">ID de operação exclusiva.</span><span class="sxs-lookup"><span data-stu-id="c7967-116">Unique operation id.</span></span>|
|<span data-ttu-id="c7967-117">OperationType</span><span class="sxs-lookup"><span data-stu-id="c7967-117">operationType</span></span>|[<span data-ttu-id="c7967-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="c7967-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="c7967-119">Indica o tipo de operação que está sendo descrito.</span><span class="sxs-lookup"><span data-stu-id="c7967-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="c7967-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7967-120">createdDateTime</span></span>|<span data-ttu-id="c7967-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7967-121">DateTimeOffset</span></span> |<span data-ttu-id="c7967-122">Hora em que a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="c7967-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="c7967-123">status</span><span class="sxs-lookup"><span data-stu-id="c7967-123">status</span></span>|[<span data-ttu-id="c7967-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="c7967-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="c7967-125">Status da operação.</span><span class="sxs-lookup"><span data-stu-id="c7967-125">Operation status.</span></span>|
|<span data-ttu-id="c7967-126">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c7967-126">lastActionDateTime</span></span>|<span data-ttu-id="c7967-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7967-127">DateTimeOffset</span></span> |<span data-ttu-id="c7967-128">Hora em que a operação assíncrona foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c7967-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="c7967-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="c7967-129">attemptsCount</span></span>|<span data-ttu-id="c7967-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c7967-130">Int32</span></span>|<span data-ttu-id="c7967-131">Número de vezes em que a operação foi tentada antes de ser marcada com êxito ou falhou.</span><span class="sxs-lookup"><span data-stu-id="c7967-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="c7967-132">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="c7967-132">targetResourceId</span></span>|<span data-ttu-id="c7967-133">#c0</span><span class="sxs-lookup"><span data-stu-id="c7967-133">guid</span></span> |<span data-ttu-id="c7967-134">A ID do objeto que é criado ou modificado como resultado dessa operação assíncrona, normalmente uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c7967-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="c7967-135">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="c7967-135">targetResourceLocation</span></span>|<span data-ttu-id="c7967-136">string</span><span class="sxs-lookup"><span data-stu-id="c7967-136">string</span></span>|<span data-ttu-id="c7967-137">O local do objeto que é criado ou modificado como resultado dessa operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="c7967-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="c7967-138">Essa URL deve ser tratada como um valor opaco e não analisada em seus caminhos de componente.</span><span class="sxs-lookup"><span data-stu-id="c7967-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="c7967-139">erro</span><span class="sxs-lookup"><span data-stu-id="c7967-139">error</span></span>|[<span data-ttu-id="c7967-140">operationError</span><span class="sxs-lookup"><span data-stu-id="c7967-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="c7967-141">Qualquer erro que causa falha na operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="c7967-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7967-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7967-142">JSON representation</span></span>

<span data-ttu-id="c7967-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7967-143">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
