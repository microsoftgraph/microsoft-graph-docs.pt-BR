---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
ms.openlocfilehash: e8cf5253676dab8a4b31c3ab33faa0af3ddfd527
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003605"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="d1dd1-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="d1dd1-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="d1dd1-104">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="d1dd1-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="d1dd1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1dd1-105">Properties</span></span>
| <span data-ttu-id="d1dd1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1dd1-106">Property</span></span>     | <span data-ttu-id="d1dd1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1dd1-107">Type</span></span>   |<span data-ttu-id="d1dd1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1dd1-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="d1dd1-109">enabled</span><span class="sxs-lookup"><span data-stu-id="d1dd1-109">enabled</span></span>|<span data-ttu-id="d1dd1-110">Int32</span><span class="sxs-lookup"><span data-stu-id="d1dd1-110">Int32</span></span>| <span data-ttu-id="d1dd1-111">O número de unidades que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="d1dd1-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="d1dd1-112">suspended</span><span class="sxs-lookup"><span data-stu-id="d1dd1-112">suspended</span></span>|<span data-ttu-id="d1dd1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d1dd1-113">Int32</span></span>| <span data-ttu-id="d1dd1-114">O número de unidades que estão suspensas.</span><span class="sxs-lookup"><span data-stu-id="d1dd1-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="d1dd1-115">warning</span><span class="sxs-lookup"><span data-stu-id="d1dd1-115">warning</span></span>|<span data-ttu-id="d1dd1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d1dd1-116">Int32</span></span>| <span data-ttu-id="d1dd1-117">O número de unidades que estão com um status de aviso.</span><span class="sxs-lookup"><span data-stu-id="d1dd1-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d1dd1-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1dd1-118">JSON representation</span></span>

<span data-ttu-id="d1dd1-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d1dd1-119">Here is a JSON representation of the resource</span></span>

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
