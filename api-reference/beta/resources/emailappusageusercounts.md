---
title: tipo de recurso de emailAppUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7822528aacc9d6f104012d43004fbb9aabba127c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990800"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="ca566-103">tipo de recurso de emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ca566-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ca566-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca566-104">Properties</span></span>

| <span data-ttu-id="ca566-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca566-105">Property</span></span>          | <span data-ttu-id="ca566-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca566-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ca566-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ca566-107">reportRefreshDate</span></span> | <span data-ttu-id="ca566-108">Data</span><span class="sxs-lookup"><span data-stu-id="ca566-108">Date</span></span>   |
| <span data-ttu-id="ca566-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="ca566-109">mailForMac</span></span>        | <span data-ttu-id="ca566-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-110">Int64</span></span>  |
| <span data-ttu-id="ca566-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="ca566-111">outlookForMac</span></span>     | <span data-ttu-id="ca566-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-112">Int64</span></span>  |
| <span data-ttu-id="ca566-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="ca566-113">outlookForWindows</span></span> | <span data-ttu-id="ca566-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-114">Int64</span></span>  |
| <span data-ttu-id="ca566-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="ca566-115">outlookForMobile</span></span>  | <span data-ttu-id="ca566-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-116">Int64</span></span>  |
| <span data-ttu-id="ca566-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="ca566-117">otherForMobile</span></span>    | <span data-ttu-id="ca566-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-118">Int64</span></span>  |
| <span data-ttu-id="ca566-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="ca566-119">outlookForWeb</span></span>     | <span data-ttu-id="ca566-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-120">Int64</span></span>  |
| <span data-ttu-id="ca566-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="ca566-121">pop3App</span></span>           | <span data-ttu-id="ca566-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-122">Int64</span></span>  |
| <span data-ttu-id="ca566-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="ca566-123">imap4App</span></span>          | <span data-ttu-id="ca566-124">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-124">Int64</span></span>  |
| <span data-ttu-id="ca566-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="ca566-125">smtpApp</span></span>           | <span data-ttu-id="ca566-126">Int64</span><span class="sxs-lookup"><span data-stu-id="ca566-126">Int64</span></span>  |
| <span data-ttu-id="ca566-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="ca566-127">reportDate</span></span>        | <span data-ttu-id="ca566-128">Data</span><span class="sxs-lookup"><span data-stu-id="ca566-128">Date</span></span>   |
| <span data-ttu-id="ca566-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ca566-129">reportPeriod</span></span>      | <span data-ttu-id="ca566-130">String</span><span class="sxs-lookup"><span data-stu-id="ca566-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ca566-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca566-131">JSON representation</span></span>

<span data-ttu-id="ca566-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca566-132">The following is a JSON representation of the resource.</span></span>

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
