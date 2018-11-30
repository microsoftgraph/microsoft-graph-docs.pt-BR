---
title: Tipo de recurso plannerChecklistItem
description: O recurso de **plannerChecklistItem** representa um item na lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo objeto itens.
ms.openlocfilehash: 846c1877fb421c9070eff7c041983367a7beb29b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036426"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="a5ec8-104">Tipo de recurso plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="a5ec8-104">plannerChecklistItem resource type</span></span>

> <span data-ttu-id="a5ec8-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5ec8-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5ec8-p103">O recurso **plannerChecklistItem** representa um item da lista de verificação de uma tarefa. A lista de verificação em uma tarefa é representada pelo [objeto checklistItems](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="a5ec8-p103">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="a5ec8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5ec8-109">Properties</span></span>
| <span data-ttu-id="a5ec8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5ec8-110">Property</span></span>     | <span data-ttu-id="a5ec8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5ec8-111">Type</span></span>   |<span data-ttu-id="a5ec8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ec8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5ec8-113">isChecked</span><span class="sxs-lookup"><span data-stu-id="a5ec8-113">isChecked</span></span>|<span data-ttu-id="a5ec8-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5ec8-114">Boolean</span></span>|<span data-ttu-id="a5ec8-115">O valor será `true` se o item estiver marcado ou `false`, caso não estiver marcado.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-115">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="a5ec8-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a5ec8-116">lastModifiedBy</span></span>|[<span data-ttu-id="a5ec8-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="a5ec8-117">identitySet</span></span>](identityset.md)| <span data-ttu-id="a5ec8-p104">Somente leitura. A identificação de usuário pela qual isso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="a5ec8-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5ec8-120">lastModifiedDateTime</span></span>|<span data-ttu-id="a5ec8-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5ec8-121">DateTimeOffset</span></span>|<span data-ttu-id="a5ec8-p105">Somente leitura. A data e a hora pelas quais isso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a5ec8-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a5ec8-126">orderHint</span><span class="sxs-lookup"><span data-stu-id="a5ec8-126">orderHint</span></span>|<span data-ttu-id="a5ec8-127">String</span><span class="sxs-lookup"><span data-stu-id="a5ec8-127">String</span></span>|<span data-ttu-id="a5ec8-p106">Usado para definir a ordem relativa dos itens na lista de verificação. O formato é definido como descrito [aqui](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="a5ec8-p106">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="a5ec8-130">title</span><span class="sxs-lookup"><span data-stu-id="a5ec8-130">title</span></span>|<span data-ttu-id="a5ec8-131">String</span><span class="sxs-lookup"><span data-stu-id="a5ec8-131">String</span></span>|<span data-ttu-id="a5ec8-132">Título do item de lista de verificação</span><span class="sxs-lookup"><span data-stu-id="a5ec8-132">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5ec8-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5ec8-133">JSON representation</span></span>
<span data-ttu-id="a5ec8-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-134">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->