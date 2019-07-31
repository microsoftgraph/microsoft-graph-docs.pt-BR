---
title: tipo de recurso accessReviewRecurrenceSettings
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: ''
ms.openlocfilehash: 2bf71fe1c715eb96e98b0caf7720cc0d637ee33b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974514"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="16ff1-102">tipo de recurso accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="16ff1-102">accessReviewRecurrenceSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="16ff1-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16ff1-103">Properties</span></span>
|<span data-ttu-id="16ff1-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16ff1-104">Property</span></span>|<span data-ttu-id="16ff1-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="16ff1-105">Type</span></span>|<span data-ttu-id="16ff1-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="16ff1-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="16ff1-107">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="16ff1-107">recurrenceType</span></span> | <span data-ttu-id="16ff1-108">string</span><span class="sxs-lookup"><span data-stu-id="16ff1-108">string</span></span> |  |
| <span data-ttu-id="16ff1-109">recurrenceEndType</span><span class="sxs-lookup"><span data-stu-id="16ff1-109">recurrenceEndType</span></span> | <span data-ttu-id="16ff1-110">string</span><span class="sxs-lookup"><span data-stu-id="16ff1-110">string</span></span> |  |
| <span data-ttu-id="16ff1-111">durationInDays</span><span class="sxs-lookup"><span data-stu-id="16ff1-111">durationInDays</span></span> | <span data-ttu-id="16ff1-112">Int32</span><span class="sxs-lookup"><span data-stu-id="16ff1-112">Int32</span></span> |  |
| <span data-ttu-id="16ff1-113">recurrenceCount</span><span class="sxs-lookup"><span data-stu-id="16ff1-113">recurrenceCount</span></span> | <span data-ttu-id="16ff1-114">Int32</span><span class="sxs-lookup"><span data-stu-id="16ff1-114">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="16ff1-115">Relações</span><span class="sxs-lookup"><span data-stu-id="16ff1-115">Relationships</span></span>
<span data-ttu-id="16ff1-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16ff1-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="16ff1-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16ff1-117">JSON Representation</span></span>
<span data-ttu-id="16ff1-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16ff1-118">Here is a JSON representation of the resource.</span></span>
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



