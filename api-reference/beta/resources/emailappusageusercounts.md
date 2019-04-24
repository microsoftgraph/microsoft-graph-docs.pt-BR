---
title: tipo de recurso emailAppUsageUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7822528aacc9d6f104012d43004fbb9aabba127c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506689"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="71e42-103">tipo de recurso emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="71e42-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="71e42-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71e42-104">Properties</span></span>

| <span data-ttu-id="71e42-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71e42-105">Property</span></span>          | <span data-ttu-id="71e42-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="71e42-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="71e42-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="71e42-107">reportRefreshDate</span></span> | <span data-ttu-id="71e42-108">Data</span><span class="sxs-lookup"><span data-stu-id="71e42-108">Date</span></span>   |
| <span data-ttu-id="71e42-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="71e42-109">mailForMac</span></span>        | <span data-ttu-id="71e42-110">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-110">Int64</span></span>  |
| <span data-ttu-id="71e42-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="71e42-111">outlookForMac</span></span>     | <span data-ttu-id="71e42-112">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-112">Int64</span></span>  |
| <span data-ttu-id="71e42-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="71e42-113">outlookForWindows</span></span> | <span data-ttu-id="71e42-114">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-114">Int64</span></span>  |
| <span data-ttu-id="71e42-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="71e42-115">outlookForMobile</span></span>  | <span data-ttu-id="71e42-116">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-116">Int64</span></span>  |
| <span data-ttu-id="71e42-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="71e42-117">otherForMobile</span></span>    | <span data-ttu-id="71e42-118">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-118">Int64</span></span>  |
| <span data-ttu-id="71e42-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="71e42-119">outlookForWeb</span></span>     | <span data-ttu-id="71e42-120">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-120">Int64</span></span>  |
| <span data-ttu-id="71e42-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="71e42-121">pop3App</span></span>           | <span data-ttu-id="71e42-122">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-122">Int64</span></span>  |
| <span data-ttu-id="71e42-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="71e42-123">imap4App</span></span>          | <span data-ttu-id="71e42-124">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-124">Int64</span></span>  |
| <span data-ttu-id="71e42-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="71e42-125">smtpApp</span></span>           | <span data-ttu-id="71e42-126">Int64</span><span class="sxs-lookup"><span data-stu-id="71e42-126">Int64</span></span>  |
| <span data-ttu-id="71e42-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="71e42-127">reportDate</span></span>        | <span data-ttu-id="71e42-128">Data</span><span class="sxs-lookup"><span data-stu-id="71e42-128">Date</span></span>   |
| <span data-ttu-id="71e42-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="71e42-129">reportPeriod</span></span>      | <span data-ttu-id="71e42-130">String</span><span class="sxs-lookup"><span data-stu-id="71e42-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71e42-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71e42-131">JSON representation</span></span>

<span data-ttu-id="71e42-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71e42-132">The following is a JSON representation of the resource.</span></span>

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
