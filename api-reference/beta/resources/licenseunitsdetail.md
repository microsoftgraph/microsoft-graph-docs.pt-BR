---
title: Tipo de recurso licenseUnitsDetail
description: A propriedade **prepaidUnits** da entidade subscribedSku é do tipo **licenseUnitsDetail**.
ms.openlocfilehash: 5f3d62c39248739746923195945efbc3322d5686
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033204"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="7c647-103">Tipo de recurso licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="7c647-103">licenseUnitsDetail resource type</span></span>

> <span data-ttu-id="7c647-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7c647-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c647-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7c647-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c647-106">A propriedade **prepaidUnits** da entidade [subscribedSku](subscribedsku.md) é do tipo **licenseUnitsDetail**.</span><span class="sxs-lookup"><span data-stu-id="7c647-106">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="7c647-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c647-107">Properties</span></span>
| <span data-ttu-id="7c647-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c647-108">Property</span></span>     | <span data-ttu-id="7c647-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c647-109">Type</span></span>   |<span data-ttu-id="7c647-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c647-110">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="7c647-111">enabled</span><span class="sxs-lookup"><span data-stu-id="7c647-111">enabled</span></span>|<span data-ttu-id="7c647-112">Int32</span><span class="sxs-lookup"><span data-stu-id="7c647-112">Int32</span></span>| <span data-ttu-id="7c647-113">O número de unidades que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="7c647-113">The number of units that are enabled.</span></span> |
|<span data-ttu-id="7c647-114">suspended</span><span class="sxs-lookup"><span data-stu-id="7c647-114">suspended</span></span>|<span data-ttu-id="7c647-115">Int32</span><span class="sxs-lookup"><span data-stu-id="7c647-115">Int32</span></span>| <span data-ttu-id="7c647-116">O número de unidades que estão suspensas.</span><span class="sxs-lookup"><span data-stu-id="7c647-116">The number of units that are suspended.</span></span> |
|<span data-ttu-id="7c647-117">warning</span><span class="sxs-lookup"><span data-stu-id="7c647-117">warning</span></span>|<span data-ttu-id="7c647-118">Int32</span><span class="sxs-lookup"><span data-stu-id="7c647-118">Int32</span></span>| <span data-ttu-id="7c647-119">O número de unidades que estão com um status de aviso.</span><span class="sxs-lookup"><span data-stu-id="7c647-119">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c647-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c647-120">JSON representation</span></span>

<span data-ttu-id="7c647-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7c647-121">Here is a JSON representation of the resource</span></span>

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
