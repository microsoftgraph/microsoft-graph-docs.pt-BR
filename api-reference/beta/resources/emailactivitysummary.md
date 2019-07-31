---
title: tipo de recurso emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 64c9468d79a93b6f82fff0f04206a0fb6e95e4fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972219"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="74e5d-103">tipo de recurso emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="74e5d-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="74e5d-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74e5d-104">Properties</span></span>

| <span data-ttu-id="74e5d-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74e5d-105">Property</span></span>          | <span data-ttu-id="74e5d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="74e5d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="74e5d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="74e5d-107">reportRefreshDate</span></span> | <span data-ttu-id="74e5d-108">Data</span><span class="sxs-lookup"><span data-stu-id="74e5d-108">Date</span></span>   |
| <span data-ttu-id="74e5d-109">Enviar</span><span class="sxs-lookup"><span data-stu-id="74e5d-109">send</span></span>              | <span data-ttu-id="74e5d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="74e5d-110">Int64</span></span>  |
| <span data-ttu-id="74e5d-111">receber</span><span class="sxs-lookup"><span data-stu-id="74e5d-111">receive</span></span>           | <span data-ttu-id="74e5d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="74e5d-112">Int64</span></span>  |
| <span data-ttu-id="74e5d-113">Saiba</span><span class="sxs-lookup"><span data-stu-id="74e5d-113">read</span></span>              | <span data-ttu-id="74e5d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="74e5d-114">Int64</span></span>  |
| <span data-ttu-id="74e5d-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="74e5d-115">reportDate</span></span>        | <span data-ttu-id="74e5d-116">Data</span><span class="sxs-lookup"><span data-stu-id="74e5d-116">Date</span></span>   |
| <span data-ttu-id="74e5d-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="74e5d-117">reportPeriod</span></span>      | <span data-ttu-id="74e5d-118">String</span><span class="sxs-lookup"><span data-stu-id="74e5d-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="74e5d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74e5d-119">JSON representation</span></span>

<span data-ttu-id="74e5d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74e5d-120">The following is a JSON representation of the resource.</span></span>

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
