---
title: Tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto task tem um objeto de detalhes.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512308"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="6975f-104">Tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6975f-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6975f-p102">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="6975f-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="6975f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6975f-107">Methods</span></span>

| <span data-ttu-id="6975f-108">Método</span><span class="sxs-lookup"><span data-stu-id="6975f-108">Method</span></span>           | <span data-ttu-id="6975f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6975f-109">Return Type</span></span>    |<span data-ttu-id="6975f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6975f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6975f-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6975f-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="6975f-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6975f-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="6975f-113">Leia as propriedades e as relações do objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="6975f-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="6975f-114">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6975f-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="6975f-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6975f-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="6975f-116">Atualize o objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="6975f-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6975f-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6975f-117">Properties</span></span>
| <span data-ttu-id="6975f-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6975f-118">Property</span></span>     | <span data-ttu-id="6975f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6975f-119">Type</span></span>   |<span data-ttu-id="6975f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6975f-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6975f-121">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="6975f-121">checklist</span></span>|[<span data-ttu-id="6975f-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="6975f-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="6975f-123">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="6975f-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="6975f-124">description</span><span class="sxs-lookup"><span data-stu-id="6975f-124">description</span></span>|<span data-ttu-id="6975f-125">String</span><span class="sxs-lookup"><span data-stu-id="6975f-125">String</span></span>|<span data-ttu-id="6975f-126">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="6975f-126">Description of the task</span></span>|
|<span data-ttu-id="6975f-127">id</span><span class="sxs-lookup"><span data-stu-id="6975f-127">id</span></span>|<span data-ttu-id="6975f-128">String</span><span class="sxs-lookup"><span data-stu-id="6975f-128">String</span></span>| <span data-ttu-id="6975f-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6975f-129">Read-only.</span></span> <span data-ttu-id="6975f-130">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="6975f-130">ID of the task details.</span></span> <span data-ttu-id="6975f-131">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="6975f-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="6975f-132">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="6975f-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6975f-133">previewType</span><span class="sxs-lookup"><span data-stu-id="6975f-133">previewType</span></span>|<span data-ttu-id="6975f-134">string</span><span class="sxs-lookup"><span data-stu-id="6975f-134">string</span></span>|<span data-ttu-id="6975f-p104">Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.</span><span class="sxs-lookup"><span data-stu-id="6975f-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="6975f-138">referências</span><span class="sxs-lookup"><span data-stu-id="6975f-138">references</span></span>|[<span data-ttu-id="6975f-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="6975f-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="6975f-140">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="6975f-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6975f-141">Relações</span><span class="sxs-lookup"><span data-stu-id="6975f-141">Relationships</span></span>
<span data-ttu-id="6975f-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6975f-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6975f-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6975f-143">JSON representation</span></span>
<span data-ttu-id="6975f-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6975f-144">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertaskdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
