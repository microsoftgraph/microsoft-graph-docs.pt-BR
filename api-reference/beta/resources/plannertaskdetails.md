---
title: Tipo de recurso plannerTaskDetails
description: O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto task tem um objeto de detalhes.
localization_priority: Normal
ms.openlocfilehash: 0bec5b47d1472eae43906841c5074e4080672817
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888162"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="6219d-104">Tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6219d-104">plannerTaskDetails resource type</span></span>

> <span data-ttu-id="6219d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6219d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6219d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6219d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6219d-p103">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="6219d-p103">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="6219d-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="6219d-109">Methods</span></span>

| <span data-ttu-id="6219d-110">Método</span><span class="sxs-lookup"><span data-stu-id="6219d-110">Method</span></span>           | <span data-ttu-id="6219d-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6219d-111">Return Type</span></span>    |<span data-ttu-id="6219d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6219d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6219d-113">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6219d-113">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="6219d-114">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6219d-114">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="6219d-115">Leia as propriedades e as relações do objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="6219d-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="6219d-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6219d-116">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="6219d-117">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6219d-117">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="6219d-118">Atualize o objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="6219d-118">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6219d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6219d-119">Properties</span></span>
| <span data-ttu-id="6219d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6219d-120">Property</span></span>     | <span data-ttu-id="6219d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6219d-121">Type</span></span>   |<span data-ttu-id="6219d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6219d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6219d-123">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="6219d-123">checklist</span></span>|[<span data-ttu-id="6219d-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="6219d-124">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="6219d-125">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="6219d-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="6219d-126">description</span><span class="sxs-lookup"><span data-stu-id="6219d-126">description</span></span>|<span data-ttu-id="6219d-127">String</span><span class="sxs-lookup"><span data-stu-id="6219d-127">String</span></span>|<span data-ttu-id="6219d-128">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="6219d-128">Description of the task</span></span>|
|<span data-ttu-id="6219d-129">id</span><span class="sxs-lookup"><span data-stu-id="6219d-129">id</span></span>|<span data-ttu-id="6219d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6219d-130">String</span></span>| <span data-ttu-id="6219d-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6219d-131">Read-only.</span></span> <span data-ttu-id="6219d-132">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="6219d-132">ID of the task details.</span></span> <span data-ttu-id="6219d-133">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="6219d-133">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="6219d-134">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="6219d-134">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6219d-135">previewType</span><span class="sxs-lookup"><span data-stu-id="6219d-135">previewType</span></span>|<span data-ttu-id="6219d-136">string</span><span class="sxs-lookup"><span data-stu-id="6219d-136">string</span></span>|<span data-ttu-id="6219d-p105">Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.</span><span class="sxs-lookup"><span data-stu-id="6219d-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="6219d-140">referências</span><span class="sxs-lookup"><span data-stu-id="6219d-140">references</span></span>|[<span data-ttu-id="6219d-141">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="6219d-141">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="6219d-142">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="6219d-142">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6219d-143">Relações</span><span class="sxs-lookup"><span data-stu-id="6219d-143">Relationships</span></span>
<span data-ttu-id="6219d-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6219d-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6219d-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6219d-145">JSON representation</span></span>
<span data-ttu-id="6219d-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6219d-146">Here is a JSON representation of the resource.</span></span>

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
