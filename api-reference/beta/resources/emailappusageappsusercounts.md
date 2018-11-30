---
title: tipo de recurso de emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: e588a671129c6aa131bce781e3a6db0d44128f6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036006"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="87e30-103">tipo de recurso de emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="87e30-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="87e30-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87e30-104">Properties</span></span>

| <span data-ttu-id="87e30-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87e30-105">Property</span></span>          | <span data-ttu-id="87e30-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="87e30-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="87e30-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="87e30-107">reportRefreshDate</span></span> | <span data-ttu-id="87e30-108">Data</span><span class="sxs-lookup"><span data-stu-id="87e30-108">Date</span></span>   |
| <span data-ttu-id="87e30-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="87e30-109">mailForMac</span></span>        | <span data-ttu-id="87e30-110">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-110">Int64</span></span>  |
| <span data-ttu-id="87e30-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="87e30-111">outlookForMac</span></span>     | <span data-ttu-id="87e30-112">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-112">Int64</span></span>  |
| <span data-ttu-id="87e30-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="87e30-113">outlookForWindows</span></span> | <span data-ttu-id="87e30-114">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-114">Int64</span></span>  |
| <span data-ttu-id="87e30-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="87e30-115">outlookForMobile</span></span>  | <span data-ttu-id="87e30-116">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-116">Int64</span></span>  |
| <span data-ttu-id="87e30-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="87e30-117">otherForMobile</span></span>    | <span data-ttu-id="87e30-118">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-118">Int64</span></span>  |
| <span data-ttu-id="87e30-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="87e30-119">outlookForWeb</span></span>     | <span data-ttu-id="87e30-120">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-120">Int64</span></span>  |
| <span data-ttu-id="87e30-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="87e30-121">pop3App</span></span>           | <span data-ttu-id="87e30-122">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-122">Int64</span></span>  |
| <span data-ttu-id="87e30-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="87e30-123">imap4App</span></span>          | <span data-ttu-id="87e30-124">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-124">Int64</span></span>  |
| <span data-ttu-id="87e30-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="87e30-125">smtpApp</span></span>           | <span data-ttu-id="87e30-126">Int64</span><span class="sxs-lookup"><span data-stu-id="87e30-126">Int64</span></span>  |
| <span data-ttu-id="87e30-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="87e30-127">reportPeriod</span></span>      | <span data-ttu-id="87e30-128">String</span><span class="sxs-lookup"><span data-stu-id="87e30-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87e30-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87e30-129">JSON representation</span></span>

<span data-ttu-id="87e30-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87e30-130">The following is a JSON representation of the resource.</span></span>

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
