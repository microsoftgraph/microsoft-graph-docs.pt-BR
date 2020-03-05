---
title: tipo de recurso mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ce215e0eae3a13aa0c2d27f54338efc57c0c5486
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522838"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="93f4a-103">tipo de recurso mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="93f4a-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="93f4a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="93f4a-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="93f4a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93f4a-105">Properties</span></span>

| <span data-ttu-id="93f4a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93f4a-106">Property</span></span>              | <span data-ttu-id="93f4a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="93f4a-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="93f4a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="93f4a-108">reportRefreshDate</span></span>     | <span data-ttu-id="93f4a-109">Data</span><span class="sxs-lookup"><span data-stu-id="93f4a-109">Date</span></span>   |
| <span data-ttu-id="93f4a-110">Limite máximo</span><span class="sxs-lookup"><span data-stu-id="93f4a-110">underLimit</span></span>            | <span data-ttu-id="93f4a-111">Int64</span><span class="sxs-lookup"><span data-stu-id="93f4a-111">Int64</span></span>  |
| <span data-ttu-id="93f4a-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="93f4a-112">warningIssued</span></span>         | <span data-ttu-id="93f4a-113">Int64</span><span class="sxs-lookup"><span data-stu-id="93f4a-113">Int64</span></span>  |
| <span data-ttu-id="93f4a-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="93f4a-114">sendProhibited</span></span>        | <span data-ttu-id="93f4a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="93f4a-115">Int64</span></span>  |
| <span data-ttu-id="93f4a-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="93f4a-116">sendReceiveProhibited</span></span> | <span data-ttu-id="93f4a-117">Int64</span><span class="sxs-lookup"><span data-stu-id="93f4a-117">Int64</span></span>  |
| <span data-ttu-id="93f4a-118">determinado</span><span class="sxs-lookup"><span data-stu-id="93f4a-118">indeterminate</span></span>         | <span data-ttu-id="93f4a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="93f4a-119">Int64</span></span>  |
| <span data-ttu-id="93f4a-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="93f4a-120">reportDate</span></span>            | <span data-ttu-id="93f4a-121">Data</span><span class="sxs-lookup"><span data-stu-id="93f4a-121">Date</span></span>   |
| <span data-ttu-id="93f4a-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="93f4a-122">reportPeriod</span></span>          | <span data-ttu-id="93f4a-123">String</span><span class="sxs-lookup"><span data-stu-id="93f4a-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93f4a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93f4a-124">JSON representation</span></span>

<span data-ttu-id="93f4a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93f4a-125">The following is a JSON representation of the resource.</span></span>

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
