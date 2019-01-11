---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 40049b506c72af5aacddf461b22e1ddd280d7ad4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852896"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="9bb3d-102">Tipo de recurso MoveAction</span><span class="sxs-lookup"><span data-stu-id="9bb3d-102">MoveAction resource type</span></span>

> <span data-ttu-id="9bb3d-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9bb3d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bb3d-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9bb3d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9bb3d-105">A presença do recurso **MoveAction** em uma [**itemActivity**][activity] indica que a atividade moveu um item.</span><span class="sxs-lookup"><span data-stu-id="9bb3d-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9bb3d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bb3d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9bb3d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bb3d-107">Properties</span></span>

| <span data-ttu-id="9bb3d-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9bb3d-108">Property name</span></span> | <span data-ttu-id="9bb3d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bb3d-109">Type</span></span>   | <span data-ttu-id="9bb3d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bb3d-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="9bb3d-111">from</span><span class="sxs-lookup"><span data-stu-id="9bb3d-111">from</span></span>          | <span data-ttu-id="9bb3d-112">string</span><span class="sxs-lookup"><span data-stu-id="9bb3d-112">string</span></span> | <span data-ttu-id="9bb3d-113">O nome do local do qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="9bb3d-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="9bb3d-114">para</span><span class="sxs-lookup"><span data-stu-id="9bb3d-114">to</span></span>            | <span data-ttu-id="9bb3d-115">string</span><span class="sxs-lookup"><span data-stu-id="9bb3d-115">string</span></span> | <span data-ttu-id="9bb3d-116">O nome do local para o qual o item foi movido.</span><span class="sxs-lookup"><span data-stu-id="9bb3d-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="9bb3d-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="9bb3d-117">Remarks</span></span>

<span data-ttu-id="9bb3d-118">Registros de atividade de item atualmente só estão disponíveis no SharePoint e no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="9bb3d-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction"
} -->
