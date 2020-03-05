---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4de4d89b5abec06abc6d2f8bfa4f78c22abe4ca0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447574"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="02a65-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="02a65-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="02a65-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02a65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02a65-105">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="02a65-105">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="02a65-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02a65-106">Properties</span></span>
| <span data-ttu-id="02a65-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02a65-107">Property</span></span>     | <span data-ttu-id="02a65-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="02a65-108">Type</span></span>   |<span data-ttu-id="02a65-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="02a65-109">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="02a65-110">enabled</span><span class="sxs-lookup"><span data-stu-id="02a65-110">enabled</span></span>|<span data-ttu-id="02a65-111">Int32</span><span class="sxs-lookup"><span data-stu-id="02a65-111">Int32</span></span>| <span data-ttu-id="02a65-112">O número de unidades que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="02a65-112">The number of units that are enabled.</span></span> |
|<span data-ttu-id="02a65-113">suspended</span><span class="sxs-lookup"><span data-stu-id="02a65-113">suspended</span></span>|<span data-ttu-id="02a65-114">Int32</span><span class="sxs-lookup"><span data-stu-id="02a65-114">Int32</span></span>| <span data-ttu-id="02a65-115">O número de unidades que estão suspensas.</span><span class="sxs-lookup"><span data-stu-id="02a65-115">The number of units that are suspended.</span></span> |
|<span data-ttu-id="02a65-116">warning</span><span class="sxs-lookup"><span data-stu-id="02a65-116">warning</span></span>|<span data-ttu-id="02a65-117">Int32</span><span class="sxs-lookup"><span data-stu-id="02a65-117">Int32</span></span>| <span data-ttu-id="02a65-118">O número de unidades que estão no status de aviso.</span><span class="sxs-lookup"><span data-stu-id="02a65-118">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="02a65-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02a65-119">JSON representation</span></span>

<span data-ttu-id="02a65-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="02a65-120">Here is a JSON representation of the resource</span></span>

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
