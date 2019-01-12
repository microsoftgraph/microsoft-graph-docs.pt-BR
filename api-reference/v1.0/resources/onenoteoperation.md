---
title: Tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: eaab313e9399e6e8724d5096b7ac29ec315889ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977462"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="49a61-103">Tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="49a61-103">onenoteOperation resource type</span></span>

<span data-ttu-id="49a61-104">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="49a61-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="49a61-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49a61-105">JSON representation</span></span>

<span data-ttu-id="49a61-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49a61-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="49a61-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49a61-107">Properties</span></span>
| <span data-ttu-id="49a61-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49a61-108">Property</span></span>     | <span data-ttu-id="49a61-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="49a61-109">Type</span></span>   |<span data-ttu-id="49a61-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="49a61-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49a61-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49a61-111">createdDateTime</span></span>| <span data-ttu-id="49a61-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49a61-112">DateTimeOffset</span></span> |<span data-ttu-id="49a61-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="49a61-113">The start time of the operation.</span></span>|
|<span data-ttu-id="49a61-114">erro</span><span class="sxs-lookup"><span data-stu-id="49a61-114">error</span></span>|[<span data-ttu-id="49a61-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="49a61-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="49a61-116">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="49a61-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="49a61-117">id</span><span class="sxs-lookup"><span data-stu-id="49a61-117">id</span></span>|<span data-ttu-id="49a61-118">string</span><span class="sxs-lookup"><span data-stu-id="49a61-118">string</span></span>|<span data-ttu-id="49a61-119">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49a61-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="49a61-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="49a61-120">lastActionDateTime</span></span>| <span data-ttu-id="49a61-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49a61-121">DateTimeOffset</span></span> |<span data-ttu-id="49a61-122">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="49a61-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="49a61-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="49a61-123">resourceId</span></span>|<span data-ttu-id="49a61-124">string</span><span class="sxs-lookup"><span data-stu-id="49a61-124">string</span></span>|<span data-ttu-id="49a61-125">A id do recurso.</span><span class="sxs-lookup"><span data-stu-id="49a61-125">The resource id.</span></span>|
|<span data-ttu-id="49a61-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="49a61-126">resourceLocation</span></span>|<span data-ttu-id="49a61-127">string</span><span class="sxs-lookup"><span data-stu-id="49a61-127">string</span></span>|<span data-ttu-id="49a61-p101">O URI de recurso do objeto. Por exemplo, o URI de recurso para uma seção ou página copiada.</span><span class="sxs-lookup"><span data-stu-id="49a61-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="49a61-130">status</span><span class="sxs-lookup"><span data-stu-id="49a61-130">status</span></span>|<span data-ttu-id="49a61-131">string</span><span class="sxs-lookup"><span data-stu-id="49a61-131">string</span></span>|<span data-ttu-id="49a61-132">O status atual da operação: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="49a61-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="49a61-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="49a61-133">percentComplete</span></span>|<span data-ttu-id="49a61-134">string</span><span class="sxs-lookup"><span data-stu-id="49a61-134">string</span></span>|<span data-ttu-id="49a61-135">A porcentagem concluída da operação se a operação ainda estiver com um status `running`</span><span class="sxs-lookup"><span data-stu-id="49a61-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="49a61-136">Relações</span><span class="sxs-lookup"><span data-stu-id="49a61-136">Relationships</span></span>
<span data-ttu-id="49a61-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49a61-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="49a61-138">Métodos</span><span class="sxs-lookup"><span data-stu-id="49a61-138">Methods</span></span>

| <span data-ttu-id="49a61-139">Método</span><span class="sxs-lookup"><span data-stu-id="49a61-139">Method</span></span>           | <span data-ttu-id="49a61-140">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="49a61-140">Return Type</span></span>    |<span data-ttu-id="49a61-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="49a61-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="49a61-142">Get operation</span><span class="sxs-lookup"><span data-stu-id="49a61-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="49a61-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="49a61-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="49a61-144">Obter o status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="49a61-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
