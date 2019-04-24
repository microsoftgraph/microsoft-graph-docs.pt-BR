---
title: tipo de recurso emailActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 84958874af09b31aafed694c1a62d080a5c798ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506668"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="5b260-103">tipo de recurso emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="5b260-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5b260-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b260-104">Properties</span></span>

| <span data-ttu-id="5b260-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b260-105">Property</span></span>          | <span data-ttu-id="5b260-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b260-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5b260-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5b260-107">reportRefreshDate</span></span> | <span data-ttu-id="5b260-108">Data</span><span class="sxs-lookup"><span data-stu-id="5b260-108">Date</span></span>   |
| <span data-ttu-id="5b260-109">Enviar</span><span class="sxs-lookup"><span data-stu-id="5b260-109">send</span></span>              | <span data-ttu-id="5b260-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5b260-110">Int64</span></span>  |
| <span data-ttu-id="5b260-111">receber</span><span class="sxs-lookup"><span data-stu-id="5b260-111">receive</span></span>           | <span data-ttu-id="5b260-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5b260-112">Int64</span></span>  |
| <span data-ttu-id="5b260-113">Saiba</span><span class="sxs-lookup"><span data-stu-id="5b260-113">read</span></span>              | <span data-ttu-id="5b260-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5b260-114">Int64</span></span>  |
| <span data-ttu-id="5b260-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="5b260-115">reportDate</span></span>        | <span data-ttu-id="5b260-116">Data</span><span class="sxs-lookup"><span data-stu-id="5b260-116">Date</span></span>   |
| <span data-ttu-id="5b260-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5b260-117">reportPeriod</span></span>      | <span data-ttu-id="5b260-118">String</span><span class="sxs-lookup"><span data-stu-id="5b260-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5b260-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b260-119">JSON representation</span></span>

<span data-ttu-id="5b260-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b260-120">The following is a JSON representation of the resource.</span></span>

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
