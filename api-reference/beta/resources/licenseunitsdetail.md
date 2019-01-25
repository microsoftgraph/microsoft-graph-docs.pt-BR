---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade prepaidUnits da entidade subscribedSku é do tipo licenseUnitsDetail.
localization_priority: Normal
ms.openlocfilehash: a5eacb79dfca97b992e2f8584761aaa45beccd76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511314"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="35b81-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="35b81-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35b81-104">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="35b81-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="35b81-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35b81-105">Properties</span></span>
| <span data-ttu-id="35b81-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35b81-106">Property</span></span>     | <span data-ttu-id="35b81-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="35b81-107">Type</span></span>   |<span data-ttu-id="35b81-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="35b81-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="35b81-109">enabled</span><span class="sxs-lookup"><span data-stu-id="35b81-109">enabled</span></span>|<span data-ttu-id="35b81-110">Int32</span><span class="sxs-lookup"><span data-stu-id="35b81-110">Int32</span></span>| <span data-ttu-id="35b81-111">O número de unidades que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="35b81-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="35b81-112">suspended</span><span class="sxs-lookup"><span data-stu-id="35b81-112">suspended</span></span>|<span data-ttu-id="35b81-113">Int32</span><span class="sxs-lookup"><span data-stu-id="35b81-113">Int32</span></span>| <span data-ttu-id="35b81-114">O número de unidades que estão suspensas.</span><span class="sxs-lookup"><span data-stu-id="35b81-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="35b81-115">warning</span><span class="sxs-lookup"><span data-stu-id="35b81-115">warning</span></span>|<span data-ttu-id="35b81-116">Int32</span><span class="sxs-lookup"><span data-stu-id="35b81-116">Int32</span></span>| <span data-ttu-id="35b81-117">O número de unidades que estão com um status de aviso.</span><span class="sxs-lookup"><span data-stu-id="35b81-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35b81-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35b81-118">JSON representation</span></span>

<span data-ttu-id="35b81-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="35b81-119">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseunitsdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
