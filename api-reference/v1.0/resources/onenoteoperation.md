---
title: Tipo de recurso do onenoteOperation
description: O status de determinadas operações do OneNote de longa duração.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 146cfec00c630fc0abde326a57374549d7b2d378
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961948"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="c85bd-103">Tipo de recurso do onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="c85bd-103">onenoteOperation resource type</span></span>

<span data-ttu-id="c85bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c85bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c85bd-105">O status de determinadas operações do OneNote de longa duração.</span><span class="sxs-lookup"><span data-stu-id="c85bd-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c85bd-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c85bd-106">JSON representation</span></span>

<span data-ttu-id="c85bd-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c85bd-107">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="c85bd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c85bd-108">Properties</span></span>
| <span data-ttu-id="c85bd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c85bd-109">Property</span></span>     | <span data-ttu-id="c85bd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c85bd-110">Type</span></span>   |<span data-ttu-id="c85bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c85bd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c85bd-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c85bd-112">createdDateTime</span></span>| <span data-ttu-id="c85bd-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c85bd-113">DateTimeOffset</span></span> |<span data-ttu-id="c85bd-114">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="c85bd-114">The start time of the operation.</span></span>|
|<span data-ttu-id="c85bd-115">erro</span><span class="sxs-lookup"><span data-stu-id="c85bd-115">error</span></span>|[<span data-ttu-id="c85bd-116">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="c85bd-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="c85bd-117">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="c85bd-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="c85bd-118">id</span><span class="sxs-lookup"><span data-stu-id="c85bd-118">id</span></span>|<span data-ttu-id="c85bd-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c85bd-119">string</span></span>|<span data-ttu-id="c85bd-120">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c85bd-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="c85bd-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c85bd-121">lastActionDateTime</span></span>| <span data-ttu-id="c85bd-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c85bd-122">DateTimeOffset</span></span> |<span data-ttu-id="c85bd-123">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="c85bd-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="c85bd-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="c85bd-124">resourceId</span></span>|<span data-ttu-id="c85bd-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c85bd-125">string</span></span>|<span data-ttu-id="c85bd-126">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="c85bd-126">The resource id.</span></span>|
|<span data-ttu-id="c85bd-127">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="c85bd-127">resourceLocation</span></span>|<span data-ttu-id="c85bd-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c85bd-128">string</span></span>|<span data-ttu-id="c85bd-129">O URI do recurso do objeto.</span><span class="sxs-lookup"><span data-stu-id="c85bd-129">The resource URI for the object.</span></span> <span data-ttu-id="c85bd-130">Por exemplo, o URI de recurso para uma página ou seção copiada.</span><span class="sxs-lookup"><span data-stu-id="c85bd-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="c85bd-131">status</span><span class="sxs-lookup"><span data-stu-id="c85bd-131">status</span></span>|<span data-ttu-id="c85bd-132">operationStatus</span><span class="sxs-lookup"><span data-stu-id="c85bd-132">operationStatus</span></span>|<span data-ttu-id="c85bd-133">O status atual da operação: `NotStarted` , `Running` , , `Completed` `Failed` .</span><span class="sxs-lookup"><span data-stu-id="c85bd-133">The current status of the operation: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span> |
|<span data-ttu-id="c85bd-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="c85bd-134">percentComplete</span></span>|<span data-ttu-id="c85bd-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c85bd-135">string</span></span>|<span data-ttu-id="c85bd-136">A porcentagem de operação será concluída se a operação ainda estiver em `running` status.</span><span class="sxs-lookup"><span data-stu-id="c85bd-136">The operation percent complete if the operation is still in `running` status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c85bd-137">Relações</span><span class="sxs-lookup"><span data-stu-id="c85bd-137">Relationships</span></span>
<span data-ttu-id="c85bd-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c85bd-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="c85bd-139">Métodos</span><span class="sxs-lookup"><span data-stu-id="c85bd-139">Methods</span></span>

| <span data-ttu-id="c85bd-140">Método</span><span class="sxs-lookup"><span data-stu-id="c85bd-140">Method</span></span>           | <span data-ttu-id="c85bd-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c85bd-141">Return Type</span></span>    |<span data-ttu-id="c85bd-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="c85bd-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c85bd-143">Obter operação</span><span class="sxs-lookup"><span data-stu-id="c85bd-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="c85bd-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="c85bd-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="c85bd-145">Obter o status da operação.</span><span class="sxs-lookup"><span data-stu-id="c85bd-145">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

