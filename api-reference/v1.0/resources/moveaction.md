---
author: daspek
ms.author: dspektor
title: tipo de recurso MoveAction
description: O objeto MoveAction fornece informações sobre uma atividade que moveu um item.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 04c9ddad00b5705d84af6e72ac194a0d32fd015c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447378"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="8c23a-103">tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="8c23a-103">moveAction resource type</span></span>

<span data-ttu-id="8c23a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c23a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c23a-105">A presença do recurso **MoveAction** em uma [**myactivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="8c23a-105">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="8c23a-106">**Observação:** Os registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="8c23a-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="8c23a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c23a-107">Properties</span></span>

| <span data-ttu-id="8c23a-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8c23a-108">Property name</span></span> | <span data-ttu-id="8c23a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c23a-109">Type</span></span>   | <span data-ttu-id="8c23a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c23a-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8c23a-111">from</span><span class="sxs-lookup"><span data-stu-id="8c23a-111">from</span></span>          | <span data-ttu-id="8c23a-112">string</span><span class="sxs-lookup"><span data-stu-id="8c23a-112">string</span></span> | <span data-ttu-id="8c23a-113">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="8c23a-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="8c23a-114">para</span><span class="sxs-lookup"><span data-stu-id="8c23a-114">to</span></span>            | <span data-ttu-id="8c23a-115">string</span><span class="sxs-lookup"><span data-stu-id="8c23a-115">string</span></span> | <span data-ttu-id="8c23a-116">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="8c23a-116">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c23a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c23a-117">JSON representation</span></span>

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
