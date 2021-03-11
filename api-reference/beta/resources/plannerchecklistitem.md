---
title: Tipo de recurso plannerChecklistItem
description: O **recurso plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo objeto checklistItems.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5702e7a8c34c9ca0b996f437a65409371e8f3c98
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721002"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="6d41d-104">Tipo de recurso plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="6d41d-104">plannerChecklistItem resource type</span></span>

<span data-ttu-id="6d41d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d41d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d41d-106">O **recurso plannerChecklistItem** representa um item na lista de verificação de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="6d41d-106">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="6d41d-107">A lista de verificação em uma tarefa é representada pelo [objeto checklistItems](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="6d41d-107">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="6d41d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d41d-108">Properties</span></span>
| <span data-ttu-id="6d41d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d41d-109">Property</span></span>     | <span data-ttu-id="6d41d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d41d-110">Type</span></span>   |<span data-ttu-id="6d41d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d41d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d41d-112">isChecked</span><span class="sxs-lookup"><span data-stu-id="6d41d-112">isChecked</span></span>|<span data-ttu-id="6d41d-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d41d-113">Boolean</span></span>|<span data-ttu-id="6d41d-114">O valor `true` é se o item for verificado e caso `false` contrário.</span><span class="sxs-lookup"><span data-stu-id="6d41d-114">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="6d41d-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6d41d-115">lastModifiedBy</span></span>|[<span data-ttu-id="6d41d-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d41d-116">identitySet</span></span>](identityset.md)| <span data-ttu-id="6d41d-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d41d-117">Read-only.</span></span> <span data-ttu-id="6d41d-118">ID do usuário pela qual foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6d41d-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="6d41d-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d41d-119">lastModifiedDateTime</span></span>|<span data-ttu-id="6d41d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d41d-120">DateTimeOffset</span></span>|<span data-ttu-id="6d41d-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d41d-121">Read-only.</span></span> <span data-ttu-id="6d41d-122">Data e hora em que isso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6d41d-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="6d41d-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6d41d-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d41d-124">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="6d41d-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6d41d-125">orderHint</span><span class="sxs-lookup"><span data-stu-id="6d41d-125">orderHint</span></span>|<span data-ttu-id="6d41d-126">String</span><span class="sxs-lookup"><span data-stu-id="6d41d-126">String</span></span>|<span data-ttu-id="6d41d-127">Usado para definir a ordem relativa de itens na lista de verificação.</span><span class="sxs-lookup"><span data-stu-id="6d41d-127">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="6d41d-128">O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="6d41d-128">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="6d41d-129">title</span><span class="sxs-lookup"><span data-stu-id="6d41d-129">title</span></span>|<span data-ttu-id="6d41d-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d41d-130">String</span></span>|<span data-ttu-id="6d41d-131">Título do item de lista de verificação</span><span class="sxs-lookup"><span data-stu-id="6d41d-131">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d41d-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d41d-132">JSON representation</span></span>
<span data-ttu-id="6d41d-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d41d-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


