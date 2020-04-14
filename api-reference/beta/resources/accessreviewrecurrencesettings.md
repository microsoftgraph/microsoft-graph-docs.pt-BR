---
title: tipo de recurso accessReviewRecurrenceSettings
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: markwahl-msft
ms.openlocfilehash: 7c45a0b57d869acdb49c5a37f235232c70e8ec6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472233"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="09b9e-102">tipo de recurso accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="09b9e-102">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="09b9e-103">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09b9e-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="09b9e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09b9e-104">Properties</span></span>
|<span data-ttu-id="09b9e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09b9e-105">Property</span></span>|<span data-ttu-id="09b9e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="09b9e-106">Type</span></span>|<span data-ttu-id="09b9e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="09b9e-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="09b9e-108">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="09b9e-108">recurrenceType</span></span> | <span data-ttu-id="09b9e-109">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09b9e-109">string</span></span> |  |
| <span data-ttu-id="09b9e-110">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="09b9e-110">recurrenceEndType</span></span> | <span data-ttu-id="09b9e-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09b9e-111">string</span></span> |  |
| <span data-ttu-id="09b9e-112">durationInDays</span><span class="sxs-lookup"><span data-stu-id="09b9e-112">durationInDays</span></span> | <span data-ttu-id="09b9e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="09b9e-113">Int32</span></span> |  |
| <span data-ttu-id="09b9e-114">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="09b9e-114">recurrenceCount</span></span> | <span data-ttu-id="09b9e-115">Int32</span><span class="sxs-lookup"><span data-stu-id="09b9e-115">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="09b9e-116">Relações</span><span class="sxs-lookup"><span data-stu-id="09b9e-116">Relationships</span></span>
<span data-ttu-id="09b9e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09b9e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09b9e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09b9e-118">JSON Representation</span></span>
<span data-ttu-id="09b9e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09b9e-119">Here is a JSON representation of the resource.</span></span>
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



