---
title: tipo de recurso mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 40cc5f9b9cab7f17e185619d7fccdec028ae6250
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522831"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="81367-103">tipo de recurso mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="81367-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="81367-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="81367-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="81367-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81367-105">Properties</span></span>

| <span data-ttu-id="81367-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81367-106">Property</span></span>           | <span data-ttu-id="81367-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="81367-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="81367-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="81367-108">reportRefreshDate</span></span>  | <span data-ttu-id="81367-109">Data</span><span class="sxs-lookup"><span data-stu-id="81367-109">Date</span></span>   |
| <span data-ttu-id="81367-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="81367-110">storageUsedInBytes</span></span> | <span data-ttu-id="81367-111">Int64</span><span class="sxs-lookup"><span data-stu-id="81367-111">Int64</span></span>  |
| <span data-ttu-id="81367-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="81367-112">reportDate</span></span>         | <span data-ttu-id="81367-113">Data</span><span class="sxs-lookup"><span data-stu-id="81367-113">Date</span></span>   |
| <span data-ttu-id="81367-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="81367-114">reportPeriod</span></span>       | <span data-ttu-id="81367-115">String</span><span class="sxs-lookup"><span data-stu-id="81367-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81367-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81367-116">JSON representation</span></span>

<span data-ttu-id="81367-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81367-117">The following is a JSON representation of the resource.</span></span>

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
