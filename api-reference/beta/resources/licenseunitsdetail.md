---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
ms.openlocfilehash: a119ea5d81689a814a9f7f8b10da8b267e98dd03
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345285"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="b9a64-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="b9a64-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9a64-104">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="b9a64-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="b9a64-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9a64-105">Properties</span></span>
| <span data-ttu-id="b9a64-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9a64-106">Property</span></span>     | <span data-ttu-id="b9a64-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9a64-107">Type</span></span>   |<span data-ttu-id="b9a64-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a64-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="b9a64-109">enabled</span><span class="sxs-lookup"><span data-stu-id="b9a64-109">enabled</span></span>|<span data-ttu-id="b9a64-110">Int32</span><span class="sxs-lookup"><span data-stu-id="b9a64-110">Int32</span></span>| <span data-ttu-id="b9a64-111">O número de unidades que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="b9a64-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="b9a64-112">suspended</span><span class="sxs-lookup"><span data-stu-id="b9a64-112">suspended</span></span>|<span data-ttu-id="b9a64-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b9a64-113">Int32</span></span>| <span data-ttu-id="b9a64-114">O número de unidades que estão suspensas.</span><span class="sxs-lookup"><span data-stu-id="b9a64-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="b9a64-115">warning</span><span class="sxs-lookup"><span data-stu-id="b9a64-115">warning</span></span>|<span data-ttu-id="b9a64-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b9a64-116">Int32</span></span>| <span data-ttu-id="b9a64-117">O número de unidades que estão no status de aviso.</span><span class="sxs-lookup"><span data-stu-id="b9a64-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9a64-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9a64-118">JSON representation</span></span>

<span data-ttu-id="b9a64-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b9a64-119">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
