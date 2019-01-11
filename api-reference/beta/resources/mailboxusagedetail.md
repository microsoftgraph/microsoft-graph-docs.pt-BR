---
title: tipo de recurso de mailboxUsageDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 25cb41e38138a677bfc6636b035003bb8fc5858c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818008"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="b388e-103">tipo de recurso de mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="b388e-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b388e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b388e-104">Properties</span></span>

| <span data-ttu-id="b388e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b388e-105">Property</span></span>                        | <span data-ttu-id="b388e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b388e-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="b388e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b388e-107">reportRefreshDate</span></span>               | <span data-ttu-id="b388e-108">Data</span><span class="sxs-lookup"><span data-stu-id="b388e-108">Date</span></span>    |
| <span data-ttu-id="b388e-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b388e-109">userPrincipalName</span></span>               | <span data-ttu-id="b388e-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b388e-110">String</span></span>  |
| <span data-ttu-id="b388e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b388e-111">displayName</span></span>                     | <span data-ttu-id="b388e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b388e-112">String</span></span>  |
| <span data-ttu-id="b388e-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b388e-113">isDeleted</span></span>                       | <span data-ttu-id="b388e-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="b388e-114">Boolean</span></span> |
| <span data-ttu-id="b388e-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="b388e-115">deletedDate</span></span>                     | <span data-ttu-id="b388e-116">Data</span><span class="sxs-lookup"><span data-stu-id="b388e-116">Date</span></span>    |
| <span data-ttu-id="b388e-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="b388e-117">createdDate</span></span>                     | <span data-ttu-id="b388e-118">Data</span><span class="sxs-lookup"><span data-stu-id="b388e-118">Date</span></span>    |
| <span data-ttu-id="b388e-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="b388e-119">lastActivityDate</span></span>                | <span data-ttu-id="b388e-120">Data</span><span class="sxs-lookup"><span data-stu-id="b388e-120">Date</span></span>    |
| <span data-ttu-id="b388e-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="b388e-121">itemCount</span></span>                       | <span data-ttu-id="b388e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b388e-122">Int64</span></span>   |
| <span data-ttu-id="b388e-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="b388e-123">storageUsedInBytes</span></span>              | <span data-ttu-id="b388e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b388e-124">Int64</span></span>   |
| <span data-ttu-id="b388e-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="b388e-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="b388e-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b388e-126">Int64</span></span>   |
| <span data-ttu-id="b388e-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="b388e-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="b388e-128">Int64</span><span class="sxs-lookup"><span data-stu-id="b388e-128">Int64</span></span>   |
| <span data-ttu-id="b388e-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="b388e-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="b388e-130">Int64</span><span class="sxs-lookup"><span data-stu-id="b388e-130">Int64</span></span>   |
| <span data-ttu-id="b388e-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b388e-131">reportPeriod</span></span>                    | <span data-ttu-id="b388e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b388e-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="b388e-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b388e-133">JSON representation</span></span>

<span data-ttu-id="b388e-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b388e-134">The following is a JSON representation of the resource.</span></span>

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
