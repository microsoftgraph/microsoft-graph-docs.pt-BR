---
title: tipo de recurso teamsAsyncOperation
description: 'Uma operação assíncrona do Microsoft Teams é uma operação que transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 61c26b0d594ccdbad8020557f60c6f6b23a83254
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581549"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="d1fc9-103">tipo de recurso teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d1fc9-103">teamsAsyncOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1fc9-104">Uma operação assíncrona do Microsoft Teams é uma operação que transcende o tempo de vida de uma única solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="d1fc9-105">Essas operações são de longa duração ou muito caras para concluir dentro do prazo de sua solicitação de origem.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="d1fc9-106">Quando uma operação assíncrona é iniciada, o método retorna um código de resposta aceito 202.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="d1fc9-107">A resposta também conterá um cabeçalho de local, que contém o local do teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="d1fc9-108">Verifique periodicamente o status da operação fazendo uma solicitação GET para este local; Aguarde >30 segundos entre as verificações.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="d1fc9-109">Quando a solicitação for concluída com êxito, o status será "bem-sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d1fc9-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1fc9-110">Properties</span></span>

| <span data-ttu-id="d1fc9-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1fc9-111">Property</span></span> | <span data-ttu-id="d1fc9-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1fc9-112">Type</span></span>   | <span data-ttu-id="d1fc9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1fc9-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d1fc9-114">id</span><span class="sxs-lookup"><span data-stu-id="d1fc9-114">id</span></span>|<span data-ttu-id="d1fc9-115">string</span><span class="sxs-lookup"><span data-stu-id="d1fc9-115">string</span></span> |<span data-ttu-id="d1fc9-116">ID de operação exclusiva.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-116">Unique operation id.</span></span>|
|<span data-ttu-id="d1fc9-117">OperationType</span><span class="sxs-lookup"><span data-stu-id="d1fc9-117">operationType</span></span>|[<span data-ttu-id="d1fc9-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="d1fc9-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="d1fc9-119">Indica o tipo de operação que está sendo descrito.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="d1fc9-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1fc9-120">createdDateTime</span></span>|<span data-ttu-id="d1fc9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1fc9-121">DateTimeOffset</span></span> |<span data-ttu-id="d1fc9-122">Hora em que a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="d1fc9-123">status</span><span class="sxs-lookup"><span data-stu-id="d1fc9-123">status</span></span>|[<span data-ttu-id="d1fc9-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="d1fc9-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="d1fc9-125">Status da operação.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-125">Operation status.</span></span>|
|<span data-ttu-id="d1fc9-126">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d1fc9-126">lastActionDateTime</span></span>|<span data-ttu-id="d1fc9-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1fc9-127">DateTimeOffset</span></span> |<span data-ttu-id="d1fc9-128">Hora em que a operação assíncrona foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="d1fc9-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="d1fc9-129">attemptsCount</span></span>|<span data-ttu-id="d1fc9-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fc9-130">Int32</span></span>|<span data-ttu-id="d1fc9-131">Número de vezes em que a operação foi tentada antes de ser marcada com êxito ou falhou.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="d1fc9-132">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="d1fc9-132">targetResourceId</span></span>|<span data-ttu-id="d1fc9-133">#c0</span><span class="sxs-lookup"><span data-stu-id="d1fc9-133">guid</span></span> |<span data-ttu-id="d1fc9-134">A ID do objeto que é criado ou modificado como resultado dessa operação assíncrona, normalmente uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d1fc9-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="d1fc9-135">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="d1fc9-135">targetResourceLocation</span></span>|<span data-ttu-id="d1fc9-136">string</span><span class="sxs-lookup"><span data-stu-id="d1fc9-136">string</span></span>|<span data-ttu-id="d1fc9-137">O local do objeto que é criado ou modificado como resultado dessa operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="d1fc9-138">Essa URL deve ser tratada como um valor opaco e não analisada em seus caminhos de componente.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="d1fc9-139">erro</span><span class="sxs-lookup"><span data-stu-id="d1fc9-139">error</span></span>|[<span data-ttu-id="d1fc9-140">operationError</span><span class="sxs-lookup"><span data-stu-id="d1fc9-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="d1fc9-141">Qualquer erro que causa falha na operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1fc9-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1fc9-142">JSON representation</span></span>

<span data-ttu-id="d1fc9-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1fc9-143">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
