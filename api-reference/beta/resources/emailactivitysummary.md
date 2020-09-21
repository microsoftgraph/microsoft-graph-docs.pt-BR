---
title: tipo de recurso emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 78853954ef7c6fe4a191cbccefca350e628db210
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989588"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="7185c-103">tipo de recurso emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="7185c-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="7185c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7185c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="7185c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7185c-105">Properties</span></span>

| <span data-ttu-id="7185c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7185c-106">Property</span></span>          | <span data-ttu-id="7185c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7185c-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7185c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7185c-108">reportRefreshDate</span></span> | <span data-ttu-id="7185c-109">Data</span><span class="sxs-lookup"><span data-stu-id="7185c-109">Date</span></span>   |
| <span data-ttu-id="7185c-110">send</span><span class="sxs-lookup"><span data-stu-id="7185c-110">send</span></span>              | <span data-ttu-id="7185c-111">Int64</span><span class="sxs-lookup"><span data-stu-id="7185c-111">Int64</span></span>  |
| <span data-ttu-id="7185c-112">receber</span><span class="sxs-lookup"><span data-stu-id="7185c-112">receive</span></span>           | <span data-ttu-id="7185c-113">Int64</span><span class="sxs-lookup"><span data-stu-id="7185c-113">Int64</span></span>  |
| <span data-ttu-id="7185c-114">leitura</span><span class="sxs-lookup"><span data-stu-id="7185c-114">read</span></span>              | <span data-ttu-id="7185c-115">Int64</span><span class="sxs-lookup"><span data-stu-id="7185c-115">Int64</span></span>  |
| <span data-ttu-id="7185c-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="7185c-116">reportDate</span></span>        | <span data-ttu-id="7185c-117">Data</span><span class="sxs-lookup"><span data-stu-id="7185c-117">Date</span></span>   |
| <span data-ttu-id="7185c-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7185c-118">reportPeriod</span></span>      | <span data-ttu-id="7185c-119">String</span><span class="sxs-lookup"><span data-stu-id="7185c-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7185c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7185c-120">JSON representation</span></span>

<span data-ttu-id="7185c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7185c-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


