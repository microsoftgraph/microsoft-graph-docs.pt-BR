---
title: tipo de recurso de oneDriveUsageAccountCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 959d6602cec98f7351ec3d9819fb9a59599d3e6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037007"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="d00dd-103">tipo de recurso de oneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="d00dd-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d00dd-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d00dd-104">Properties</span></span>

| <span data-ttu-id="d00dd-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d00dd-105">Property</span></span>          | <span data-ttu-id="d00dd-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d00dd-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d00dd-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d00dd-107">reportRefreshDate</span></span> | <span data-ttu-id="d00dd-108">Data</span><span class="sxs-lookup"><span data-stu-id="d00dd-108">Date</span></span>   |
| <span data-ttu-id="d00dd-109">siteType</span><span class="sxs-lookup"><span data-stu-id="d00dd-109">siteType</span></span>          | <span data-ttu-id="d00dd-110">String</span><span class="sxs-lookup"><span data-stu-id="d00dd-110">String</span></span> |
| <span data-ttu-id="d00dd-111">total</span><span class="sxs-lookup"><span data-stu-id="d00dd-111">total</span></span>             | <span data-ttu-id="d00dd-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d00dd-112">Int64</span></span>  |
| <span data-ttu-id="d00dd-113">ativo</span><span class="sxs-lookup"><span data-stu-id="d00dd-113">active</span></span>            | <span data-ttu-id="d00dd-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d00dd-114">Int64</span></span>  |
| <span data-ttu-id="d00dd-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="d00dd-115">reportDate</span></span>        | <span data-ttu-id="d00dd-116">Data</span><span class="sxs-lookup"><span data-stu-id="d00dd-116">Date</span></span>   |
| <span data-ttu-id="d00dd-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d00dd-117">reportPeriod</span></span>      | <span data-ttu-id="d00dd-118">String</span><span class="sxs-lookup"><span data-stu-id="d00dd-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d00dd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d00dd-119">JSON representation</span></span>

<span data-ttu-id="d00dd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d00dd-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
