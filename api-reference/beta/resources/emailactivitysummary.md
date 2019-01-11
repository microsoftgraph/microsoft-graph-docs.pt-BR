---
title: tipo de recurso de emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 82fbdc2621b9c8746ed3028fe44414edeb7e56db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871341"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="ae8aa-103">tipo de recurso de emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="ae8aa-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ae8aa-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae8aa-104">Properties</span></span>

| <span data-ttu-id="ae8aa-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae8aa-105">Property</span></span>          | <span data-ttu-id="ae8aa-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae8aa-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ae8aa-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ae8aa-107">reportRefreshDate</span></span> | <span data-ttu-id="ae8aa-108">Data</span><span class="sxs-lookup"><span data-stu-id="ae8aa-108">Date</span></span>   |
| <span data-ttu-id="ae8aa-109">enviar</span><span class="sxs-lookup"><span data-stu-id="ae8aa-109">send</span></span>              | <span data-ttu-id="ae8aa-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ae8aa-110">Int64</span></span>  |
| <span data-ttu-id="ae8aa-111">receber</span><span class="sxs-lookup"><span data-stu-id="ae8aa-111">receive</span></span>           | <span data-ttu-id="ae8aa-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ae8aa-112">Int64</span></span>  |
| <span data-ttu-id="ae8aa-113">leitura</span><span class="sxs-lookup"><span data-stu-id="ae8aa-113">read</span></span>              | <span data-ttu-id="ae8aa-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ae8aa-114">Int64</span></span>  |
| <span data-ttu-id="ae8aa-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="ae8aa-115">reportDate</span></span>        | <span data-ttu-id="ae8aa-116">Data</span><span class="sxs-lookup"><span data-stu-id="ae8aa-116">Date</span></span>   |
| <span data-ttu-id="ae8aa-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ae8aa-117">reportPeriod</span></span>      | <span data-ttu-id="ae8aa-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae8aa-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae8aa-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae8aa-119">JSON representation</span></span>

<span data-ttu-id="ae8aa-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae8aa-120">The following is a JSON representation of the resource.</span></span>

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
