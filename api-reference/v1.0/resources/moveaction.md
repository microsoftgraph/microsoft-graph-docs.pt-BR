---
author: daspek
ms.author: dspektor
title: tipo de recurso MoveAction
description: O objeto MoveAction fornece informações sobre uma atividade que moveu um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 8ef93cd83c8fd020af91a9ea8c9288c1d27d5cf6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036068"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="e6719-103">tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="e6719-103">moveAction resource type</span></span>

<span data-ttu-id="e6719-104">A presença do recurso **MoveAction** em uma myactivity indica que a atividade moveu um item. [\*\*\*\*][activity]</span><span class="sxs-lookup"><span data-stu-id="e6719-104">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="e6719-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e6719-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="e6719-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6719-106">Properties</span></span>

| <span data-ttu-id="e6719-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e6719-107">Property name</span></span> | <span data-ttu-id="e6719-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6719-108">Type</span></span>   | <span data-ttu-id="e6719-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6719-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e6719-110">from</span><span class="sxs-lookup"><span data-stu-id="e6719-110">from</span></span>          | <span data-ttu-id="e6719-111">string</span><span class="sxs-lookup"><span data-stu-id="e6719-111">string</span></span> | <span data-ttu-id="e6719-112">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="e6719-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="e6719-113">para</span><span class="sxs-lookup"><span data-stu-id="e6719-113">to</span></span>            | <span data-ttu-id="e6719-114">string</span><span class="sxs-lookup"><span data-stu-id="e6719-114">string</span></span> | <span data-ttu-id="e6719-115">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="e6719-115">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6719-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6719-116">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
