---
title: tipo de recurso mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e09b9d27da4a85dd89f6a09440d56532045573b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029173"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="a0239-103">tipo de recurso mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="a0239-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="a0239-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0239-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a0239-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0239-105">Properties</span></span>

| <span data-ttu-id="a0239-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0239-106">Property</span></span>              | <span data-ttu-id="a0239-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0239-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="a0239-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a0239-108">reportRefreshDate</span></span>     | <span data-ttu-id="a0239-109">Data</span><span class="sxs-lookup"><span data-stu-id="a0239-109">Date</span></span>   |
| <span data-ttu-id="a0239-110">Limite máximo</span><span class="sxs-lookup"><span data-stu-id="a0239-110">underLimit</span></span>            | <span data-ttu-id="a0239-111">Int64</span><span class="sxs-lookup"><span data-stu-id="a0239-111">Int64</span></span>  |
| <span data-ttu-id="a0239-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="a0239-112">warningIssued</span></span>         | <span data-ttu-id="a0239-113">Int64</span><span class="sxs-lookup"><span data-stu-id="a0239-113">Int64</span></span>  |
| <span data-ttu-id="a0239-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="a0239-114">sendProhibited</span></span>        | <span data-ttu-id="a0239-115">Int64</span><span class="sxs-lookup"><span data-stu-id="a0239-115">Int64</span></span>  |
| <span data-ttu-id="a0239-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="a0239-116">sendReceiveProhibited</span></span> | <span data-ttu-id="a0239-117">Int64</span><span class="sxs-lookup"><span data-stu-id="a0239-117">Int64</span></span>  |
| <span data-ttu-id="a0239-118">determinado</span><span class="sxs-lookup"><span data-stu-id="a0239-118">indeterminate</span></span>         | <span data-ttu-id="a0239-119">Int64</span><span class="sxs-lookup"><span data-stu-id="a0239-119">Int64</span></span>  |
| <span data-ttu-id="a0239-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="a0239-120">reportDate</span></span>            | <span data-ttu-id="a0239-121">Data</span><span class="sxs-lookup"><span data-stu-id="a0239-121">Date</span></span>   |
| <span data-ttu-id="a0239-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a0239-122">reportPeriod</span></span>          | <span data-ttu-id="a0239-123">String</span><span class="sxs-lookup"><span data-stu-id="a0239-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0239-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0239-124">JSON representation</span></span>

<span data-ttu-id="a0239-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0239-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


