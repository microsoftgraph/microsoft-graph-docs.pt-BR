---
title: tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 179bdad12d81298605a7ac196ab717b9024e9df0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035774"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="680d5-103">tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="680d5-103">onenoteOperation resource type</span></span>

<span data-ttu-id="680d5-104">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="680d5-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="680d5-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="680d5-105">JSON representation</span></span>

<span data-ttu-id="680d5-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="680d5-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="680d5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="680d5-107">Properties</span></span>
| <span data-ttu-id="680d5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="680d5-108">Property</span></span>     | <span data-ttu-id="680d5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="680d5-109">Type</span></span>   |<span data-ttu-id="680d5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="680d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="680d5-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="680d5-111">createdDateTime</span></span>| <span data-ttu-id="680d5-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="680d5-112">DateTimeOffset</span></span> |<span data-ttu-id="680d5-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="680d5-113">The start time of the operation.</span></span>|
|<span data-ttu-id="680d5-114">erro</span><span class="sxs-lookup"><span data-stu-id="680d5-114">error</span></span>|[<span data-ttu-id="680d5-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="680d5-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="680d5-116">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="680d5-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="680d5-117">id</span><span class="sxs-lookup"><span data-stu-id="680d5-117">id</span></span>|<span data-ttu-id="680d5-118">string</span><span class="sxs-lookup"><span data-stu-id="680d5-118">string</span></span>|<span data-ttu-id="680d5-119">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="680d5-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="680d5-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="680d5-120">lastActionDateTime</span></span>| <span data-ttu-id="680d5-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="680d5-121">DateTimeOffset</span></span> |<span data-ttu-id="680d5-122">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="680d5-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="680d5-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="680d5-123">resourceId</span></span>|<span data-ttu-id="680d5-124">string</span><span class="sxs-lookup"><span data-stu-id="680d5-124">string</span></span>|<span data-ttu-id="680d5-125">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="680d5-125">The resource id.</span></span>|
|<span data-ttu-id="680d5-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="680d5-126">resourceLocation</span></span>|<span data-ttu-id="680d5-127">string</span><span class="sxs-lookup"><span data-stu-id="680d5-127">string</span></span>|<span data-ttu-id="680d5-128">O URI do recurso para o objeto.</span><span class="sxs-lookup"><span data-stu-id="680d5-128">The resource URI for the object.</span></span> <span data-ttu-id="680d5-129">Por exemplo, o URI do recurso para uma página ou seção copiada.</span><span class="sxs-lookup"><span data-stu-id="680d5-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="680d5-130">status</span><span class="sxs-lookup"><span data-stu-id="680d5-130">status</span></span>|<span data-ttu-id="680d5-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="680d5-131">string</span></span>|<span data-ttu-id="680d5-132">O status atual da operação: `notstarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="680d5-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="680d5-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="680d5-133">percentComplete</span></span>|<span data-ttu-id="680d5-134">string</span><span class="sxs-lookup"><span data-stu-id="680d5-134">string</span></span>|<span data-ttu-id="680d5-135">A porcentagem concluída da operação se a operação ainda estiver `running` em status</span><span class="sxs-lookup"><span data-stu-id="680d5-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="680d5-136">Relações</span><span class="sxs-lookup"><span data-stu-id="680d5-136">Relationships</span></span>
<span data-ttu-id="680d5-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="680d5-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="680d5-138">Métodos</span><span class="sxs-lookup"><span data-stu-id="680d5-138">Methods</span></span>

| <span data-ttu-id="680d5-139">Método</span><span class="sxs-lookup"><span data-stu-id="680d5-139">Method</span></span>           | <span data-ttu-id="680d5-140">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="680d5-140">Return Type</span></span>    |<span data-ttu-id="680d5-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="680d5-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="680d5-142">Operação get</span><span class="sxs-lookup"><span data-stu-id="680d5-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="680d5-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="680d5-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="680d5-144">Obter o status da operação.</span><span class="sxs-lookup"><span data-stu-id="680d5-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
