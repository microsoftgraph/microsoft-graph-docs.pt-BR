---
title: Tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: Jewan-microsoft
ms.openlocfilehash: bbb7b9457ce5a3d7ba9faf45d893ae86cdfd8b32
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326905"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="a3e2e-103">Tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="a3e2e-103">onenoteOperation resource type</span></span>

<span data-ttu-id="a3e2e-104">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3e2e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3e2e-105">JSON representation</span></span>

<span data-ttu-id="a3e2e-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a3e2e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3e2e-107">Properties</span></span>
| <span data-ttu-id="a3e2e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3e2e-108">Property</span></span>     | <span data-ttu-id="a3e2e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3e2e-109">Type</span></span>   |<span data-ttu-id="a3e2e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3e2e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3e2e-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3e2e-111">createdDateTime</span></span>| <span data-ttu-id="a3e2e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3e2e-112">DateTimeOffset</span></span> |<span data-ttu-id="a3e2e-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-113">The start time of the operation.</span></span>|
|<span data-ttu-id="a3e2e-114">erro</span><span class="sxs-lookup"><span data-stu-id="a3e2e-114">error</span></span>|[<span data-ttu-id="a3e2e-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="a3e2e-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="a3e2e-116">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="a3e2e-117">id</span><span class="sxs-lookup"><span data-stu-id="a3e2e-117">id</span></span>|<span data-ttu-id="a3e2e-118">string</span><span class="sxs-lookup"><span data-stu-id="a3e2e-118">string</span></span>|<span data-ttu-id="a3e2e-119">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="a3e2e-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="a3e2e-120">lastActionDateTime</span></span>| <span data-ttu-id="a3e2e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3e2e-121">DateTimeOffset</span></span> |<span data-ttu-id="a3e2e-122">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="a3e2e-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="a3e2e-123">resourceId</span></span>|<span data-ttu-id="a3e2e-124">string</span><span class="sxs-lookup"><span data-stu-id="a3e2e-124">string</span></span>|<span data-ttu-id="a3e2e-125">A id do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-125">The resource id.</span></span>|
|<span data-ttu-id="a3e2e-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="a3e2e-126">resourceLocation</span></span>|<span data-ttu-id="a3e2e-127">string</span><span class="sxs-lookup"><span data-stu-id="a3e2e-127">string</span></span>|<span data-ttu-id="a3e2e-p101">O URI de recurso do objeto. Por exemplo, o URI de recurso para uma seção ou página copiada.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="a3e2e-130">status</span><span class="sxs-lookup"><span data-stu-id="a3e2e-130">status</span></span>|<span data-ttu-id="a3e2e-131">string</span><span class="sxs-lookup"><span data-stu-id="a3e2e-131">string</span></span>|<span data-ttu-id="a3e2e-132">O status atual da operação: `notstarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="a3e2e-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="a3e2e-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="a3e2e-133">percentComplete</span></span>|<span data-ttu-id="a3e2e-134">string</span><span class="sxs-lookup"><span data-stu-id="a3e2e-134">string</span></span>|<span data-ttu-id="a3e2e-135">A porcentagem concluída da operação se a operação ainda estiver com um status `running`</span><span class="sxs-lookup"><span data-stu-id="a3e2e-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="a3e2e-136">Relações</span><span class="sxs-lookup"><span data-stu-id="a3e2e-136">Relationships</span></span>
<span data-ttu-id="a3e2e-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3e2e-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="a3e2e-138">Métodos</span><span class="sxs-lookup"><span data-stu-id="a3e2e-138">Methods</span></span>

| <span data-ttu-id="a3e2e-139">Método</span><span class="sxs-lookup"><span data-stu-id="a3e2e-139">Method</span></span>           | <span data-ttu-id="a3e2e-140">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a3e2e-140">Return Type</span></span>    |<span data-ttu-id="a3e2e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3e2e-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3e2e-142">Get operation</span><span class="sxs-lookup"><span data-stu-id="a3e2e-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="a3e2e-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="a3e2e-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="a3e2e-144">Obter o status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="a3e2e-144">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
