---
title: tipo de recurso de yammerActivitySummary
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 6ff2b347de77f91c96cb5f5be797eb70db0bbbee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034097"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="00db5-103">tipo de recurso de yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="00db5-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="00db5-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00db5-104">Properties</span></span>

| <span data-ttu-id="00db5-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00db5-105">Property</span></span>          | <span data-ttu-id="00db5-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="00db5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="00db5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="00db5-107">reportRefreshDate</span></span> | <span data-ttu-id="00db5-108">Data</span><span class="sxs-lookup"><span data-stu-id="00db5-108">Date</span></span>   |
| <span data-ttu-id="00db5-109">curtidas</span><span class="sxs-lookup"><span data-stu-id="00db5-109">liked</span></span>             | <span data-ttu-id="00db5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="00db5-110">Int64</span></span>  |
| <span data-ttu-id="00db5-111">lançada</span><span class="sxs-lookup"><span data-stu-id="00db5-111">posted</span></span>            | <span data-ttu-id="00db5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="00db5-112">Int64</span></span>  |
| <span data-ttu-id="00db5-113">leitura</span><span class="sxs-lookup"><span data-stu-id="00db5-113">read</span></span>              | <span data-ttu-id="00db5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="00db5-114">Int64</span></span>  |
| <span data-ttu-id="00db5-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="00db5-115">reportDate</span></span>        | <span data-ttu-id="00db5-116">Data</span><span class="sxs-lookup"><span data-stu-id="00db5-116">Date</span></span>   |
| <span data-ttu-id="00db5-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="00db5-117">reportPeriod</span></span>      | <span data-ttu-id="00db5-118">String</span><span class="sxs-lookup"><span data-stu-id="00db5-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="00db5-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00db5-119">JSON representation</span></span>

<span data-ttu-id="00db5-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00db5-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
