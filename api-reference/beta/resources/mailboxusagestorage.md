---
title: tipo de recurso mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 080b1e5eafb23e40df1307fc6ab3e9a4ef9c87f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075529"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="d4f22-103">tipo de recurso mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="d4f22-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="d4f22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4f22-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d4f22-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4f22-105">Properties</span></span>

| <span data-ttu-id="d4f22-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4f22-106">Property</span></span>           | <span data-ttu-id="d4f22-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4f22-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="d4f22-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d4f22-108">reportRefreshDate</span></span>  | <span data-ttu-id="d4f22-109">Data</span><span class="sxs-lookup"><span data-stu-id="d4f22-109">Date</span></span>   |
| <span data-ttu-id="d4f22-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d4f22-110">storageUsedInBytes</span></span> | <span data-ttu-id="d4f22-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d4f22-111">Int64</span></span>  |
| <span data-ttu-id="d4f22-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="d4f22-112">reportDate</span></span>         | <span data-ttu-id="d4f22-113">Data</span><span class="sxs-lookup"><span data-stu-id="d4f22-113">Date</span></span>   |
| <span data-ttu-id="d4f22-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d4f22-114">reportPeriod</span></span>       | <span data-ttu-id="d4f22-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4f22-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4f22-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4f22-116">JSON representation</span></span>

<span data-ttu-id="d4f22-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4f22-117">The following is a JSON representation of the resource.</span></span>

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


