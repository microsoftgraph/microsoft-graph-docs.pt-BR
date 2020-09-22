---
title: tipo de recurso plannerChecklistItem
description: O recurso **plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo objeto checklistItems.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3c60b2727af2fccfdac8e8f9e60e055b0471c861
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046801"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="3703a-104">tipo de recurso plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="3703a-104">plannerChecklistItem resource type</span></span>

<span data-ttu-id="3703a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3703a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3703a-106">O recurso **plannerChecklistItem** representa um item na lista de verificação de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="3703a-106">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="3703a-107">A lista de verificação em uma tarefa é representada pelo [objeto checklistItems](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="3703a-107">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="3703a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3703a-108">Properties</span></span>
| <span data-ttu-id="3703a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3703a-109">Property</span></span>     | <span data-ttu-id="3703a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3703a-110">Type</span></span>   |<span data-ttu-id="3703a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3703a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3703a-112">IsChecked</span><span class="sxs-lookup"><span data-stu-id="3703a-112">isChecked</span></span>|<span data-ttu-id="3703a-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="3703a-113">Boolean</span></span>|<span data-ttu-id="3703a-114">Value é `true` se o item estiver marcado e `false` , caso contrário.</span><span class="sxs-lookup"><span data-stu-id="3703a-114">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="3703a-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3703a-115">lastModifiedBy</span></span>|[<span data-ttu-id="3703a-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="3703a-116">identitySet</span></span>](identityset.md)| <span data-ttu-id="3703a-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3703a-117">Read-only.</span></span> <span data-ttu-id="3703a-118">ID de usuário pela qual esta foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3703a-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="3703a-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3703a-119">lastModifiedDateTime</span></span>|<span data-ttu-id="3703a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3703a-120">DateTimeOffset</span></span>|<span data-ttu-id="3703a-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3703a-121">Read-only.</span></span> <span data-ttu-id="3703a-122">Data e hora da última modificação.</span><span class="sxs-lookup"><span data-stu-id="3703a-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="3703a-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3703a-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3703a-124">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3703a-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3703a-125">orderHint</span><span class="sxs-lookup"><span data-stu-id="3703a-125">orderHint</span></span>|<span data-ttu-id="3703a-126">String</span><span class="sxs-lookup"><span data-stu-id="3703a-126">String</span></span>|<span data-ttu-id="3703a-127">Usado para definir a ordem relativa dos itens na lista de verificação.</span><span class="sxs-lookup"><span data-stu-id="3703a-127">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="3703a-128">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="3703a-128">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="3703a-129">title</span><span class="sxs-lookup"><span data-stu-id="3703a-129">title</span></span>|<span data-ttu-id="3703a-130">String</span><span class="sxs-lookup"><span data-stu-id="3703a-130">String</span></span>|<span data-ttu-id="3703a-131">Título do item de lista de verificação</span><span class="sxs-lookup"><span data-stu-id="3703a-131">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3703a-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3703a-132">JSON representation</span></span>
<span data-ttu-id="3703a-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3703a-133">Here is a JSON representation of the resource.</span></span>

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


