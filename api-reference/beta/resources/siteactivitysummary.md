---
title: tipo de recurso de siteActivitySummary
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 354b329f592964249590b2f551d66681f45de485
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036876"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="62378-103">tipo de recurso de siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="62378-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="62378-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62378-104">Properties</span></span>

| <span data-ttu-id="62378-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62378-105">Property</span></span>          | <span data-ttu-id="62378-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="62378-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="62378-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="62378-107">reportRefreshDate</span></span> | <span data-ttu-id="62378-108">Data</span><span class="sxs-lookup"><span data-stu-id="62378-108">Date</span></span>   |
| <span data-ttu-id="62378-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="62378-109">viewedOrEdited</span></span>    | <span data-ttu-id="62378-110">Int64</span><span class="sxs-lookup"><span data-stu-id="62378-110">Int64</span></span>  |
| <span data-ttu-id="62378-111">sincronizados</span><span class="sxs-lookup"><span data-stu-id="62378-111">synced</span></span>            | <span data-ttu-id="62378-112">Int64</span><span class="sxs-lookup"><span data-stu-id="62378-112">Int64</span></span>  |
| <span data-ttu-id="62378-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="62378-113">sharedInternally</span></span>  | <span data-ttu-id="62378-114">Int64</span><span class="sxs-lookup"><span data-stu-id="62378-114">Int64</span></span>  |
| <span data-ttu-id="62378-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="62378-115">sharedExternally</span></span>  | <span data-ttu-id="62378-116">Int64</span><span class="sxs-lookup"><span data-stu-id="62378-116">Int64</span></span>  |
| <span data-ttu-id="62378-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="62378-117">reportDate</span></span>        | <span data-ttu-id="62378-118">Data</span><span class="sxs-lookup"><span data-stu-id="62378-118">Date</span></span>   |
| <span data-ttu-id="62378-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="62378-119">reportPeriod</span></span>      | <span data-ttu-id="62378-120">String</span><span class="sxs-lookup"><span data-stu-id="62378-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62378-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62378-121">JSON representation</span></span>

<span data-ttu-id="62378-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62378-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
