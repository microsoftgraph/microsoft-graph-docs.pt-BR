---
title: Tipo de recurso teamsAsyncOperation
description: 'Uma Microsoft Teams assíncrona é uma operação que transcende o tempo de vida de uma única solicitação de API. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9239e9543b77348b4524dc76be8fee64e1b9919a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030835"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="5d357-103">Tipo de recurso teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="5d357-103">teamsAsyncOperation resource type</span></span>

<span data-ttu-id="5d357-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d357-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d357-105">Uma Microsoft Teams assíncrona é uma operação que transcende o tempo de vida de uma única solicitação de API.</span><span class="sxs-lookup"><span data-stu-id="5d357-105">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="5d357-106">Essas operações são de longa duração ou muito caras para concluir dentro do período de tempo de sua solicitação de origem.</span><span class="sxs-lookup"><span data-stu-id="5d357-106">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="5d357-107">Quando uma operação assíncrona é iniciada, o método retorna um código de resposta aceito 202.</span><span class="sxs-lookup"><span data-stu-id="5d357-107">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="5d357-108">A resposta também conterá um header Location, que contém o local do teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="5d357-108">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="5d357-109">Verifique periodicamente o status da operação fazendo uma solicitação GET para esse local; aguarde >30 segundos entre verificações.</span><span class="sxs-lookup"><span data-stu-id="5d357-109">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="5d357-110">Quando a solicitação for concluída com êxito, o status será "bem-sucedido" e o targetResourceLocation apontará para o recurso criado/modificado.</span><span class="sxs-lookup"><span data-stu-id="5d357-110">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="methods"></a><span data-ttu-id="5d357-111">Methods</span><span class="sxs-lookup"><span data-stu-id="5d357-111">Methods</span></span>

|  <span data-ttu-id="5d357-112">Método</span><span class="sxs-lookup"><span data-stu-id="5d357-112">Method</span></span>                                                                   |  <span data-ttu-id="5d357-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5d357-113">Return Type</span></span>                                                                     | <span data-ttu-id="5d357-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d357-114">Description</span></span>                                                       | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :---------------------------------------------------------------- |
| [<span data-ttu-id="5d357-115">Listar operações em um chat</span><span class="sxs-lookup"><span data-stu-id="5d357-115">List operations on a chat</span></span>](../api/chat-list-operations.md)               | <span data-ttu-id="5d357-116">Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="5d357-116">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="5d357-117">Listar operações assíncronas que executam ou estão em execução em um chat específico.</span><span class="sxs-lookup"><span data-stu-id="5d357-117">List async operations that ran or are running on a specific chat.</span></span> |
| [<span data-ttu-id="5d357-118">Obter operação</span><span class="sxs-lookup"><span data-stu-id="5d357-118">Get operation</span></span>](../api/teamsasyncoperation-get.md)                   | <span data-ttu-id="5d357-119">Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="5d357-119">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="5d357-120">Obter uma operação assíncrona que foi executado ou está sendo executado em um recurso específico.</span><span class="sxs-lookup"><span data-stu-id="5d357-120">Get an async operation that ran or is running on a specific resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="5d357-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d357-121">Properties</span></span>

| <span data-ttu-id="5d357-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d357-122">Property</span></span> | <span data-ttu-id="5d357-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d357-123">Type</span></span>   | <span data-ttu-id="5d357-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d357-124">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5d357-125">id</span><span class="sxs-lookup"><span data-stu-id="5d357-125">id</span></span>|<span data-ttu-id="5d357-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d357-126">string</span></span> |<span data-ttu-id="5d357-127">ID de operação exclusiva.</span><span class="sxs-lookup"><span data-stu-id="5d357-127">Unique operation id.</span></span>|
|<span data-ttu-id="5d357-128">operationType</span><span class="sxs-lookup"><span data-stu-id="5d357-128">operationType</span></span>|[<span data-ttu-id="5d357-129">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="5d357-129">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="5d357-130">Indica qual tipo de operação está sendo descrito.</span><span class="sxs-lookup"><span data-stu-id="5d357-130">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="5d357-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d357-131">createdDateTime</span></span>|<span data-ttu-id="5d357-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d357-132">DateTimeOffset</span></span> |<span data-ttu-id="5d357-133">Hora em que a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="5d357-133">Time when the operation was created.</span></span>|
|<span data-ttu-id="5d357-134">status</span><span class="sxs-lookup"><span data-stu-id="5d357-134">status</span></span>|[<span data-ttu-id="5d357-135">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="5d357-135">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="5d357-136">Status da operação.</span><span class="sxs-lookup"><span data-stu-id="5d357-136">Operation status.</span></span>|
|<span data-ttu-id="5d357-137">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="5d357-137">lastActionDateTime</span></span>|<span data-ttu-id="5d357-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d357-138">DateTimeOffset</span></span> |<span data-ttu-id="5d357-139">Hora em que a operação assíncrona foi atualizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5d357-139">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="5d357-140">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="5d357-140">attemptsCount</span></span>|<span data-ttu-id="5d357-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5d357-141">Int32</span></span>|<span data-ttu-id="5d357-142">Número de vezes que a operação foi tentada antes de ser marcada com êxito ou falha.</span><span class="sxs-lookup"><span data-stu-id="5d357-142">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="5d357-143">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="5d357-143">targetResourceId</span></span>|<span data-ttu-id="5d357-144">guid</span><span class="sxs-lookup"><span data-stu-id="5d357-144">guid</span></span> |<span data-ttu-id="5d357-145">A ID do objeto criado ou modificado como resultado dessa operação assíncrona, normalmente uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="5d357-145">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="5d357-146">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="5d357-146">targetResourceLocation</span></span>|<span data-ttu-id="5d357-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d357-147">string</span></span>|<span data-ttu-id="5d357-148">O local do objeto criado ou modificado como resultado dessa operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="5d357-148">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="5d357-149">Essa URL deve ser tratada como um valor opaco e não analisado em seus caminhos de componente.</span><span class="sxs-lookup"><span data-stu-id="5d357-149">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="5d357-150">erro</span><span class="sxs-lookup"><span data-stu-id="5d357-150">error</span></span>|[<span data-ttu-id="5d357-151">operationError</span><span class="sxs-lookup"><span data-stu-id="5d357-151">operationError</span></span>](operationerror.md)|<span data-ttu-id="5d357-152">Qualquer erro que cause falha na operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="5d357-152">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d357-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d357-153">JSON representation</span></span>

<span data-ttu-id="5d357-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d357-154">The following is a JSON representation of the resource.</span></span>

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


