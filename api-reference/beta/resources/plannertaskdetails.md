---
title: Tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto task tem um objeto de detalhes.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 84b7191822be56e881b31d99503fdcdc4097890c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941139"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="82ce6-104">Tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="82ce6-104">plannerTaskDetails resource type</span></span>

> <span data-ttu-id="82ce6-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="82ce6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82ce6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="82ce6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82ce6-p103">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="82ce6-p103">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="82ce6-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="82ce6-109">Methods</span></span>

| <span data-ttu-id="82ce6-110">Método</span><span class="sxs-lookup"><span data-stu-id="82ce6-110">Method</span></span>           | <span data-ttu-id="82ce6-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="82ce6-111">Return Type</span></span>    |<span data-ttu-id="82ce6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ce6-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82ce6-113">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="82ce6-113">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="82ce6-114">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="82ce6-114">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="82ce6-115">Leia as propriedades e as relações do objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="82ce6-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="82ce6-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="82ce6-116">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="82ce6-117">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="82ce6-117">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="82ce6-118">Atualize o objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="82ce6-118">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="82ce6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82ce6-119">Properties</span></span>
| <span data-ttu-id="82ce6-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82ce6-120">Property</span></span>     | <span data-ttu-id="82ce6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="82ce6-121">Type</span></span>   |<span data-ttu-id="82ce6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ce6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82ce6-123">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="82ce6-123">checklist</span></span>|[<span data-ttu-id="82ce6-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="82ce6-124">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="82ce6-125">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="82ce6-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="82ce6-126">description</span><span class="sxs-lookup"><span data-stu-id="82ce6-126">description</span></span>|<span data-ttu-id="82ce6-127">String</span><span class="sxs-lookup"><span data-stu-id="82ce6-127">String</span></span>|<span data-ttu-id="82ce6-128">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="82ce6-128">Description of the task</span></span>|
|<span data-ttu-id="82ce6-129">id</span><span class="sxs-lookup"><span data-stu-id="82ce6-129">id</span></span>|<span data-ttu-id="82ce6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82ce6-130">String</span></span>| <span data-ttu-id="82ce6-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82ce6-131">Read-only.</span></span> <span data-ttu-id="82ce6-132">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="82ce6-132">ID of the task details.</span></span> <span data-ttu-id="82ce6-133">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="82ce6-133">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="82ce6-134">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="82ce6-134">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="82ce6-135">previewType</span><span class="sxs-lookup"><span data-stu-id="82ce6-135">previewType</span></span>|<span data-ttu-id="82ce6-136">string</span><span class="sxs-lookup"><span data-stu-id="82ce6-136">string</span></span>|<span data-ttu-id="82ce6-p105">Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.</span><span class="sxs-lookup"><span data-stu-id="82ce6-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="82ce6-140">referências</span><span class="sxs-lookup"><span data-stu-id="82ce6-140">references</span></span>|[<span data-ttu-id="82ce6-141">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="82ce6-141">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="82ce6-142">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="82ce6-142">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82ce6-143">Relações</span><span class="sxs-lookup"><span data-stu-id="82ce6-143">Relationships</span></span>
<span data-ttu-id="82ce6-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82ce6-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="82ce6-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82ce6-145">JSON representation</span></span>
<span data-ttu-id="82ce6-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82ce6-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
