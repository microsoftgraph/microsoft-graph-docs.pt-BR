---
title: tipo de recurso de siteActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 2eb5bdb89924338d1d352ea80bd516b8fb948250
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817763"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="eadbb-103">tipo de recurso de siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="eadbb-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="eadbb-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eadbb-104">Properties</span></span>

| <span data-ttu-id="eadbb-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eadbb-105">Property</span></span>          | <span data-ttu-id="eadbb-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="eadbb-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="eadbb-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="eadbb-107">reportRefreshDate</span></span> | <span data-ttu-id="eadbb-108">Data</span><span class="sxs-lookup"><span data-stu-id="eadbb-108">Date</span></span>   |
| <span data-ttu-id="eadbb-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="eadbb-109">viewedOrEdited</span></span>    | <span data-ttu-id="eadbb-110">Int64</span><span class="sxs-lookup"><span data-stu-id="eadbb-110">Int64</span></span>  |
| <span data-ttu-id="eadbb-111">sincronizados</span><span class="sxs-lookup"><span data-stu-id="eadbb-111">synced</span></span>            | <span data-ttu-id="eadbb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="eadbb-112">Int64</span></span>  |
| <span data-ttu-id="eadbb-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="eadbb-113">sharedInternally</span></span>  | <span data-ttu-id="eadbb-114">Int64</span><span class="sxs-lookup"><span data-stu-id="eadbb-114">Int64</span></span>  |
| <span data-ttu-id="eadbb-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="eadbb-115">sharedExternally</span></span>  | <span data-ttu-id="eadbb-116">Int64</span><span class="sxs-lookup"><span data-stu-id="eadbb-116">Int64</span></span>  |
| <span data-ttu-id="eadbb-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="eadbb-117">reportDate</span></span>        | <span data-ttu-id="eadbb-118">Data</span><span class="sxs-lookup"><span data-stu-id="eadbb-118">Date</span></span>   |
| <span data-ttu-id="eadbb-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="eadbb-119">reportPeriod</span></span>      | <span data-ttu-id="eadbb-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eadbb-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eadbb-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eadbb-121">JSON representation</span></span>

<span data-ttu-id="eadbb-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eadbb-122">The following is a JSON representation of the resource.</span></span>

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
