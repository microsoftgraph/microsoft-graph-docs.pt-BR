---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: aa20816165ed4f41e8b89af106e3f781b1be8dd7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530080"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="a1cbe-102">Tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="a1cbe-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1cbe-103">A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="a1cbe-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="a1cbe-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1cbe-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

## <a name="properties"></a><span data-ttu-id="a1cbe-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1cbe-105">Properties</span></span>

| <span data-ttu-id="a1cbe-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a1cbe-106">Property name</span></span> | <span data-ttu-id="a1cbe-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1cbe-107">Type</span></span>   | <span data-ttu-id="a1cbe-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1cbe-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="a1cbe-109">from</span><span class="sxs-lookup"><span data-stu-id="a1cbe-109">from</span></span>          | <span data-ttu-id="a1cbe-110">string</span><span class="sxs-lookup"><span data-stu-id="a1cbe-110">string</span></span> | <span data-ttu-id="a1cbe-111">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="a1cbe-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="a1cbe-112">para</span><span class="sxs-lookup"><span data-stu-id="a1cbe-112">to</span></span>            | <span data-ttu-id="a1cbe-113">string</span><span class="sxs-lookup"><span data-stu-id="a1cbe-113">string</span></span> | <span data-ttu-id="a1cbe-114">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="a1cbe-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="a1cbe-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="a1cbe-115">Remarks</span></span>

<span data-ttu-id="a1cbe-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a1cbe-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/moveaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
