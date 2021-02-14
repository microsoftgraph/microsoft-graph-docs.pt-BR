---
author: daspek
title: Tipo de recurso moveAction
description: O objeto MoveAction fornece informações sobre uma atividade que moveu um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2f588ecabefa1425f47d3efec6728587fb694798
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239335"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="4ef47-103">Tipo de recurso moveAction</span><span class="sxs-lookup"><span data-stu-id="4ef47-103">moveAction resource type</span></span>

<span data-ttu-id="4ef47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ef47-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ef47-105">A presença do recurso **moveAction** em um [**itemActivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="4ef47-105">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="4ef47-106">**Observação:** No momento, os registros de atividades do item só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="4ef47-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="4ef47-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ef47-107">Properties</span></span>

| <span data-ttu-id="4ef47-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4ef47-108">Property name</span></span> | <span data-ttu-id="4ef47-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ef47-109">Type</span></span>   | <span data-ttu-id="4ef47-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ef47-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="4ef47-111">from</span><span class="sxs-lookup"><span data-stu-id="4ef47-111">from</span></span>          | <span data-ttu-id="4ef47-112">string</span><span class="sxs-lookup"><span data-stu-id="4ef47-112">string</span></span> | <span data-ttu-id="4ef47-113">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="4ef47-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="4ef47-114">para</span><span class="sxs-lookup"><span data-stu-id="4ef47-114">to</span></span>            | <span data-ttu-id="4ef47-115">string</span><span class="sxs-lookup"><span data-stu-id="4ef47-115">string</span></span> | <span data-ttu-id="4ef47-116">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="4ef47-116">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ef47-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ef47-117">JSON representation</span></span>

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

