---
title: tipo de recurso onenoteOperation
description: O status de determinadas operações demoradas do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 500a4c20583f6af9cc8bacf98dd4de60354f0ab2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522341"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="f4ea1-103">tipo de recurso onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f4ea1-103">onenoteOperation resource type</span></span>

<span data-ttu-id="f4ea1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4ea1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4ea1-105">O status de determinadas operações demoradas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-105">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4ea1-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4ea1-106">JSON representation</span></span>

<span data-ttu-id="f4ea1-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f4ea1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4ea1-108">Properties</span></span>
| <span data-ttu-id="f4ea1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4ea1-109">Property</span></span>     | <span data-ttu-id="f4ea1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ea1-110">Type</span></span>   |<span data-ttu-id="f4ea1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ea1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4ea1-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ea1-112">createdDateTime</span></span>| <span data-ttu-id="f4ea1-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ea1-113">DateTimeOffset</span></span> |<span data-ttu-id="f4ea1-114">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-114">The start time of the operation.</span></span>|
|<span data-ttu-id="f4ea1-115">erro</span><span class="sxs-lookup"><span data-stu-id="f4ea1-115">error</span></span>|[<span data-ttu-id="f4ea1-116">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="f4ea1-116">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="f4ea1-117">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-117">The error returned by the operation.</span></span>|
|<span data-ttu-id="f4ea1-118">id</span><span class="sxs-lookup"><span data-stu-id="f4ea1-118">id</span></span>|<span data-ttu-id="f4ea1-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4ea1-119">string</span></span>|<span data-ttu-id="f4ea1-120">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-120">The operation id. Read-only.</span></span>|
|<span data-ttu-id="f4ea1-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f4ea1-121">lastActionDateTime</span></span>| <span data-ttu-id="f4ea1-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4ea1-122">DateTimeOffset</span></span> |<span data-ttu-id="f4ea1-123">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-123">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="f4ea1-124">resourceId</span><span class="sxs-lookup"><span data-stu-id="f4ea1-124">resourceId</span></span>|<span data-ttu-id="f4ea1-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4ea1-125">string</span></span>|<span data-ttu-id="f4ea1-126">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-126">The resource id.</span></span>|
|<span data-ttu-id="f4ea1-127">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="f4ea1-127">resourceLocation</span></span>|<span data-ttu-id="f4ea1-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4ea1-128">string</span></span>|<span data-ttu-id="f4ea1-129">O URI do recurso para o objeto.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-129">The resource URI for the object.</span></span> <span data-ttu-id="f4ea1-130">Por exemplo, o URI do recurso para uma página ou seção copiada.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-130">For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="f4ea1-131">status</span><span class="sxs-lookup"><span data-stu-id="f4ea1-131">status</span></span>|<span data-ttu-id="f4ea1-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4ea1-132">string</span></span>|<span data-ttu-id="f4ea1-133">O status atual da operação: `notstarted` , `running` , `completed` ,`failed`</span><span class="sxs-lookup"><span data-stu-id="f4ea1-133">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="f4ea1-134">percentComplete</span><span class="sxs-lookup"><span data-stu-id="f4ea1-134">percentComplete</span></span>|<span data-ttu-id="f4ea1-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4ea1-135">string</span></span>|<span data-ttu-id="f4ea1-136">A porcentagem concluída da operação se a operação ainda estiver em `running` status</span><span class="sxs-lookup"><span data-stu-id="f4ea1-136">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="f4ea1-137">Relações</span><span class="sxs-lookup"><span data-stu-id="f4ea1-137">Relationships</span></span>
<span data-ttu-id="f4ea1-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f4ea1-138">None</span></span>


## <a name="methods"></a><span data-ttu-id="f4ea1-139">Métodos</span><span class="sxs-lookup"><span data-stu-id="f4ea1-139">Methods</span></span>

| <span data-ttu-id="f4ea1-140">Método</span><span class="sxs-lookup"><span data-stu-id="f4ea1-140">Method</span></span>           | <span data-ttu-id="f4ea1-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4ea1-141">Return Type</span></span>    |<span data-ttu-id="f4ea1-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ea1-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4ea1-143">Operação get</span><span class="sxs-lookup"><span data-stu-id="f4ea1-143">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="f4ea1-144">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="f4ea1-144">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="f4ea1-145">Obter o status da operação.</span><span class="sxs-lookup"><span data-stu-id="f4ea1-145">Get the status of the operation.</span></span> |

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
