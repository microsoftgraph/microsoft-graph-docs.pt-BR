---
title: tipo de recurso de mailboxUsageMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e9da6a72c3c2d79323041e683702a7af2e4699c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941307"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="5748f-103">tipo de recurso de mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="5748f-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5748f-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5748f-104">Properties</span></span>

| <span data-ttu-id="5748f-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5748f-105">Property</span></span>          | <span data-ttu-id="5748f-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="5748f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5748f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5748f-107">reportRefreshDate</span></span> | <span data-ttu-id="5748f-108">Data</span><span class="sxs-lookup"><span data-stu-id="5748f-108">Date</span></span>   |
| <span data-ttu-id="5748f-109">total</span><span class="sxs-lookup"><span data-stu-id="5748f-109">total</span></span>             | <span data-ttu-id="5748f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5748f-110">Int64</span></span>  |
| <span data-ttu-id="5748f-111">ativo</span><span class="sxs-lookup"><span data-stu-id="5748f-111">active</span></span>            | <span data-ttu-id="5748f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5748f-112">Int64</span></span>  |
| <span data-ttu-id="5748f-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="5748f-113">reportDate</span></span>        | <span data-ttu-id="5748f-114">Data</span><span class="sxs-lookup"><span data-stu-id="5748f-114">Date</span></span>   |
| <span data-ttu-id="5748f-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5748f-115">reportPeriod</span></span>      | <span data-ttu-id="5748f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5748f-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5748f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5748f-117">JSON representation</span></span>

<span data-ttu-id="5748f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5748f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
