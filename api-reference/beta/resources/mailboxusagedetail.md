---
title: tipo de recurso de mailboxUsageDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: af49fac7c6286c7e9f9ce1e6d7ffdede225b4072
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034793"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="3b008-103">tipo de recurso de mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="3b008-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3b008-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b008-104">Properties</span></span>

| <span data-ttu-id="3b008-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b008-105">Property</span></span>                        | <span data-ttu-id="3b008-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b008-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="3b008-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3b008-107">reportRefreshDate</span></span>               | <span data-ttu-id="3b008-108">Data</span><span class="sxs-lookup"><span data-stu-id="3b008-108">Date</span></span>    |
| <span data-ttu-id="3b008-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3b008-109">userPrincipalName</span></span>               | <span data-ttu-id="3b008-110">String</span><span class="sxs-lookup"><span data-stu-id="3b008-110">String</span></span>  |
| <span data-ttu-id="3b008-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3b008-111">displayName</span></span>                     | <span data-ttu-id="3b008-112">String</span><span class="sxs-lookup"><span data-stu-id="3b008-112">String</span></span>  |
| <span data-ttu-id="3b008-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="3b008-113">isDeleted</span></span>                       | <span data-ttu-id="3b008-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b008-114">Boolean</span></span> |
| <span data-ttu-id="3b008-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="3b008-115">deletedDate</span></span>                     | <span data-ttu-id="3b008-116">Data</span><span class="sxs-lookup"><span data-stu-id="3b008-116">Date</span></span>    |
| <span data-ttu-id="3b008-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="3b008-117">createdDate</span></span>                     | <span data-ttu-id="3b008-118">Data</span><span class="sxs-lookup"><span data-stu-id="3b008-118">Date</span></span>    |
| <span data-ttu-id="3b008-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3b008-119">lastActivityDate</span></span>                | <span data-ttu-id="3b008-120">Data</span><span class="sxs-lookup"><span data-stu-id="3b008-120">Date</span></span>    |
| <span data-ttu-id="3b008-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="3b008-121">itemCount</span></span>                       | <span data-ttu-id="3b008-122">Int64</span><span class="sxs-lookup"><span data-stu-id="3b008-122">Int64</span></span>   |
| <span data-ttu-id="3b008-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="3b008-123">storageUsedInBytes</span></span>              | <span data-ttu-id="3b008-124">Int64</span><span class="sxs-lookup"><span data-stu-id="3b008-124">Int64</span></span>   |
| <span data-ttu-id="3b008-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="3b008-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="3b008-126">Int64</span><span class="sxs-lookup"><span data-stu-id="3b008-126">Int64</span></span>   |
| <span data-ttu-id="3b008-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="3b008-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="3b008-128">Int64</span><span class="sxs-lookup"><span data-stu-id="3b008-128">Int64</span></span>   |
| <span data-ttu-id="3b008-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="3b008-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="3b008-130">Int64</span><span class="sxs-lookup"><span data-stu-id="3b008-130">Int64</span></span>   |
| <span data-ttu-id="3b008-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3b008-131">reportPeriod</span></span>                    | <span data-ttu-id="3b008-132">String</span><span class="sxs-lookup"><span data-stu-id="3b008-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="3b008-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b008-133">JSON representation</span></span>

<span data-ttu-id="3b008-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b008-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
