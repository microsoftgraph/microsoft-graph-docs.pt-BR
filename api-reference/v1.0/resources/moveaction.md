---
author: daspek
ms.author: dspektor
title: tipo de recurso MoveAction
description: O objeto MoveAction fornece informações sobre uma atividade que moveu um item.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 525558d040109e637e2f3532d16c308a197e45fb
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970617"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="34000-103">tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="34000-103">moveAction resource type</span></span>

<span data-ttu-id="34000-104">A presença do recurso **MoveAction** em uma myactivity [\*\*\*\*] [ activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="34000-104">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="34000-105">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="34000-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="34000-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34000-106">Properties</span></span>

| <span data-ttu-id="34000-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="34000-107">Property name</span></span> | <span data-ttu-id="34000-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="34000-108">Type</span></span>   | <span data-ttu-id="34000-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34000-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="34000-110">from</span><span class="sxs-lookup"><span data-stu-id="34000-110">from</span></span>          | <span data-ttu-id="34000-111">string</span><span class="sxs-lookup"><span data-stu-id="34000-111">string</span></span> | <span data-ttu-id="34000-112">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="34000-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="34000-113">para</span><span class="sxs-lookup"><span data-stu-id="34000-113">to</span></span>            | <span data-ttu-id="34000-114">string</span><span class="sxs-lookup"><span data-stu-id="34000-114">string</span></span> | <span data-ttu-id="34000-115">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="34000-115">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34000-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34000-116">JSON representation</span></span>

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
