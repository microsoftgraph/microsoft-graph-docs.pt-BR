---
title: tipo de recurso emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6a8b6fd714b506404e7788a067fc655197f22ccc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440573"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="71e35-103">tipo de recurso emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="71e35-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="71e35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71e35-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="71e35-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71e35-105">Properties</span></span>

| <span data-ttu-id="71e35-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71e35-106">Property</span></span>          | <span data-ttu-id="71e35-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="71e35-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="71e35-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="71e35-108">reportRefreshDate</span></span> | <span data-ttu-id="71e35-109">Data</span><span class="sxs-lookup"><span data-stu-id="71e35-109">Date</span></span>   |
| <span data-ttu-id="71e35-110">send</span><span class="sxs-lookup"><span data-stu-id="71e35-110">send</span></span>              | <span data-ttu-id="71e35-111">Int64</span><span class="sxs-lookup"><span data-stu-id="71e35-111">Int64</span></span>  |
| <span data-ttu-id="71e35-112">receber</span><span class="sxs-lookup"><span data-stu-id="71e35-112">receive</span></span>           | <span data-ttu-id="71e35-113">Int64</span><span class="sxs-lookup"><span data-stu-id="71e35-113">Int64</span></span>  |
| <span data-ttu-id="71e35-114">Saiba</span><span class="sxs-lookup"><span data-stu-id="71e35-114">read</span></span>              | <span data-ttu-id="71e35-115">Int64</span><span class="sxs-lookup"><span data-stu-id="71e35-115">Int64</span></span>  |
| <span data-ttu-id="71e35-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="71e35-116">reportDate</span></span>        | <span data-ttu-id="71e35-117">Data</span><span class="sxs-lookup"><span data-stu-id="71e35-117">Date</span></span>   |
| <span data-ttu-id="71e35-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="71e35-118">reportPeriod</span></span>      | <span data-ttu-id="71e35-119">String</span><span class="sxs-lookup"><span data-stu-id="71e35-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71e35-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71e35-120">JSON representation</span></span>

<span data-ttu-id="71e35-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71e35-121">The following is a JSON representation of the resource.</span></span>

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
