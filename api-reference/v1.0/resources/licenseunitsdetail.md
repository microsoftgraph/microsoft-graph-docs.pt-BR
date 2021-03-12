---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
author: jpettere
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a34b093954915fa49ed7d907e367c7e53133c14f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722220"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="77e4e-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="77e4e-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="77e4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77e4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77e4e-105">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="77e4e-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="77e4e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77e4e-106">Properties</span></span>
| <span data-ttu-id="77e4e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77e4e-107">Property</span></span>     | <span data-ttu-id="77e4e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="77e4e-108">Type</span></span>   |<span data-ttu-id="77e4e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="77e4e-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="77e4e-110">enabled</span><span class="sxs-lookup"><span data-stu-id="77e4e-110">enabled</span></span>|<span data-ttu-id="77e4e-111">Int32</span><span class="sxs-lookup"><span data-stu-id="77e4e-111">Int32</span></span>| <span data-ttu-id="77e4e-112">O número de unidades habilitadas.</span><span class="sxs-lookup"><span data-stu-id="77e4e-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="77e4e-113">suspended</span><span class="sxs-lookup"><span data-stu-id="77e4e-113">suspended</span></span>|<span data-ttu-id="77e4e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="77e4e-114">Int32</span></span>| <span data-ttu-id="77e4e-115">O número de unidades suspensas.</span><span class="sxs-lookup"><span data-stu-id="77e4e-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="77e4e-116">warning</span><span class="sxs-lookup"><span data-stu-id="77e4e-116">warning</span></span>|<span data-ttu-id="77e4e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="77e4e-117">Int32</span></span>| <span data-ttu-id="77e4e-118">O número de unidades que estão em status de aviso.</span><span class="sxs-lookup"><span data-stu-id="77e4e-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77e4e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77e4e-119">JSON representation</span></span>

<span data-ttu-id="77e4e-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="77e4e-120">Here is a JSON representation of the resource</span></span>

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

