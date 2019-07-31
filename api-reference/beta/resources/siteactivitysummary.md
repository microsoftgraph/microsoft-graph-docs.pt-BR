---
title: tipo de recurso siteActivitySummary
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1258530aea56f7ec26a2f48274935afc809f2fd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965016"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="50111-103">tipo de recurso siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="50111-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="50111-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50111-104">Properties</span></span>

| <span data-ttu-id="50111-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50111-105">Property</span></span>          | <span data-ttu-id="50111-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="50111-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="50111-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="50111-107">reportRefreshDate</span></span> | <span data-ttu-id="50111-108">Data</span><span class="sxs-lookup"><span data-stu-id="50111-108">Date</span></span>   |
| <span data-ttu-id="50111-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="50111-109">viewedOrEdited</span></span>    | <span data-ttu-id="50111-110">Int64</span><span class="sxs-lookup"><span data-stu-id="50111-110">Int64</span></span>  |
| <span data-ttu-id="50111-111">sincronizados</span><span class="sxs-lookup"><span data-stu-id="50111-111">synced</span></span>            | <span data-ttu-id="50111-112">Int64</span><span class="sxs-lookup"><span data-stu-id="50111-112">Int64</span></span>  |
| <span data-ttu-id="50111-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="50111-113">sharedInternally</span></span>  | <span data-ttu-id="50111-114">Int64</span><span class="sxs-lookup"><span data-stu-id="50111-114">Int64</span></span>  |
| <span data-ttu-id="50111-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="50111-115">sharedExternally</span></span>  | <span data-ttu-id="50111-116">Int64</span><span class="sxs-lookup"><span data-stu-id="50111-116">Int64</span></span>  |
| <span data-ttu-id="50111-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="50111-117">reportDate</span></span>        | <span data-ttu-id="50111-118">Data</span><span class="sxs-lookup"><span data-stu-id="50111-118">Date</span></span>   |
| <span data-ttu-id="50111-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="50111-119">reportPeriod</span></span>      | <span data-ttu-id="50111-120">String</span><span class="sxs-lookup"><span data-stu-id="50111-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50111-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50111-121">JSON representation</span></span>

<span data-ttu-id="50111-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50111-122">The following is a JSON representation of the resource.</span></span>

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
