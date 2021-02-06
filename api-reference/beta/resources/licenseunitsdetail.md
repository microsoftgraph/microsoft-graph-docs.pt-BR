---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: krbain
ms.openlocfilehash: 3d4925c2acea0216e16283eaa8f779cb556e0857
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132430"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="05f68-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="05f68-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="05f68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05f68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05f68-105">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="05f68-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="05f68-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05f68-106">Properties</span></span>
| <span data-ttu-id="05f68-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05f68-107">Property</span></span>     | <span data-ttu-id="05f68-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="05f68-108">Type</span></span>   |<span data-ttu-id="05f68-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="05f68-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="05f68-110">enabled</span><span class="sxs-lookup"><span data-stu-id="05f68-110">enabled</span></span>|<span data-ttu-id="05f68-111">Int32</span><span class="sxs-lookup"><span data-stu-id="05f68-111">Int32</span></span>| <span data-ttu-id="05f68-112">O número de unidades habilitadas.</span><span class="sxs-lookup"><span data-stu-id="05f68-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="05f68-113">suspended</span><span class="sxs-lookup"><span data-stu-id="05f68-113">suspended</span></span>|<span data-ttu-id="05f68-114">Int32</span><span class="sxs-lookup"><span data-stu-id="05f68-114">Int32</span></span>| <span data-ttu-id="05f68-115">O número de unidades suspensas.</span><span class="sxs-lookup"><span data-stu-id="05f68-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="05f68-116">warning</span><span class="sxs-lookup"><span data-stu-id="05f68-116">warning</span></span>|<span data-ttu-id="05f68-117">Int32</span><span class="sxs-lookup"><span data-stu-id="05f68-117">Int32</span></span>| <span data-ttu-id="05f68-118">O número de unidades que estão no status de aviso.</span><span class="sxs-lookup"><span data-stu-id="05f68-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="05f68-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05f68-119">JSON representation</span></span>

<span data-ttu-id="05f68-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="05f68-120">Here is a JSON representation of the resource</span></span>

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


