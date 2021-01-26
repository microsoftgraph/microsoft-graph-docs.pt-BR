---
title: Tipo de recurso emailAppUsageAppsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c6393d8f99d734c63c810622c91ce508adfecf23
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981827"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="d1a0d-103">Tipo de recurso emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="d1a0d-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="d1a0d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1a0d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d1a0d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1a0d-105">Properties</span></span>

| <span data-ttu-id="d1a0d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1a0d-106">Property</span></span>          | <span data-ttu-id="d1a0d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1a0d-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d1a0d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d1a0d-108">reportRefreshDate</span></span> | <span data-ttu-id="d1a0d-109">Data</span><span class="sxs-lookup"><span data-stu-id="d1a0d-109">Date</span></span>   |
| <span data-ttu-id="d1a0d-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="d1a0d-110">mailForMac</span></span>        | <span data-ttu-id="d1a0d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-111">Int64</span></span>  |
| <span data-ttu-id="d1a0d-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="d1a0d-112">outlookForMac</span></span>     | <span data-ttu-id="d1a0d-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-113">Int64</span></span>  |
| <span data-ttu-id="d1a0d-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="d1a0d-114">outlookForWindows</span></span> | <span data-ttu-id="d1a0d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-115">Int64</span></span>  |
| <span data-ttu-id="d1a0d-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="d1a0d-116">outlookForMobile</span></span>  | <span data-ttu-id="d1a0d-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-117">Int64</span></span>  |
| <span data-ttu-id="d1a0d-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="d1a0d-118">otherForMobile</span></span>    | <span data-ttu-id="d1a0d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-119">Int64</span></span>  |
| <span data-ttu-id="d1a0d-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="d1a0d-120">outlookForWeb</span></span>     | <span data-ttu-id="d1a0d-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-121">Int64</span></span>  |
| <span data-ttu-id="d1a0d-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="d1a0d-122">pop3App</span></span>           | <span data-ttu-id="d1a0d-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-123">Int64</span></span>  |
| <span data-ttu-id="d1a0d-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="d1a0d-124">imap4App</span></span>          | <span data-ttu-id="d1a0d-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-125">Int64</span></span>  |
| <span data-ttu-id="d1a0d-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="d1a0d-126">smtpApp</span></span>           | <span data-ttu-id="d1a0d-127">Int64</span><span class="sxs-lookup"><span data-stu-id="d1a0d-127">Int64</span></span>  |
| <span data-ttu-id="d1a0d-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d1a0d-128">reportPeriod</span></span>      | <span data-ttu-id="d1a0d-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1a0d-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d1a0d-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1a0d-130">JSON representation</span></span>

<span data-ttu-id="d1a0d-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1a0d-131">The following is a JSON representation of the resource.</span></span>

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


