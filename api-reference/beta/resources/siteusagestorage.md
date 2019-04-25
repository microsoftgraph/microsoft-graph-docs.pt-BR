---
title: tipo de recurso siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583197"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="bddbc-103">tipo de recurso siteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="bddbc-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bddbc-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bddbc-104">Properties</span></span>

| <span data-ttu-id="bddbc-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bddbc-105">Property</span></span>           | <span data-ttu-id="bddbc-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="bddbc-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="bddbc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bddbc-107">reportRefreshDate</span></span>  | <span data-ttu-id="bddbc-108">Data</span><span class="sxs-lookup"><span data-stu-id="bddbc-108">Date</span></span>   |
| <span data-ttu-id="bddbc-109">sitetype</span><span class="sxs-lookup"><span data-stu-id="bddbc-109">siteType</span></span>           | <span data-ttu-id="bddbc-110">String</span><span class="sxs-lookup"><span data-stu-id="bddbc-110">String</span></span> |
| <span data-ttu-id="bddbc-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="bddbc-111">storageUsedInBytes</span></span> | <span data-ttu-id="bddbc-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bddbc-112">Int64</span></span>  |
| <span data-ttu-id="bddbc-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="bddbc-113">reportDate</span></span>         | <span data-ttu-id="bddbc-114">Data</span><span class="sxs-lookup"><span data-stu-id="bddbc-114">Date</span></span>   |
| <span data-ttu-id="bddbc-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bddbc-115">reportPeriod</span></span>       | <span data-ttu-id="bddbc-116">String</span><span class="sxs-lookup"><span data-stu-id="bddbc-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bddbc-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bddbc-117">JSON representation</span></span>

<span data-ttu-id="bddbc-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bddbc-118">The following is a JSON representation of the resource.</span></span>

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
