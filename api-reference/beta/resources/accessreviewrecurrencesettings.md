---
title: tipo de recurso accessReviewRecurrenceSettings
description: ''
localization_priority: Normal
ms.openlocfilehash: 1a5235639209830d36cf69c027cfd309fab09c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348331"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="4b67e-102">tipo de recurso accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="4b67e-102">accessReviewRecurrenceSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="4b67e-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b67e-103">Properties</span></span>
|<span data-ttu-id="4b67e-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b67e-104">Property</span></span>|<span data-ttu-id="4b67e-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b67e-105">Type</span></span>|<span data-ttu-id="4b67e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b67e-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="4b67e-107">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="4b67e-107">recurrenceType</span></span> | <span data-ttu-id="4b67e-108">string</span><span class="sxs-lookup"><span data-stu-id="4b67e-108">string</span></span> |  |
| <span data-ttu-id="4b67e-109">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="4b67e-109">recurrenceEndType</span></span> | <span data-ttu-id="4b67e-110">string</span><span class="sxs-lookup"><span data-stu-id="4b67e-110">string</span></span> |  |
| <span data-ttu-id="4b67e-111">durationInDays</span><span class="sxs-lookup"><span data-stu-id="4b67e-111">durationInDays</span></span> | <span data-ttu-id="4b67e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="4b67e-112">Int32</span></span> |  |
| <span data-ttu-id="4b67e-113">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="4b67e-113">recurrenceCount</span></span> | <span data-ttu-id="4b67e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="4b67e-114">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="4b67e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="4b67e-115">Relationships</span></span>
<span data-ttu-id="4b67e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b67e-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b67e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b67e-117">JSON Representation</span></span>
<span data-ttu-id="4b67e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b67e-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
``` json
{
    "recurrenceType":"string",
    "recurrenceEndType":"string",
    "durationInDays":"Int32",
    "recurrenceCount":"Int32"
}
```



