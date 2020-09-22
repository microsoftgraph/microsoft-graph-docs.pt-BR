---
title: tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto Task tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 32ea3fff1c97920a83f667282e1341926a02b5c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037371"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="2b2c7-104">tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="2b2c7-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="2b2c7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b2c7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b2c7-106">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="2b2c7-107">Cada objeto [Task](plannertask.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="2b2c7-108">Methods</span><span class="sxs-lookup"><span data-stu-id="2b2c7-108">Methods</span></span>

| <span data-ttu-id="2b2c7-109">Método</span><span class="sxs-lookup"><span data-stu-id="2b2c7-109">Method</span></span>           | <span data-ttu-id="2b2c7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2b2c7-110">Return Type</span></span>    |<span data-ttu-id="2b2c7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b2c7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b2c7-112">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="2b2c7-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="2b2c7-113">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="2b2c7-113">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="2b2c7-114">Leia as propriedades e os relacionamentos do objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="2b2c7-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="2b2c7-115">Atualização</span><span class="sxs-lookup"><span data-stu-id="2b2c7-115">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="2b2c7-116">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="2b2c7-116">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="2b2c7-117">Atualize o objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="2b2c7-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2b2c7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b2c7-118">Properties</span></span>
| <span data-ttu-id="2b2c7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b2c7-119">Property</span></span>     | <span data-ttu-id="2b2c7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b2c7-120">Type</span></span>   |<span data-ttu-id="2b2c7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b2c7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b2c7-122">verificação</span><span class="sxs-lookup"><span data-stu-id="2b2c7-122">checklist</span></span>|[<span data-ttu-id="2b2c7-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="2b2c7-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="2b2c7-124">A coleção de itens de lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="2b2c7-125">description</span><span class="sxs-lookup"><span data-stu-id="2b2c7-125">description</span></span>|<span data-ttu-id="2b2c7-126">String</span><span class="sxs-lookup"><span data-stu-id="2b2c7-126">String</span></span>|<span data-ttu-id="2b2c7-127">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="2b2c7-127">Description of the task</span></span>|
|<span data-ttu-id="2b2c7-128">id</span><span class="sxs-lookup"><span data-stu-id="2b2c7-128">id</span></span>|<span data-ttu-id="2b2c7-129">String</span><span class="sxs-lookup"><span data-stu-id="2b2c7-129">String</span></span>| <span data-ttu-id="2b2c7-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-130">Read-only.</span></span> <span data-ttu-id="2b2c7-131">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-131">ID of the task details.</span></span> <span data-ttu-id="2b2c7-132">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2b2c7-133">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-133">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="2b2c7-134">previewType</span><span class="sxs-lookup"><span data-stu-id="2b2c7-134">previewType</span></span>|<span data-ttu-id="2b2c7-135">string</span><span class="sxs-lookup"><span data-stu-id="2b2c7-135">string</span></span>|<span data-ttu-id="2b2c7-136">Isso define o tipo de visualização que aparece na tarefa.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-136">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="2b2c7-137">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-137">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="2b2c7-138">Quando definido para `automatic` a visualização exibida é escolhido pelo aplicativo que está exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-138">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="2b2c7-139">Referencie</span><span class="sxs-lookup"><span data-stu-id="2b2c7-139">references</span></span>|[<span data-ttu-id="2b2c7-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="2b2c7-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="2b2c7-141">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b2c7-142">Relações</span><span class="sxs-lookup"><span data-stu-id="2b2c7-142">Relationships</span></span>
<span data-ttu-id="2b2c7-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b2c7-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2b2c7-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b2c7-144">JSON representation</span></span>
<span data-ttu-id="2b2c7-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b2c7-145">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

