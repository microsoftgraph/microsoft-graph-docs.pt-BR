---
title: tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto Task tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d22c932989b9c0d21350842babd9b4bbf420124c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035165"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="86b82-104">tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="86b82-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="86b82-105">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="86b82-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="86b82-106">Cada objeto [Task](plannertask.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="86b82-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="86b82-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="86b82-107">Methods</span></span>

| <span data-ttu-id="86b82-108">Método</span><span class="sxs-lookup"><span data-stu-id="86b82-108">Method</span></span>           | <span data-ttu-id="86b82-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86b82-109">Return Type</span></span>    |<span data-ttu-id="86b82-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="86b82-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86b82-111">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="86b82-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="86b82-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="86b82-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="86b82-113">Leia as propriedades e os relacionamentos do objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="86b82-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="86b82-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="86b82-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="86b82-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="86b82-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="86b82-116">Atualize o objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="86b82-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="86b82-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86b82-117">Properties</span></span>
| <span data-ttu-id="86b82-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86b82-118">Property</span></span>     | <span data-ttu-id="86b82-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="86b82-119">Type</span></span>   |<span data-ttu-id="86b82-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="86b82-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86b82-121">verificação</span><span class="sxs-lookup"><span data-stu-id="86b82-121">checklist</span></span>|[<span data-ttu-id="86b82-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="86b82-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="86b82-123">A coleção de itens de lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="86b82-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="86b82-124">descrição</span><span class="sxs-lookup"><span data-stu-id="86b82-124">description</span></span>|<span data-ttu-id="86b82-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b82-125">String</span></span>|<span data-ttu-id="86b82-126">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="86b82-126">Description of the task</span></span>|
|<span data-ttu-id="86b82-127">id</span><span class="sxs-lookup"><span data-stu-id="86b82-127">id</span></span>|<span data-ttu-id="86b82-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86b82-128">String</span></span>| <span data-ttu-id="86b82-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86b82-129">Read-only.</span></span> <span data-ttu-id="86b82-130">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="86b82-130">ID of the task details.</span></span> <span data-ttu-id="86b82-131">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="86b82-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="86b82-132">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="86b82-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="86b82-133">previewType</span><span class="sxs-lookup"><span data-stu-id="86b82-133">previewType</span></span>|<span data-ttu-id="86b82-134">string</span><span class="sxs-lookup"><span data-stu-id="86b82-134">string</span></span>|<span data-ttu-id="86b82-135">Isso define o tipo de visualização que aparece na tarefa.</span><span class="sxs-lookup"><span data-stu-id="86b82-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="86b82-136">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="86b82-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="86b82-137">Quando definido para `automatic` a visualização exibida é escolhido pelo aplicativo que está exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="86b82-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="86b82-138">Referencie</span><span class="sxs-lookup"><span data-stu-id="86b82-138">references</span></span>|[<span data-ttu-id="86b82-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="86b82-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="86b82-140">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="86b82-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86b82-141">Relações</span><span class="sxs-lookup"><span data-stu-id="86b82-141">Relationships</span></span>
<span data-ttu-id="86b82-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86b82-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="86b82-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86b82-143">JSON representation</span></span>
<span data-ttu-id="86b82-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86b82-144">Here is a JSON representation of the resource.</span></span>

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
