---
title: Tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 146a1b1d9a51cc541e06fd789f987a2d39dff48a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512847"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="999c0-103">Tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="999c0-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="999c0-104">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="999c0-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="999c0-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="999c0-105">JSON representation</span></span>

<span data-ttu-id="999c0-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="999c0-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="999c0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="999c0-107">Properties</span></span>
| <span data-ttu-id="999c0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="999c0-108">Property</span></span>     | <span data-ttu-id="999c0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="999c0-109">Type</span></span>   |<span data-ttu-id="999c0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="999c0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="999c0-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="999c0-111">createdDateTime</span></span>| <span data-ttu-id="999c0-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="999c0-112">DateTimeOffset</span></span> |<span data-ttu-id="999c0-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="999c0-113">The start time of the operation.</span></span>|
|<span data-ttu-id="999c0-114">erro</span><span class="sxs-lookup"><span data-stu-id="999c0-114">error</span></span>|[<span data-ttu-id="999c0-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="999c0-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="999c0-116">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="999c0-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="999c0-117">id</span><span class="sxs-lookup"><span data-stu-id="999c0-117">id</span></span>|<span data-ttu-id="999c0-118">string</span><span class="sxs-lookup"><span data-stu-id="999c0-118">string</span></span>|<span data-ttu-id="999c0-119">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="999c0-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="999c0-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="999c0-120">lastActionDateTime</span></span>| <span data-ttu-id="999c0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="999c0-121">DateTimeOffset</span></span> |<span data-ttu-id="999c0-122">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="999c0-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="999c0-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="999c0-123">resourceId</span></span>|<span data-ttu-id="999c0-124">string</span><span class="sxs-lookup"><span data-stu-id="999c0-124">string</span></span>|<span data-ttu-id="999c0-125">A id do recurso.</span><span class="sxs-lookup"><span data-stu-id="999c0-125">The resource id.</span></span>|
|<span data-ttu-id="999c0-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="999c0-126">resourceLocation</span></span>|<span data-ttu-id="999c0-127">string</span><span class="sxs-lookup"><span data-stu-id="999c0-127">string</span></span>|<span data-ttu-id="999c0-p101">O URI de recurso do objeto. Por exemplo, o URI de recurso para uma seção ou página copiada.</span><span class="sxs-lookup"><span data-stu-id="999c0-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="999c0-130">status</span><span class="sxs-lookup"><span data-stu-id="999c0-130">status</span></span>|<span data-ttu-id="999c0-131">string</span><span class="sxs-lookup"><span data-stu-id="999c0-131">string</span></span>|<span data-ttu-id="999c0-132">O status atual da operação: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="999c0-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="999c0-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="999c0-133">percentComplete</span></span>|<span data-ttu-id="999c0-134">string</span><span class="sxs-lookup"><span data-stu-id="999c0-134">string</span></span>|<span data-ttu-id="999c0-135">A porcentagem concluída da operação se a operação ainda estiver com um status `running`</span><span class="sxs-lookup"><span data-stu-id="999c0-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="999c0-136">Relações</span><span class="sxs-lookup"><span data-stu-id="999c0-136">Relationships</span></span>
<span data-ttu-id="999c0-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="999c0-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="999c0-138">Métodos</span><span class="sxs-lookup"><span data-stu-id="999c0-138">Methods</span></span>

| <span data-ttu-id="999c0-139">Método</span><span class="sxs-lookup"><span data-stu-id="999c0-139">Method</span></span>           | <span data-ttu-id="999c0-140">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="999c0-140">Return Type</span></span>    |<span data-ttu-id="999c0-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="999c0-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="999c0-142">Get operation</span><span class="sxs-lookup"><span data-stu-id="999c0-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="999c0-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="999c0-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="999c0-144">Obter o status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="999c0-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
