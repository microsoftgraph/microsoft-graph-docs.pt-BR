---
title: tipo de recurso plannerChecklistItem
description: O recurso **plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo objeto checklistItems.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9bce6b0089f9e713e66e0354ce58d68cfd17fa7c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009073"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="642c7-104">tipo de recurso plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="642c7-104">plannerChecklistItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="642c7-105">O recurso **plannerChecklistItem** representa um item na lista de verificação de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="642c7-105">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="642c7-106">A lista de verificação em uma tarefa é representada pelo [objeto checklistItems](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="642c7-106">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="642c7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="642c7-107">Properties</span></span>
| <span data-ttu-id="642c7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="642c7-108">Property</span></span>     | <span data-ttu-id="642c7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="642c7-109">Type</span></span>   |<span data-ttu-id="642c7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="642c7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="642c7-111">IsChecked</span><span class="sxs-lookup"><span data-stu-id="642c7-111">isChecked</span></span>|<span data-ttu-id="642c7-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="642c7-112">Boolean</span></span>|<span data-ttu-id="642c7-113">Value é `true` se o item estiver marcado e `false` , caso contrário.</span><span class="sxs-lookup"><span data-stu-id="642c7-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="642c7-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="642c7-114">lastModifiedBy</span></span>|[<span data-ttu-id="642c7-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="642c7-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="642c7-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="642c7-116">Read-only.</span></span> <span data-ttu-id="642c7-117">ID de usuário pela qual esta foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="642c7-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="642c7-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="642c7-118">lastModifiedDateTime</span></span>|<span data-ttu-id="642c7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="642c7-119">DateTimeOffset</span></span>|<span data-ttu-id="642c7-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="642c7-120">Read-only.</span></span> <span data-ttu-id="642c7-121">Data e hora da última modificação.</span><span class="sxs-lookup"><span data-stu-id="642c7-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="642c7-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="642c7-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="642c7-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="642c7-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="642c7-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="642c7-124">orderHint</span></span>|<span data-ttu-id="642c7-125">String</span><span class="sxs-lookup"><span data-stu-id="642c7-125">String</span></span>|<span data-ttu-id="642c7-126">Usado para definir a ordem relativa dos itens na lista de verificação.</span><span class="sxs-lookup"><span data-stu-id="642c7-126">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="642c7-127">O formato é definido conforme descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="642c7-127">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="642c7-128">title</span><span class="sxs-lookup"><span data-stu-id="642c7-128">title</span></span>|<span data-ttu-id="642c7-129">String</span><span class="sxs-lookup"><span data-stu-id="642c7-129">String</span></span>|<span data-ttu-id="642c7-130">Título do item de lista de verificação</span><span class="sxs-lookup"><span data-stu-id="642c7-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="642c7-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="642c7-131">JSON representation</span></span>
<span data-ttu-id="642c7-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="642c7-132">Here is a JSON representation of the resource.</span></span>

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
