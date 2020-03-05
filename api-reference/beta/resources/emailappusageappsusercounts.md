---
title: tipo de recurso emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34ceaf4450a66f07c0678e55db344adc20bb0b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499495"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="48883-103">tipo de recurso emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="48883-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="48883-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="48883-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="48883-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48883-105">Properties</span></span>

| <span data-ttu-id="48883-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48883-106">Property</span></span>          | <span data-ttu-id="48883-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="48883-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="48883-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="48883-108">reportRefreshDate</span></span> | <span data-ttu-id="48883-109">Data</span><span class="sxs-lookup"><span data-stu-id="48883-109">Date</span></span>   |
| <span data-ttu-id="48883-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="48883-110">mailForMac</span></span>        | <span data-ttu-id="48883-111">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-111">Int64</span></span>  |
| <span data-ttu-id="48883-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="48883-112">outlookForMac</span></span>     | <span data-ttu-id="48883-113">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-113">Int64</span></span>  |
| <span data-ttu-id="48883-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="48883-114">outlookForWindows</span></span> | <span data-ttu-id="48883-115">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-115">Int64</span></span>  |
| <span data-ttu-id="48883-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="48883-116">outlookForMobile</span></span>  | <span data-ttu-id="48883-117">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-117">Int64</span></span>  |
| <span data-ttu-id="48883-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="48883-118">otherForMobile</span></span>    | <span data-ttu-id="48883-119">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-119">Int64</span></span>  |
| <span data-ttu-id="48883-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="48883-120">outlookForWeb</span></span>     | <span data-ttu-id="48883-121">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-121">Int64</span></span>  |
| <span data-ttu-id="48883-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="48883-122">pop3App</span></span>           | <span data-ttu-id="48883-123">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-123">Int64</span></span>  |
| <span data-ttu-id="48883-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="48883-124">imap4App</span></span>          | <span data-ttu-id="48883-125">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-125">Int64</span></span>  |
| <span data-ttu-id="48883-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="48883-126">smtpApp</span></span>           | <span data-ttu-id="48883-127">Int64</span><span class="sxs-lookup"><span data-stu-id="48883-127">Int64</span></span>  |
| <span data-ttu-id="48883-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="48883-128">reportPeriod</span></span>      | <span data-ttu-id="48883-129">String</span><span class="sxs-lookup"><span data-stu-id="48883-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="48883-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48883-130">JSON representation</span></span>

<span data-ttu-id="48883-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48883-131">The following is a JSON representation of the resource.</span></span>

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
