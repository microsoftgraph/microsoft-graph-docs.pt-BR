---
title: tipo de recurso siteActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: f629d8b60179e83515af1e9fa5d86e55e7681f17
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807903"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="41a81-103">tipo de recurso siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="41a81-103">siteActivitySummary resource type</span></span>

<span data-ttu-id="41a81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41a81-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="41a81-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41a81-105">Properties</span></span>

| <span data-ttu-id="41a81-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41a81-106">Property</span></span>          | <span data-ttu-id="41a81-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="41a81-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="41a81-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="41a81-108">reportRefreshDate</span></span> | <span data-ttu-id="41a81-109">Data</span><span class="sxs-lookup"><span data-stu-id="41a81-109">Date</span></span>   |
| <span data-ttu-id="41a81-110">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="41a81-110">viewedOrEdited</span></span>    | <span data-ttu-id="41a81-111">Int64</span><span class="sxs-lookup"><span data-stu-id="41a81-111">Int64</span></span>  |
| <span data-ttu-id="41a81-112">sincronizados</span><span class="sxs-lookup"><span data-stu-id="41a81-112">synced</span></span>            | <span data-ttu-id="41a81-113">Int64</span><span class="sxs-lookup"><span data-stu-id="41a81-113">Int64</span></span>  |
| <span data-ttu-id="41a81-114">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="41a81-114">sharedInternally</span></span>  | <span data-ttu-id="41a81-115">Int64</span><span class="sxs-lookup"><span data-stu-id="41a81-115">Int64</span></span>  |
| <span data-ttu-id="41a81-116">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="41a81-116">sharedExternally</span></span>  | <span data-ttu-id="41a81-117">Int64</span><span class="sxs-lookup"><span data-stu-id="41a81-117">Int64</span></span>  |
| <span data-ttu-id="41a81-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="41a81-118">reportDate</span></span>        | <span data-ttu-id="41a81-119">Data</span><span class="sxs-lookup"><span data-stu-id="41a81-119">Date</span></span>   |
| <span data-ttu-id="41a81-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="41a81-120">reportPeriod</span></span>      | <span data-ttu-id="41a81-121">String</span><span class="sxs-lookup"><span data-stu-id="41a81-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41a81-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41a81-122">JSON representation</span></span>

<span data-ttu-id="41a81-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41a81-123">The following is a JSON representation of the resource.</span></span>

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
