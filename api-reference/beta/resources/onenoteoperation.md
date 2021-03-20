---
title: Tipo de recurso do onenoteOperation
description: O status de determinadas operações do OneNote de longa duração.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 84b1570a86b9ea01712c6859a470fbf1092f6ca3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952778"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="09ffa-103">Tipo de recurso do onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="09ffa-103">onenoteOperation resource type</span></span>

<span data-ttu-id="09ffa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09ffa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ffa-105">O status de determinadas operações do OneNote de longa duração.</span><span class="sxs-lookup"><span data-stu-id="09ffa-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09ffa-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09ffa-106">JSON representation</span></span>

<span data-ttu-id="09ffa-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09ffa-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
## <a name="properties"></a><span data-ttu-id="09ffa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09ffa-108">Properties</span></span>
| <span data-ttu-id="09ffa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09ffa-109">Property</span></span>     | <span data-ttu-id="09ffa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="09ffa-110">Type</span></span>   |<span data-ttu-id="09ffa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="09ffa-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09ffa-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09ffa-112">createdDateTime</span></span>| <span data-ttu-id="09ffa-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09ffa-113">DateTimeOffset</span></span> |<span data-ttu-id="09ffa-114">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="09ffa-114">The start time of the operation.</span></span>|
|<span data-ttu-id="09ffa-115">erro</span><span class="sxs-lookup"><span data-stu-id="09ffa-115">error</span></span>|[<span data-ttu-id="09ffa-116">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="09ffa-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="09ffa-117">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="09ffa-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="09ffa-118">id</span><span class="sxs-lookup"><span data-stu-id="09ffa-118">id</span></span>|<span data-ttu-id="09ffa-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09ffa-119">string</span></span>|<span data-ttu-id="09ffa-120">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09ffa-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="09ffa-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="09ffa-121">lastActionDateTime</span></span>| <span data-ttu-id="09ffa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09ffa-122">DateTimeOffset</span></span> |<span data-ttu-id="09ffa-123">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="09ffa-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="09ffa-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="09ffa-124">resourceId</span></span>|<span data-ttu-id="09ffa-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09ffa-125">string</span></span>|<span data-ttu-id="09ffa-126">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="09ffa-126">The resource id.</span></span>|
|<span data-ttu-id="09ffa-127">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="09ffa-127">resourceLocation</span></span>|<span data-ttu-id="09ffa-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09ffa-128">string</span></span>|<span data-ttu-id="09ffa-129">O URI do recurso do objeto.</span><span class="sxs-lookup"><span data-stu-id="09ffa-129">The resource URI for the object.</span></span> <span data-ttu-id="09ffa-130">Por exemplo, o URI de recurso para uma página ou seção copiada.</span><span class="sxs-lookup"><span data-stu-id="09ffa-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="09ffa-131">status</span><span class="sxs-lookup"><span data-stu-id="09ffa-131">status</span></span>|<span data-ttu-id="09ffa-132">operationStatus</span><span class="sxs-lookup"><span data-stu-id="09ffa-132">operationStatus</span></span>|<span data-ttu-id="09ffa-133">O status atual da operação: `NotStarted` , `Running` , , `Completed` `Failed` .</span><span class="sxs-lookup"><span data-stu-id="09ffa-133">The current status of the operation: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span> |
|<span data-ttu-id="09ffa-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="09ffa-134">percentComplete</span></span>|<span data-ttu-id="09ffa-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09ffa-135">string</span></span>|<span data-ttu-id="09ffa-136">A porcentagem de operação será concluída se a operação ainda estiver em `running` status.</span><span class="sxs-lookup"><span data-stu-id="09ffa-136">The operation percent complete if the operation is still in `running` status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09ffa-137">Relações</span><span class="sxs-lookup"><span data-stu-id="09ffa-137">Relationships</span></span>
<span data-ttu-id="09ffa-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="09ffa-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="09ffa-139">Métodos</span><span class="sxs-lookup"><span data-stu-id="09ffa-139">Methods</span></span>

| <span data-ttu-id="09ffa-140">Método</span><span class="sxs-lookup"><span data-stu-id="09ffa-140">Method</span></span>           | <span data-ttu-id="09ffa-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="09ffa-141">Return Type</span></span>    |<span data-ttu-id="09ffa-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="09ffa-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09ffa-143">Obter operação</span><span class="sxs-lookup"><span data-stu-id="09ffa-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="09ffa-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="09ffa-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="09ffa-145">Obter o status da operação.</span><span class="sxs-lookup"><span data-stu-id="09ffa-145">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


