---
title: Tipo de recurso mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4fedb101fbab2b14ec2d1ada1e02faa4bc729e0d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982198"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="fe839-103">Tipo de recurso mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="fe839-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="fe839-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe839-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="fe839-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe839-105">Properties</span></span>

| <span data-ttu-id="fe839-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe839-106">Property</span></span>           | <span data-ttu-id="fe839-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe839-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="fe839-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fe839-108">reportRefreshDate</span></span>  | <span data-ttu-id="fe839-109">Data</span><span class="sxs-lookup"><span data-stu-id="fe839-109">Date</span></span>   |
| <span data-ttu-id="fe839-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="fe839-110">storageUsedInBytes</span></span> | <span data-ttu-id="fe839-111">Int64</span><span class="sxs-lookup"><span data-stu-id="fe839-111">Int64</span></span>  |
| <span data-ttu-id="fe839-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="fe839-112">reportDate</span></span>         | <span data-ttu-id="fe839-113">Data</span><span class="sxs-lookup"><span data-stu-id="fe839-113">Date</span></span>   |
| <span data-ttu-id="fe839-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fe839-114">reportPeriod</span></span>       | <span data-ttu-id="fe839-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe839-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe839-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe839-116">JSON representation</span></span>

<span data-ttu-id="fe839-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe839-117">The following is a JSON representation of the resource.</span></span>

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


