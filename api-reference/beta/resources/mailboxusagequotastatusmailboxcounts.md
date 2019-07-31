---
title: tipo de recurso mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1e8fafe9a3cdce4519cf5755337b016fa587cd06
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966899"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="06cf3-103">tipo de recurso mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="06cf3-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="06cf3-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06cf3-104">Properties</span></span>

| <span data-ttu-id="06cf3-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06cf3-105">Property</span></span>              | <span data-ttu-id="06cf3-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="06cf3-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="06cf3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="06cf3-107">reportRefreshDate</span></span>     | <span data-ttu-id="06cf3-108">Data</span><span class="sxs-lookup"><span data-stu-id="06cf3-108">Date</span></span>   |
| <span data-ttu-id="06cf3-109">Limite máximo</span><span class="sxs-lookup"><span data-stu-id="06cf3-109">underLimit</span></span>            | <span data-ttu-id="06cf3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="06cf3-110">Int64</span></span>  |
| <span data-ttu-id="06cf3-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="06cf3-111">warningIssued</span></span>         | <span data-ttu-id="06cf3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="06cf3-112">Int64</span></span>  |
| <span data-ttu-id="06cf3-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="06cf3-113">sendProhibited</span></span>        | <span data-ttu-id="06cf3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="06cf3-114">Int64</span></span>  |
| <span data-ttu-id="06cf3-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="06cf3-115">sendReceiveProhibited</span></span> | <span data-ttu-id="06cf3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="06cf3-116">Int64</span></span>  |
| <span data-ttu-id="06cf3-117">determinado</span><span class="sxs-lookup"><span data-stu-id="06cf3-117">indeterminate</span></span>         | <span data-ttu-id="06cf3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="06cf3-118">Int64</span></span>  |
| <span data-ttu-id="06cf3-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="06cf3-119">reportDate</span></span>            | <span data-ttu-id="06cf3-120">Data</span><span class="sxs-lookup"><span data-stu-id="06cf3-120">Date</span></span>   |
| <span data-ttu-id="06cf3-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="06cf3-121">reportPeriod</span></span>          | <span data-ttu-id="06cf3-122">String</span><span class="sxs-lookup"><span data-stu-id="06cf3-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="06cf3-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06cf3-123">JSON representation</span></span>

<span data-ttu-id="06cf3-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06cf3-124">The following is a JSON representation of the resource.</span></span>

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
