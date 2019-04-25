---
title: tipo de recurso mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524542"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="853c5-103">tipo de recurso mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="853c5-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="853c5-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="853c5-104">Properties</span></span>

| <span data-ttu-id="853c5-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="853c5-105">Property</span></span>           | <span data-ttu-id="853c5-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="853c5-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="853c5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="853c5-107">reportRefreshDate</span></span>  | <span data-ttu-id="853c5-108">Data</span><span class="sxs-lookup"><span data-stu-id="853c5-108">Date</span></span>   |
| <span data-ttu-id="853c5-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="853c5-109">storageUsedInBytes</span></span> | <span data-ttu-id="853c5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="853c5-110">Int64</span></span>  |
| <span data-ttu-id="853c5-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="853c5-111">reportDate</span></span>         | <span data-ttu-id="853c5-112">Data</span><span class="sxs-lookup"><span data-stu-id="853c5-112">Date</span></span>   |
| <span data-ttu-id="853c5-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="853c5-113">reportPeriod</span></span>       | <span data-ttu-id="853c5-114">String</span><span class="sxs-lookup"><span data-stu-id="853c5-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="853c5-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="853c5-115">JSON representation</span></span>

<span data-ttu-id="853c5-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="853c5-116">The following is a JSON representation of the resource.</span></span>

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
