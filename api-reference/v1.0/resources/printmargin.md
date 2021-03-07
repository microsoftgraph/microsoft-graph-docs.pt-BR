---
title: Tipo de recurso printMargin
description: Especifica as larguras de margem a ser usadas durante a impressão.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1680cc641da02f3339dcd75977c411d3255cf037
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517035"
---
# <a name="printmargin-resource-type"></a><span data-ttu-id="aef3d-103">Tipo de recurso printMargin</span><span class="sxs-lookup"><span data-stu-id="aef3d-103">printMargin resource type</span></span>

<span data-ttu-id="aef3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aef3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="aef3d-105">Especifica as larguras de margem a ser usadas durante a impressão.</span><span class="sxs-lookup"><span data-stu-id="aef3d-105">Specifies the margin widths to use when printing.</span></span>

## <a name="properties"></a><span data-ttu-id="aef3d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aef3d-106">Properties</span></span>
|<span data-ttu-id="aef3d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aef3d-107">Property</span></span>|<span data-ttu-id="aef3d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="aef3d-108">Type</span></span>|<span data-ttu-id="aef3d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aef3d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aef3d-110">top</span><span class="sxs-lookup"><span data-stu-id="aef3d-110">top</span></span>|<span data-ttu-id="aef3d-111">Int32</span><span class="sxs-lookup"><span data-stu-id="aef3d-111">Int32</span></span>|<span data-ttu-id="aef3d-112">A margem em mícrons da borda superior.</span><span class="sxs-lookup"><span data-stu-id="aef3d-112">The margin in microns from the top edge.</span></span>|
|<span data-ttu-id="aef3d-113">bottom</span><span class="sxs-lookup"><span data-stu-id="aef3d-113">bottom</span></span>|<span data-ttu-id="aef3d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="aef3d-114">Int32</span></span>|<span data-ttu-id="aef3d-115">A margem em mícrons da borda inferior.</span><span class="sxs-lookup"><span data-stu-id="aef3d-115">The margin in microns from the bottom edge.</span></span>|
|<span data-ttu-id="aef3d-116">Certo</span><span class="sxs-lookup"><span data-stu-id="aef3d-116">right</span></span>|<span data-ttu-id="aef3d-117">Int32</span><span class="sxs-lookup"><span data-stu-id="aef3d-117">Int32</span></span>|<span data-ttu-id="aef3d-118">A margem em mícrons da borda direita.</span><span class="sxs-lookup"><span data-stu-id="aef3d-118">The margin in microns from the right edge.</span></span>|
|<span data-ttu-id="aef3d-119">left</span><span class="sxs-lookup"><span data-stu-id="aef3d-119">left</span></span>|<span data-ttu-id="aef3d-120">Int32</span><span class="sxs-lookup"><span data-stu-id="aef3d-120">Int32</span></span>|<span data-ttu-id="aef3d-121">A margem em mícrons da borda esquerda.</span><span class="sxs-lookup"><span data-stu-id="aef3d-121">The margin in microns from the left edge.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aef3d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aef3d-122">JSON representation</span></span>
<span data-ttu-id="aef3d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aef3d-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printMargin"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printMargin",
  "top": "Integer",
  "bottom": "Integer",
  "right": "Integer",
  "left": "Integer"
}
```

