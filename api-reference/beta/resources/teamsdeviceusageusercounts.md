---
title: tipo de recurso teamsDeviceUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 02dc1b734e039e7c5eac7b8ffaed7a418e443c71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519866"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="60c37-103">tipo de recurso teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="60c37-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="60c37-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="60c37-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="60c37-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60c37-105">Properties</span></span>

| <span data-ttu-id="60c37-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60c37-106">Property</span></span>          | <span data-ttu-id="60c37-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="60c37-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="60c37-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="60c37-108">reportRefreshDate</span></span> | <span data-ttu-id="60c37-109">Data</span><span class="sxs-lookup"><span data-stu-id="60c37-109">Date</span></span>   |
| <span data-ttu-id="60c37-110">web</span><span class="sxs-lookup"><span data-stu-id="60c37-110">web</span></span>               | <span data-ttu-id="60c37-111">Int64</span><span class="sxs-lookup"><span data-stu-id="60c37-111">Int64</span></span>  |
| <span data-ttu-id="60c37-112">Windowsphonee</span><span class="sxs-lookup"><span data-stu-id="60c37-112">windowsPhone</span></span>      | <span data-ttu-id="60c37-113">Int64</span><span class="sxs-lookup"><span data-stu-id="60c37-113">Int64</span></span>  |
| <span data-ttu-id="60c37-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="60c37-114">androidPhone</span></span>      | <span data-ttu-id="60c37-115">Int64</span><span class="sxs-lookup"><span data-stu-id="60c37-115">Int64</span></span>  |
| <span data-ttu-id="60c37-116">emiti</span><span class="sxs-lookup"><span data-stu-id="60c37-116">ios</span></span>               | <span data-ttu-id="60c37-117">Int64</span><span class="sxs-lookup"><span data-stu-id="60c37-117">Int64</span></span>  |
| <span data-ttu-id="60c37-118">mac</span><span class="sxs-lookup"><span data-stu-id="60c37-118">mac</span></span>               | <span data-ttu-id="60c37-119">Int64</span><span class="sxs-lookup"><span data-stu-id="60c37-119">Int64</span></span>  |
| <span data-ttu-id="60c37-120">Windows</span><span class="sxs-lookup"><span data-stu-id="60c37-120">windows</span></span>           | <span data-ttu-id="60c37-121">Int64</span><span class="sxs-lookup"><span data-stu-id="60c37-121">Int64</span></span>  |
| <span data-ttu-id="60c37-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="60c37-122">reportDate</span></span>        | <span data-ttu-id="60c37-123">Data</span><span class="sxs-lookup"><span data-stu-id="60c37-123">Date</span></span>   |
| <span data-ttu-id="60c37-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="60c37-124">reportPeriod</span></span>      | <span data-ttu-id="60c37-125">String</span><span class="sxs-lookup"><span data-stu-id="60c37-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60c37-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60c37-126">JSON representation</span></span>

<span data-ttu-id="60c37-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60c37-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
