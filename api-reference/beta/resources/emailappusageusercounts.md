---
title: tipo de recurso de emailAppUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: c8669c8a34987bc1e71152ae717f9be3ba101107
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038545"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="4cdb7-103">tipo de recurso de emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="4cdb7-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4cdb7-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cdb7-104">Properties</span></span>

| <span data-ttu-id="4cdb7-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cdb7-105">Property</span></span>          | <span data-ttu-id="4cdb7-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cdb7-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4cdb7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4cdb7-107">reportRefreshDate</span></span> | <span data-ttu-id="4cdb7-108">Data</span><span class="sxs-lookup"><span data-stu-id="4cdb7-108">Date</span></span>   |
| <span data-ttu-id="4cdb7-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="4cdb7-109">mailForMac</span></span>        | <span data-ttu-id="4cdb7-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-110">Int64</span></span>  |
| <span data-ttu-id="4cdb7-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="4cdb7-111">outlookForMac</span></span>     | <span data-ttu-id="4cdb7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-112">Int64</span></span>  |
| <span data-ttu-id="4cdb7-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="4cdb7-113">outlookForWindows</span></span> | <span data-ttu-id="4cdb7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-114">Int64</span></span>  |
| <span data-ttu-id="4cdb7-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="4cdb7-115">outlookForMobile</span></span>  | <span data-ttu-id="4cdb7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-116">Int64</span></span>  |
| <span data-ttu-id="4cdb7-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="4cdb7-117">otherForMobile</span></span>    | <span data-ttu-id="4cdb7-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-118">Int64</span></span>  |
| <span data-ttu-id="4cdb7-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="4cdb7-119">outlookForWeb</span></span>     | <span data-ttu-id="4cdb7-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-120">Int64</span></span>  |
| <span data-ttu-id="4cdb7-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="4cdb7-121">pop3App</span></span>           | <span data-ttu-id="4cdb7-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-122">Int64</span></span>  |
| <span data-ttu-id="4cdb7-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="4cdb7-123">imap4App</span></span>          | <span data-ttu-id="4cdb7-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-124">Int64</span></span>  |
| <span data-ttu-id="4cdb7-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="4cdb7-125">smtpApp</span></span>           | <span data-ttu-id="4cdb7-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4cdb7-126">Int64</span></span>  |
| <span data-ttu-id="4cdb7-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="4cdb7-127">reportDate</span></span>        | <span data-ttu-id="4cdb7-128">Data</span><span class="sxs-lookup"><span data-stu-id="4cdb7-128">Date</span></span>   |
| <span data-ttu-id="4cdb7-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4cdb7-129">reportPeriod</span></span>      | <span data-ttu-id="4cdb7-130">String</span><span class="sxs-lookup"><span data-stu-id="4cdb7-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4cdb7-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cdb7-131">JSON representation</span></span>

<span data-ttu-id="4cdb7-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4cdb7-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
