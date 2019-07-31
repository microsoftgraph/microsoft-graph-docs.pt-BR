---
title: tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 3f6a8bdfc6cee8b71fb77fb7778171677acb5df9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966430"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="7ab1e-103">tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="7ab1e-103">onenoteOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ab1e-104">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-104">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ab1e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ab1e-105">JSON representation</span></span>

<span data-ttu-id="7ab1e-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7ab1e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ab1e-107">Properties</span></span>
| <span data-ttu-id="7ab1e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ab1e-108">Property</span></span>     | <span data-ttu-id="7ab1e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ab1e-109">Type</span></span>   |<span data-ttu-id="7ab1e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ab1e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ab1e-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ab1e-111">createdDateTime</span></span>| <span data-ttu-id="7ab1e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ab1e-112">DateTimeOffset</span></span> |<span data-ttu-id="7ab1e-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-113">The start time of the operation.</span></span>|
|<span data-ttu-id="7ab1e-114">erro</span><span class="sxs-lookup"><span data-stu-id="7ab1e-114">error</span></span>|[<span data-ttu-id="7ab1e-115">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="7ab1e-115">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="7ab1e-116">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-116">The error returned by the operation.</span></span>|
|<span data-ttu-id="7ab1e-117">id</span><span class="sxs-lookup"><span data-stu-id="7ab1e-117">id</span></span>|<span data-ttu-id="7ab1e-118">string</span><span class="sxs-lookup"><span data-stu-id="7ab1e-118">string</span></span>|<span data-ttu-id="7ab1e-119">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-119">The operation id. Read-only.</span></span>|
|<span data-ttu-id="7ab1e-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7ab1e-120">lastActionDateTime</span></span>| <span data-ttu-id="7ab1e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ab1e-121">DateTimeOffset</span></span> |<span data-ttu-id="7ab1e-122">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-122">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="7ab1e-123">resourceId</span><span class="sxs-lookup"><span data-stu-id="7ab1e-123">resourceId</span></span>|<span data-ttu-id="7ab1e-124">string</span><span class="sxs-lookup"><span data-stu-id="7ab1e-124">string</span></span>|<span data-ttu-id="7ab1e-125">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-125">The resource id.</span></span>|
|<span data-ttu-id="7ab1e-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="7ab1e-126">resourceLocation</span></span>|<span data-ttu-id="7ab1e-127">string</span><span class="sxs-lookup"><span data-stu-id="7ab1e-127">string</span></span>|<span data-ttu-id="7ab1e-128">O URI do recurso para o objeto.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-128">The resource URI for the object.</span></span> <span data-ttu-id="7ab1e-129">Por exemplo, o URI do recurso para uma página ou seção copiada.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-129">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="7ab1e-130">status</span><span class="sxs-lookup"><span data-stu-id="7ab1e-130">status</span></span>|<span data-ttu-id="7ab1e-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ab1e-131">string</span></span>|<span data-ttu-id="7ab1e-132">O status atual da operação: `notstarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="7ab1e-132">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="7ab1e-133">percentComplete</span><span class="sxs-lookup"><span data-stu-id="7ab1e-133">percentComplete</span></span>|<span data-ttu-id="7ab1e-134">string</span><span class="sxs-lookup"><span data-stu-id="7ab1e-134">string</span></span>|<span data-ttu-id="7ab1e-135">A porcentagem concluída da operação se a operação ainda estiver `running` em status</span><span class="sxs-lookup"><span data-stu-id="7ab1e-135">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="7ab1e-136">Relações</span><span class="sxs-lookup"><span data-stu-id="7ab1e-136">Relationships</span></span>
<span data-ttu-id="7ab1e-137">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7ab1e-137">None</span></span>


## <a name="methods"></a><span data-ttu-id="7ab1e-138">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ab1e-138">Methods</span></span>

| <span data-ttu-id="7ab1e-139">Método</span><span class="sxs-lookup"><span data-stu-id="7ab1e-139">Method</span></span>           | <span data-ttu-id="7ab1e-140">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ab1e-140">Return Type</span></span>    |<span data-ttu-id="7ab1e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ab1e-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ab1e-142">Operação get</span><span class="sxs-lookup"><span data-stu-id="7ab1e-142">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="7ab1e-143">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="7ab1e-143">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="7ab1e-144">Obter o status da operação.</span><span class="sxs-lookup"><span data-stu-id="7ab1e-144">Get the status of the operation.</span></span> |

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
