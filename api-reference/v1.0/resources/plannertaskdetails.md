---
title: tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto Task tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75e17200dc52fff385c7be8fb0269a3da20464b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534322"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="80515-104">tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="80515-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="80515-105">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="80515-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="80515-106">Cada objeto [Task](plannertask.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="80515-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="80515-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="80515-107">Methods</span></span>

| <span data-ttu-id="80515-108">Método</span><span class="sxs-lookup"><span data-stu-id="80515-108">Method</span></span>           | <span data-ttu-id="80515-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="80515-109">Return Type</span></span>    |<span data-ttu-id="80515-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="80515-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80515-111">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="80515-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="80515-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="80515-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="80515-113">Leia as propriedades e os relacionamentos do objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="80515-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="80515-114">Update</span><span class="sxs-lookup"><span data-stu-id="80515-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="80515-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="80515-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="80515-116">Atualize o objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="80515-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80515-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80515-117">Properties</span></span>
| <span data-ttu-id="80515-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80515-118">Property</span></span>     | <span data-ttu-id="80515-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="80515-119">Type</span></span>   |<span data-ttu-id="80515-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="80515-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80515-121">verificação</span><span class="sxs-lookup"><span data-stu-id="80515-121">checklist</span></span>|[<span data-ttu-id="80515-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="80515-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="80515-123">A coleção de itens de lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="80515-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="80515-124">description</span><span class="sxs-lookup"><span data-stu-id="80515-124">description</span></span>|<span data-ttu-id="80515-125">String</span><span class="sxs-lookup"><span data-stu-id="80515-125">String</span></span>|<span data-ttu-id="80515-126">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="80515-126">Description of the task</span></span>|
|<span data-ttu-id="80515-127">id</span><span class="sxs-lookup"><span data-stu-id="80515-127">id</span></span>|<span data-ttu-id="80515-128">String</span><span class="sxs-lookup"><span data-stu-id="80515-128">String</span></span>| <span data-ttu-id="80515-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80515-129">Read-only.</span></span> <span data-ttu-id="80515-130">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="80515-130">ID of the task details.</span></span> <span data-ttu-id="80515-131">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="80515-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="80515-132">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="80515-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="80515-133">previewType</span><span class="sxs-lookup"><span data-stu-id="80515-133">previewType</span></span>|<span data-ttu-id="80515-134">string</span><span class="sxs-lookup"><span data-stu-id="80515-134">string</span></span>|<span data-ttu-id="80515-135">Isso define o tipo de visualização que aparece na tarefa.</span><span class="sxs-lookup"><span data-stu-id="80515-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="80515-136">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="80515-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="80515-137">Quando definido para `automatic` a visualização exibida é escolhido pelo aplicativo que está exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="80515-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="80515-138">Referencie</span><span class="sxs-lookup"><span data-stu-id="80515-138">references</span></span>|[<span data-ttu-id="80515-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="80515-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="80515-140">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="80515-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80515-141">Relações</span><span class="sxs-lookup"><span data-stu-id="80515-141">Relationships</span></span>
<span data-ttu-id="80515-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80515-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="80515-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80515-143">JSON representation</span></span>
<span data-ttu-id="80515-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80515-144">Here is a JSON representation of the resource.</span></span>

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
