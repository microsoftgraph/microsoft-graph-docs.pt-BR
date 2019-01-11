---
title: tipo de recurso de emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: efbc4ce75293237813e9a835cb45ff0bf0ec4b26
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807816"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="449e8-103">tipo de recurso de emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="449e8-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="449e8-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="449e8-104">Properties</span></span>

| <span data-ttu-id="449e8-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="449e8-105">Property</span></span>          | <span data-ttu-id="449e8-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="449e8-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="449e8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="449e8-107">reportRefreshDate</span></span> | <span data-ttu-id="449e8-108">Data</span><span class="sxs-lookup"><span data-stu-id="449e8-108">Date</span></span>   |
| <span data-ttu-id="449e8-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="449e8-109">mailForMac</span></span>        | <span data-ttu-id="449e8-110">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-110">Int64</span></span>  |
| <span data-ttu-id="449e8-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="449e8-111">outlookForMac</span></span>     | <span data-ttu-id="449e8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-112">Int64</span></span>  |
| <span data-ttu-id="449e8-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="449e8-113">outlookForWindows</span></span> | <span data-ttu-id="449e8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-114">Int64</span></span>  |
| <span data-ttu-id="449e8-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="449e8-115">outlookForMobile</span></span>  | <span data-ttu-id="449e8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-116">Int64</span></span>  |
| <span data-ttu-id="449e8-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="449e8-117">otherForMobile</span></span>    | <span data-ttu-id="449e8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-118">Int64</span></span>  |
| <span data-ttu-id="449e8-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="449e8-119">outlookForWeb</span></span>     | <span data-ttu-id="449e8-120">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-120">Int64</span></span>  |
| <span data-ttu-id="449e8-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="449e8-121">pop3App</span></span>           | <span data-ttu-id="449e8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-122">Int64</span></span>  |
| <span data-ttu-id="449e8-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="449e8-123">imap4App</span></span>          | <span data-ttu-id="449e8-124">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-124">Int64</span></span>  |
| <span data-ttu-id="449e8-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="449e8-125">smtpApp</span></span>           | <span data-ttu-id="449e8-126">Int64</span><span class="sxs-lookup"><span data-stu-id="449e8-126">Int64</span></span>  |
| <span data-ttu-id="449e8-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="449e8-127">reportPeriod</span></span>      | <span data-ttu-id="449e8-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="449e8-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="449e8-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="449e8-129">JSON representation</span></span>

<span data-ttu-id="449e8-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="449e8-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportPeriod": "String"
}
```
