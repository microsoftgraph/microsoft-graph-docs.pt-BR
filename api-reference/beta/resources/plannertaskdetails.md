---
title: tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto Task tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d11b0ca1f6090c65a1c5eaa45ce368d102994299
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344361"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="d8984-104">tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d8984-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8984-105">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="d8984-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="d8984-106">Cada objeto [Task](plannertask.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="d8984-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="d8984-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8984-107">Methods</span></span>

| <span data-ttu-id="d8984-108">Método</span><span class="sxs-lookup"><span data-stu-id="d8984-108">Method</span></span>           | <span data-ttu-id="d8984-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8984-109">Return Type</span></span>    |<span data-ttu-id="d8984-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8984-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8984-111">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d8984-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="d8984-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d8984-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="d8984-113">Leia as propriedades e os relacionamentos do objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="d8984-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="d8984-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d8984-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="d8984-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d8984-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="d8984-116">Atualize o objeto **plannerTaskDetails** .</span><span class="sxs-lookup"><span data-stu-id="d8984-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d8984-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8984-117">Properties</span></span>
| <span data-ttu-id="d8984-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8984-118">Property</span></span>     | <span data-ttu-id="d8984-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8984-119">Type</span></span>   |<span data-ttu-id="d8984-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8984-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8984-121">verificação</span><span class="sxs-lookup"><span data-stu-id="d8984-121">checklist</span></span>|[<span data-ttu-id="d8984-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="d8984-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="d8984-123">A coleção de itens de lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="d8984-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="d8984-124">description</span><span class="sxs-lookup"><span data-stu-id="d8984-124">description</span></span>|<span data-ttu-id="d8984-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8984-125">String</span></span>|<span data-ttu-id="d8984-126">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="d8984-126">Description of the task</span></span>|
|<span data-ttu-id="d8984-127">id</span><span class="sxs-lookup"><span data-stu-id="d8984-127">id</span></span>|<span data-ttu-id="d8984-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8984-128">String</span></span>| <span data-ttu-id="d8984-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8984-129">Read-only.</span></span> <span data-ttu-id="d8984-130">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="d8984-130">ID of the task details.</span></span> <span data-ttu-id="d8984-131">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d8984-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d8984-132">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="d8984-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d8984-133">previewType</span><span class="sxs-lookup"><span data-stu-id="d8984-133">previewType</span></span>|<span data-ttu-id="d8984-134">string</span><span class="sxs-lookup"><span data-stu-id="d8984-134">string</span></span>|<span data-ttu-id="d8984-135">Isso define o tipo de visualização que aparece na tarefa.</span><span class="sxs-lookup"><span data-stu-id="d8984-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="d8984-136">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="d8984-136">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="d8984-137">Quando definido para `automatic` a visualização exibida é escolhido pelo aplicativo que está exibindo a tarefa.</span><span class="sxs-lookup"><span data-stu-id="d8984-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="d8984-138">Referencie</span><span class="sxs-lookup"><span data-stu-id="d8984-138">references</span></span>|[<span data-ttu-id="d8984-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="d8984-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="d8984-140">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="d8984-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8984-141">Relações</span><span class="sxs-lookup"><span data-stu-id="d8984-141">Relationships</span></span>
<span data-ttu-id="d8984-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8984-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d8984-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8984-143">JSON representation</span></span>
<span data-ttu-id="d8984-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8984-144">Here is a JSON representation of the resource.</span></span>

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
