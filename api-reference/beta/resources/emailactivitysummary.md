---
title: tipo de recurso de emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 84958874af09b31aafed694c1a62d080a5c798ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990086"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="4d94f-103">tipo de recurso de emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="4d94f-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4d94f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d94f-104">Properties</span></span>

| <span data-ttu-id="4d94f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d94f-105">Property</span></span>          | <span data-ttu-id="4d94f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d94f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4d94f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4d94f-107">reportRefreshDate</span></span> | <span data-ttu-id="4d94f-108">Data</span><span class="sxs-lookup"><span data-stu-id="4d94f-108">Date</span></span>   |
| <span data-ttu-id="4d94f-109">enviar</span><span class="sxs-lookup"><span data-stu-id="4d94f-109">send</span></span>              | <span data-ttu-id="4d94f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4d94f-110">Int64</span></span>  |
| <span data-ttu-id="4d94f-111">receber</span><span class="sxs-lookup"><span data-stu-id="4d94f-111">receive</span></span>           | <span data-ttu-id="4d94f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4d94f-112">Int64</span></span>  |
| <span data-ttu-id="4d94f-113">leitura</span><span class="sxs-lookup"><span data-stu-id="4d94f-113">read</span></span>              | <span data-ttu-id="4d94f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4d94f-114">Int64</span></span>  |
| <span data-ttu-id="4d94f-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="4d94f-115">reportDate</span></span>        | <span data-ttu-id="4d94f-116">Data</span><span class="sxs-lookup"><span data-stu-id="4d94f-116">Date</span></span>   |
| <span data-ttu-id="4d94f-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4d94f-117">reportPeriod</span></span>      | <span data-ttu-id="4d94f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d94f-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4d94f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d94f-119">JSON representation</span></span>

<span data-ttu-id="4d94f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d94f-120">The following is a JSON representation of the resource.</span></span>

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
