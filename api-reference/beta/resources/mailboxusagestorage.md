---
title: tipo de recurso mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 636417b5ec299bb11f82c406abecdebe72ee45de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473412"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="aa30f-103">tipo de recurso mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="aa30f-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="aa30f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa30f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="aa30f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa30f-105">Properties</span></span>

| <span data-ttu-id="aa30f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa30f-106">Property</span></span>           | <span data-ttu-id="aa30f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa30f-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="aa30f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="aa30f-108">reportRefreshDate</span></span>  | <span data-ttu-id="aa30f-109">Data</span><span class="sxs-lookup"><span data-stu-id="aa30f-109">Date</span></span>   |
| <span data-ttu-id="aa30f-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="aa30f-110">storageUsedInBytes</span></span> | <span data-ttu-id="aa30f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="aa30f-111">Int64</span></span>  |
| <span data-ttu-id="aa30f-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="aa30f-112">reportDate</span></span>         | <span data-ttu-id="aa30f-113">Data</span><span class="sxs-lookup"><span data-stu-id="aa30f-113">Date</span></span>   |
| <span data-ttu-id="aa30f-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="aa30f-114">reportPeriod</span></span>       | <span data-ttu-id="aa30f-115">String</span><span class="sxs-lookup"><span data-stu-id="aa30f-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa30f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa30f-116">JSON representation</span></span>

<span data-ttu-id="aa30f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa30f-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
