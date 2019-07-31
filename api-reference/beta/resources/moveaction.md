---
author: daspek
description: A presença do recurso MoveAction em uma itemActivity indica que a atividade moveu um item.
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9fbb19097b6a1401bd3c0b6dba4ce1fd5649e706
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009640"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="e2907-103">Tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="e2907-103">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2907-104">A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="e2907-104">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e2907-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2907-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e2907-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2907-106">Properties</span></span>

| <span data-ttu-id="e2907-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e2907-107">Property name</span></span> | <span data-ttu-id="e2907-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2907-108">Type</span></span>   | <span data-ttu-id="e2907-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2907-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e2907-110">from</span><span class="sxs-lookup"><span data-stu-id="e2907-110">from</span></span>          | <span data-ttu-id="e2907-111">string</span><span class="sxs-lookup"><span data-stu-id="e2907-111">string</span></span> | <span data-ttu-id="e2907-112">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="e2907-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="e2907-113">para</span><span class="sxs-lookup"><span data-stu-id="e2907-113">to</span></span>            | <span data-ttu-id="e2907-114">string</span><span class="sxs-lookup"><span data-stu-id="e2907-114">string</span></span> | <span data-ttu-id="e2907-115">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="e2907-115">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="e2907-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="e2907-116">Remarks</span></span>

<span data-ttu-id="e2907-117">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e2907-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
