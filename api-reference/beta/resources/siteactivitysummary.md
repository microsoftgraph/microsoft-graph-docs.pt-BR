---
title: tipo de recurso siteActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a49b8e47ca2a6efcc5c5c87702fdea0122b208e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583596"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="ad4d1-103">tipo de recurso siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="ad4d1-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ad4d1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad4d1-104">Properties</span></span>

| <span data-ttu-id="ad4d1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad4d1-105">Property</span></span>          | <span data-ttu-id="ad4d1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad4d1-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ad4d1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ad4d1-107">reportRefreshDate</span></span> | <span data-ttu-id="ad4d1-108">Data</span><span class="sxs-lookup"><span data-stu-id="ad4d1-108">Date</span></span>   |
| <span data-ttu-id="ad4d1-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="ad4d1-109">viewedOrEdited</span></span>    | <span data-ttu-id="ad4d1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ad4d1-110">Int64</span></span>  |
| <span data-ttu-id="ad4d1-111">sincronizados</span><span class="sxs-lookup"><span data-stu-id="ad4d1-111">synced</span></span>            | <span data-ttu-id="ad4d1-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ad4d1-112">Int64</span></span>  |
| <span data-ttu-id="ad4d1-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="ad4d1-113">sharedInternally</span></span>  | <span data-ttu-id="ad4d1-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ad4d1-114">Int64</span></span>  |
| <span data-ttu-id="ad4d1-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="ad4d1-115">sharedExternally</span></span>  | <span data-ttu-id="ad4d1-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ad4d1-116">Int64</span></span>  |
| <span data-ttu-id="ad4d1-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="ad4d1-117">reportDate</span></span>        | <span data-ttu-id="ad4d1-118">Data</span><span class="sxs-lookup"><span data-stu-id="ad4d1-118">Date</span></span>   |
| <span data-ttu-id="ad4d1-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ad4d1-119">reportPeriod</span></span>      | <span data-ttu-id="ad4d1-120">String</span><span class="sxs-lookup"><span data-stu-id="ad4d1-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad4d1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad4d1-121">JSON representation</span></span>

<span data-ttu-id="ad4d1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad4d1-122">The following is a JSON representation of the resource.</span></span>

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
