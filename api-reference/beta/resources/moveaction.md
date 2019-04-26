---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 0715f8e9743c4384e8fbd851fe88563e9eaf9666
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342209"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="51b89-102">Tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="51b89-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b89-103">A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="51b89-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="51b89-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51b89-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="51b89-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51b89-105">Properties</span></span>

| <span data-ttu-id="51b89-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="51b89-106">Property name</span></span> | <span data-ttu-id="51b89-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="51b89-107">Type</span></span>   | <span data-ttu-id="51b89-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="51b89-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="51b89-109">from</span><span class="sxs-lookup"><span data-stu-id="51b89-109">from</span></span>          | <span data-ttu-id="51b89-110">string</span><span class="sxs-lookup"><span data-stu-id="51b89-110">string</span></span> | <span data-ttu-id="51b89-111">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="51b89-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="51b89-112">para</span><span class="sxs-lookup"><span data-stu-id="51b89-112">to</span></span>            | <span data-ttu-id="51b89-113">string</span><span class="sxs-lookup"><span data-stu-id="51b89-113">string</span></span> | <span data-ttu-id="51b89-114">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="51b89-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="51b89-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="51b89-115">Remarks</span></span>

<span data-ttu-id="51b89-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="51b89-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
