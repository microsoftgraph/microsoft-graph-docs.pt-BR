---
author: daspek
description: A presença do recurso MoveAction em uma itemActivity indica que a atividade moveu um item.
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 547a49e17a74be43500a9cf52aaa3a375272b810
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021284"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="37d32-103">Tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="37d32-103">MoveAction resource type</span></span>

<span data-ttu-id="37d32-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37d32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37d32-105">A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="37d32-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="37d32-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37d32-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="37d32-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37d32-107">Properties</span></span>

| <span data-ttu-id="37d32-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="37d32-108">Property name</span></span> | <span data-ttu-id="37d32-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="37d32-109">Type</span></span>   | <span data-ttu-id="37d32-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37d32-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="37d32-111">from</span><span class="sxs-lookup"><span data-stu-id="37d32-111">from</span></span>          | <span data-ttu-id="37d32-112">string</span><span class="sxs-lookup"><span data-stu-id="37d32-112">string</span></span> | <span data-ttu-id="37d32-113">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="37d32-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="37d32-114">para</span><span class="sxs-lookup"><span data-stu-id="37d32-114">to</span></span>            | <span data-ttu-id="37d32-115">string</span><span class="sxs-lookup"><span data-stu-id="37d32-115">string</span></span> | <span data-ttu-id="37d32-116">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="37d32-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="37d32-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="37d32-117">Remarks</span></span>

<span data-ttu-id="37d32-118">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="37d32-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


