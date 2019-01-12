---
title: tipo de recurso de siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928098"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="08b55-103">tipo de recurso de siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="08b55-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="08b55-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08b55-104">Properties</span></span>

| <span data-ttu-id="08b55-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08b55-105">Property</span></span>           | <span data-ttu-id="08b55-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="08b55-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="08b55-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="08b55-107">reportRefreshDate</span></span>  | <span data-ttu-id="08b55-108">Data</span><span class="sxs-lookup"><span data-stu-id="08b55-108">Date</span></span>   |
| <span data-ttu-id="08b55-109">siteType</span><span class="sxs-lookup"><span data-stu-id="08b55-109">siteType</span></span>           | <span data-ttu-id="08b55-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08b55-110">String</span></span> |
| <span data-ttu-id="08b55-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="08b55-111">storageUsedInBytes</span></span> | <span data-ttu-id="08b55-112">Int64</span><span class="sxs-lookup"><span data-stu-id="08b55-112">Int64</span></span>  |
| <span data-ttu-id="08b55-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="08b55-113">reportDate</span></span>         | <span data-ttu-id="08b55-114">Data</span><span class="sxs-lookup"><span data-stu-id="08b55-114">Date</span></span>   |
| <span data-ttu-id="08b55-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="08b55-115">reportPeriod</span></span>       | <span data-ttu-id="08b55-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08b55-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08b55-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08b55-117">JSON representation</span></span>

<span data-ttu-id="08b55-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08b55-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
