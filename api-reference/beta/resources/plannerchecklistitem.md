---
title: Tipo de recurso plannerChecklistItem
description: O recurso **plannerChecklistItem** representa um item da lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo objeto checklistItems.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 87f7349e20245068a0a29a179ddb5505cd3be0ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522536"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="d5f7b-104">Tipo de recurso plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="d5f7b-104">plannerChecklistItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5f7b-p102">O recurso **plannerChecklistItem** representa um item da lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo [objeto checklistItems](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="d5f7b-p102">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="d5f7b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5f7b-107">Properties</span></span>
| <span data-ttu-id="d5f7b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5f7b-108">Property</span></span>     | <span data-ttu-id="d5f7b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5f7b-109">Type</span></span>   |<span data-ttu-id="d5f7b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5f7b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5f7b-111">isChecked</span><span class="sxs-lookup"><span data-stu-id="d5f7b-111">isChecked</span></span>|<span data-ttu-id="d5f7b-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5f7b-112">Boolean</span></span>|<span data-ttu-id="d5f7b-113">O valor será `true` se o item estiver marcado ou `false`, caso não estiver marcado.</span><span class="sxs-lookup"><span data-stu-id="d5f7b-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="d5f7b-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d5f7b-114">lastModifiedBy</span></span>|[<span data-ttu-id="d5f7b-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="d5f7b-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="d5f7b-p103">Somente leitura. A identificação de usuário pela qual isso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d5f7b-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="d5f7b-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5f7b-118">lastModifiedDateTime</span></span>|<span data-ttu-id="d5f7b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5f7b-119">DateTimeOffset</span></span>|<span data-ttu-id="d5f7b-p104">Somente leitura. A data e a hora pelas quais isso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d5f7b-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d5f7b-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="d5f7b-124">orderHint</span></span>|<span data-ttu-id="d5f7b-125">String</span><span class="sxs-lookup"><span data-stu-id="d5f7b-125">String</span></span>|<span data-ttu-id="d5f7b-p105">Usado para definir a ordem relativa dos itens na lista de verificação. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="d5f7b-p105">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="d5f7b-128">title</span><span class="sxs-lookup"><span data-stu-id="d5f7b-128">title</span></span>|<span data-ttu-id="d5f7b-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5f7b-129">String</span></span>|<span data-ttu-id="d5f7b-130">Título do item de lista de verificação</span><span class="sxs-lookup"><span data-stu-id="d5f7b-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5f7b-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5f7b-131">JSON representation</span></span>
<span data-ttu-id="d5f7b-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5f7b-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerchecklistitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
