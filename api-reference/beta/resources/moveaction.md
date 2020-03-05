---
author: daspek
description: A presença do recurso MoveAction em uma itemActivity indica que a atividade moveu um item.
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a42ef869a32cfe01a03344d3f155880bd528c462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522614"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="22ffa-103">Tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="22ffa-103">MoveAction resource type</span></span>

<span data-ttu-id="22ffa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22ffa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22ffa-105">A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="22ffa-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="22ffa-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22ffa-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="22ffa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22ffa-107">Properties</span></span>

| <span data-ttu-id="22ffa-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="22ffa-108">Property name</span></span> | <span data-ttu-id="22ffa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="22ffa-109">Type</span></span>   | <span data-ttu-id="22ffa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="22ffa-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="22ffa-111">from</span><span class="sxs-lookup"><span data-stu-id="22ffa-111">from</span></span>          | <span data-ttu-id="22ffa-112">string</span><span class="sxs-lookup"><span data-stu-id="22ffa-112">string</span></span> | <span data-ttu-id="22ffa-113">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="22ffa-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="22ffa-114">para</span><span class="sxs-lookup"><span data-stu-id="22ffa-114">to</span></span>            | <span data-ttu-id="22ffa-115">string</span><span class="sxs-lookup"><span data-stu-id="22ffa-115">string</span></span> | <span data-ttu-id="22ffa-116">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="22ffa-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="22ffa-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="22ffa-117">Remarks</span></span>

<span data-ttu-id="22ffa-118">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="22ffa-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
