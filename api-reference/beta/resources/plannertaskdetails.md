---
title: tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto Task tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: df870a8512536b0e29a923a52c62a2b779a180e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063996"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="68161-104">tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="68161-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="68161-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68161-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68161-106">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="68161-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="68161-107">Cada objeto [Task](plannertask.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="68161-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="68161-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="68161-108">Methods</span></span>

| <span data-ttu-id="68161-109">Método</span><span class="sxs-lookup"><span data-stu-id="68161-109">Method</span></span>           | <span data-ttu-id="68161-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68161-110">Return Type</span></span>    |<span data-ttu-id="68161-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="68161-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68161-112">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="68161-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="68161-113">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="68161-113">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="68161-114">Leia as propriedades e os relacionamentos do objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="68161-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="68161-115">Update</span><span class="sxs-lookup"><span data-stu-id="68161-115">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="68161-116">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="68161-116">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="68161-117">Atualize o objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="68161-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="68161-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68161-118">Properties</span></span>
| <span data-ttu-id="68161-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68161-119">Property</span></span>     | <span data-ttu-id="68161-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="68161-120">Type</span></span>   |<span data-ttu-id="68161-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="68161-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68161-122">verificação</span><span class="sxs-lookup"><span data-stu-id="68161-122">checklist</span></span>|[<span data-ttu-id="68161-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="68161-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="68161-124">A coleção de itens de lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="68161-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="68161-125">description</span><span class="sxs-lookup"><span data-stu-id="68161-125">description</span></span>|<span data-ttu-id="68161-126">String</span><span class="sxs-lookup"><span data-stu-id="68161-126">String</span></span>|<span data-ttu-id="68161-127">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="68161-127">Description of the task</span></span>|
|<span data-ttu-id="68161-128">id</span><span class="sxs-lookup"><span data-stu-id="68161-128">id</span></span>|<span data-ttu-id="68161-129">String</span><span class="sxs-lookup"><span data-stu-id="68161-129">String</span></span>| <span data-ttu-id="68161-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68161-130">Read-only.</span></span> <span data-ttu-id="68161-131">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="68161-131">ID of the task details.</span></span> <span data-ttu-id="68161-132">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="68161-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="68161-133">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="68161-133">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="68161-134">previewType</span><span class="sxs-lookup"><span data-stu-id="68161-134">previewType</span></span>|<span data-ttu-id="68161-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68161-135">string</span></span>|<span data-ttu-id="68161-136">Isso define o tipo de visualização que aparece na tarefa.</span><span class="sxs-lookup"><span data-stu-id="68161-136">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="68161-137">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="68161-137">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="68161-138">Quando definido para `automatic` a visualização exibida é escolhido pelo aplicativo que está exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="68161-138">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="68161-139">Referencie</span><span class="sxs-lookup"><span data-stu-id="68161-139">references</span></span>|[<span data-ttu-id="68161-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="68161-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="68161-141">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="68161-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68161-142">Relações</span><span class="sxs-lookup"><span data-stu-id="68161-142">Relationships</span></span>
<span data-ttu-id="68161-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68161-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="68161-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68161-144">JSON representation</span></span>
<span data-ttu-id="68161-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68161-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


