---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
author: krbain
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: af761aea94f21d3543bcaa8032d4120e3d1ad502
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048327"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="6afbe-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="6afbe-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="6afbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6afbe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6afbe-105">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="6afbe-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="6afbe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6afbe-106">Properties</span></span>
| <span data-ttu-id="6afbe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6afbe-107">Property</span></span>     | <span data-ttu-id="6afbe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6afbe-108">Type</span></span>   |<span data-ttu-id="6afbe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6afbe-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="6afbe-110">enabled</span><span class="sxs-lookup"><span data-stu-id="6afbe-110">enabled</span></span>|<span data-ttu-id="6afbe-111">Int32</span><span class="sxs-lookup"><span data-stu-id="6afbe-111">Int32</span></span>| <span data-ttu-id="6afbe-112">O número de unidades que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="6afbe-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="6afbe-113">suspended</span><span class="sxs-lookup"><span data-stu-id="6afbe-113">suspended</span></span>|<span data-ttu-id="6afbe-114">Int32</span><span class="sxs-lookup"><span data-stu-id="6afbe-114">Int32</span></span>| <span data-ttu-id="6afbe-115">O número de unidades que estão suspensas.</span><span class="sxs-lookup"><span data-stu-id="6afbe-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="6afbe-116">warning</span><span class="sxs-lookup"><span data-stu-id="6afbe-116">warning</span></span>|<span data-ttu-id="6afbe-117">Int32</span><span class="sxs-lookup"><span data-stu-id="6afbe-117">Int32</span></span>| <span data-ttu-id="6afbe-118">O número de unidades que estão no status de aviso.</span><span class="sxs-lookup"><span data-stu-id="6afbe-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6afbe-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6afbe-119">JSON representation</span></span>

<span data-ttu-id="6afbe-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6afbe-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

