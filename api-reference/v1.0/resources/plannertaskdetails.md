---
title: Tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto task tem um objeto de detalhes.
ms.openlocfilehash: 74ba1c5b7c607f30253463e6cfc256fd3119bf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007236"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="0255e-104">Tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0255e-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="0255e-p102">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="0255e-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="0255e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0255e-107">Methods</span></span>

| <span data-ttu-id="0255e-108">Método</span><span class="sxs-lookup"><span data-stu-id="0255e-108">Method</span></span>           | <span data-ttu-id="0255e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0255e-109">Return Type</span></span>    |<span data-ttu-id="0255e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0255e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0255e-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0255e-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="0255e-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0255e-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="0255e-113">Leia as propriedades e as relações do objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="0255e-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="0255e-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="0255e-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="0255e-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0255e-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="0255e-116">Atualize o objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="0255e-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0255e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0255e-117">Properties</span></span>
| <span data-ttu-id="0255e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0255e-118">Property</span></span>     | <span data-ttu-id="0255e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0255e-119">Type</span></span>   |<span data-ttu-id="0255e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0255e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0255e-121">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="0255e-121">checklist</span></span>|[<span data-ttu-id="0255e-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="0255e-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="0255e-123">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="0255e-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="0255e-124">description</span><span class="sxs-lookup"><span data-stu-id="0255e-124">description</span></span>|<span data-ttu-id="0255e-125">String</span><span class="sxs-lookup"><span data-stu-id="0255e-125">String</span></span>|<span data-ttu-id="0255e-126">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="0255e-126">Description of the task</span></span>|
|<span data-ttu-id="0255e-127">id</span><span class="sxs-lookup"><span data-stu-id="0255e-127">id</span></span>|<span data-ttu-id="0255e-128">String</span><span class="sxs-lookup"><span data-stu-id="0255e-128">String</span></span>| <span data-ttu-id="0255e-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0255e-129">Read-only.</span></span> <span data-ttu-id="0255e-130">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="0255e-130">ID of the task details.</span></span> <span data-ttu-id="0255e-131">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="0255e-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0255e-132">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="0255e-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="0255e-133">previewType</span><span class="sxs-lookup"><span data-stu-id="0255e-133">previewType</span></span>|<span data-ttu-id="0255e-134">string</span><span class="sxs-lookup"><span data-stu-id="0255e-134">string</span></span>|<span data-ttu-id="0255e-135">Isto define o tipo de visualização que aparecerá na tarefa.</span><span class="sxs-lookup"><span data-stu-id="0255e-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="0255e-136">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="0255e-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="0255e-137">Quando definido como `automatic` a visualização exibida for escolhida pelo app exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="0255e-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="0255e-138">referências</span><span class="sxs-lookup"><span data-stu-id="0255e-138">references</span></span>|[<span data-ttu-id="0255e-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="0255e-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="0255e-140">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="0255e-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0255e-141">Relações</span><span class="sxs-lookup"><span data-stu-id="0255e-141">Relationships</span></span>
<span data-ttu-id="0255e-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0255e-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0255e-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0255e-143">JSON representation</span></span>
<span data-ttu-id="0255e-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0255e-144">Here is a JSON representation of the resource.</span></span>

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
