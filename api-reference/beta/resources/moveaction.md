---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: aa20816165ed4f41e8b89af106e3f781b1be8dd7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562577"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="e4060-102">Tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="e4060-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4060-103">A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="e4060-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e4060-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4060-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e4060-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4060-105">Properties</span></span>

| <span data-ttu-id="e4060-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e4060-106">Property name</span></span> | <span data-ttu-id="e4060-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4060-107">Type</span></span>   | <span data-ttu-id="e4060-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4060-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e4060-109">from</span><span class="sxs-lookup"><span data-stu-id="e4060-109">from</span></span>          | <span data-ttu-id="e4060-110">string</span><span class="sxs-lookup"><span data-stu-id="e4060-110">string</span></span> | <span data-ttu-id="e4060-111">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="e4060-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="e4060-112">para</span><span class="sxs-lookup"><span data-stu-id="e4060-112">to</span></span>            | <span data-ttu-id="e4060-113">string</span><span class="sxs-lookup"><span data-stu-id="e4060-113">string</span></span> | <span data-ttu-id="e4060-114">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="e4060-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="e4060-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="e4060-115">Remarks</span></span>

<span data-ttu-id="e4060-116">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="e4060-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
