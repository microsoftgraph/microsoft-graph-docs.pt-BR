---
title: tipo de recurso mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6f4ee4b29c82102db96cd4d71718f7da449776b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009836"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="8b040-103">tipo de recurso mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="8b040-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8b040-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b040-104">Properties</span></span>

| <span data-ttu-id="8b040-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b040-105">Property</span></span>           | <span data-ttu-id="8b040-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b040-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="8b040-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8b040-107">reportRefreshDate</span></span>  | <span data-ttu-id="8b040-108">Data</span><span class="sxs-lookup"><span data-stu-id="8b040-108">Date</span></span>   |
| <span data-ttu-id="8b040-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="8b040-109">storageUsedInBytes</span></span> | <span data-ttu-id="8b040-110">Int64</span><span class="sxs-lookup"><span data-stu-id="8b040-110">Int64</span></span>  |
| <span data-ttu-id="8b040-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="8b040-111">reportDate</span></span>         | <span data-ttu-id="8b040-112">Data</span><span class="sxs-lookup"><span data-stu-id="8b040-112">Date</span></span>   |
| <span data-ttu-id="8b040-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8b040-113">reportPeriod</span></span>       | <span data-ttu-id="8b040-114">String</span><span class="sxs-lookup"><span data-stu-id="8b040-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8b040-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b040-115">JSON representation</span></span>

<span data-ttu-id="8b040-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b040-116">The following is a JSON representation of the resource.</span></span>

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
