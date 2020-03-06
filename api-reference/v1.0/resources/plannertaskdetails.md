---
title: tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto Task tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4dda174401ebf3435c7a190a3f92167ac6b47c0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533971"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="d67cf-104">tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d67cf-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="d67cf-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d67cf-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d67cf-106">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="d67cf-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="d67cf-107">Cada objeto [Task](plannertask.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="d67cf-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="d67cf-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d67cf-108">Methods</span></span>

| <span data-ttu-id="d67cf-109">Método</span><span class="sxs-lookup"><span data-stu-id="d67cf-109">Method</span></span>           | <span data-ttu-id="d67cf-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d67cf-110">Return Type</span></span>    |<span data-ttu-id="d67cf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d67cf-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d67cf-112">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d67cf-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="d67cf-113">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d67cf-113">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="d67cf-114">Leia as propriedades e os relacionamentos do objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="d67cf-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="d67cf-115">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d67cf-115">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="d67cf-116">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d67cf-116">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="d67cf-117">Atualize o objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="d67cf-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d67cf-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d67cf-118">Properties</span></span>
| <span data-ttu-id="d67cf-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d67cf-119">Property</span></span>     | <span data-ttu-id="d67cf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d67cf-120">Type</span></span>   |<span data-ttu-id="d67cf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d67cf-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d67cf-122">verificação</span><span class="sxs-lookup"><span data-stu-id="d67cf-122">checklist</span></span>|[<span data-ttu-id="d67cf-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="d67cf-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="d67cf-124">A coleção de itens de lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="d67cf-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="d67cf-125">description</span><span class="sxs-lookup"><span data-stu-id="d67cf-125">description</span></span>|<span data-ttu-id="d67cf-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d67cf-126">String</span></span>|<span data-ttu-id="d67cf-127">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="d67cf-127">Description of the task</span></span>|
|<span data-ttu-id="d67cf-128">id</span><span class="sxs-lookup"><span data-stu-id="d67cf-128">id</span></span>|<span data-ttu-id="d67cf-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d67cf-129">String</span></span>| <span data-ttu-id="d67cf-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d67cf-130">Read-only.</span></span> <span data-ttu-id="d67cf-131">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="d67cf-131">ID of the task details.</span></span> <span data-ttu-id="d67cf-132">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d67cf-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d67cf-133">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="d67cf-133">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d67cf-134">previewType</span><span class="sxs-lookup"><span data-stu-id="d67cf-134">previewType</span></span>|<span data-ttu-id="d67cf-135">string</span><span class="sxs-lookup"><span data-stu-id="d67cf-135">string</span></span>|<span data-ttu-id="d67cf-136">Isso define o tipo de visualização que aparece na tarefa.</span><span class="sxs-lookup"><span data-stu-id="d67cf-136">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="d67cf-137">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="d67cf-137">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="d67cf-138">Quando definido para `automatic` a visualização exibida é escolhido pelo aplicativo que está exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="d67cf-138">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="d67cf-139">Referencie</span><span class="sxs-lookup"><span data-stu-id="d67cf-139">references</span></span>|[<span data-ttu-id="d67cf-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="d67cf-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="d67cf-141">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="d67cf-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d67cf-142">Relações</span><span class="sxs-lookup"><span data-stu-id="d67cf-142">Relationships</span></span>
<span data-ttu-id="d67cf-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d67cf-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d67cf-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d67cf-144">JSON representation</span></span>
<span data-ttu-id="d67cf-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d67cf-145">Here is a JSON representation of the resource.</span></span>

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
