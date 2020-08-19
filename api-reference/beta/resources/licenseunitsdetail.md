---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: bbff4ac919f5973caff7fbbc30fdc5d7352550b4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807504"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="0a80c-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="0a80c-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="0a80c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a80c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a80c-105">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="0a80c-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="0a80c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a80c-106">Properties</span></span>
| <span data-ttu-id="0a80c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a80c-107">Property</span></span>     | <span data-ttu-id="0a80c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a80c-108">Type</span></span>   |<span data-ttu-id="0a80c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a80c-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="0a80c-110">enabled</span><span class="sxs-lookup"><span data-stu-id="0a80c-110">enabled</span></span>|<span data-ttu-id="0a80c-111">Int32</span><span class="sxs-lookup"><span data-stu-id="0a80c-111">Int32</span></span>| <span data-ttu-id="0a80c-112">O número de unidades que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="0a80c-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="0a80c-113">suspended</span><span class="sxs-lookup"><span data-stu-id="0a80c-113">suspended</span></span>|<span data-ttu-id="0a80c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0a80c-114">Int32</span></span>| <span data-ttu-id="0a80c-115">O número de unidades que estão suspensas.</span><span class="sxs-lookup"><span data-stu-id="0a80c-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="0a80c-116">warning</span><span class="sxs-lookup"><span data-stu-id="0a80c-116">warning</span></span>|<span data-ttu-id="0a80c-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0a80c-117">Int32</span></span>| <span data-ttu-id="0a80c-118">O número de unidades que estão no status de aviso.</span><span class="sxs-lookup"><span data-stu-id="0a80c-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a80c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a80c-119">JSON representation</span></span>

<span data-ttu-id="0a80c-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0a80c-120">Here is a JSON representation of the resource</span></span>

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
