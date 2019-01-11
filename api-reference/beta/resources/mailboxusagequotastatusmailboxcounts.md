---
title: tipo de recurso de mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: b87bb1ce91626f9151d294e2243bba72ba72346b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835215"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="6c841-103">tipo de recurso de mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="6c841-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6c841-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c841-104">Properties</span></span>

| <span data-ttu-id="6c841-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c841-105">Property</span></span>              | <span data-ttu-id="6c841-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c841-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="6c841-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6c841-107">reportRefreshDate</span></span>     | <span data-ttu-id="6c841-108">Data</span><span class="sxs-lookup"><span data-stu-id="6c841-108">Date</span></span>   |
| <span data-ttu-id="6c841-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="6c841-109">underLimit</span></span>            | <span data-ttu-id="6c841-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6c841-110">Int64</span></span>  |
| <span data-ttu-id="6c841-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="6c841-111">warningIssued</span></span>         | <span data-ttu-id="6c841-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6c841-112">Int64</span></span>  |
| <span data-ttu-id="6c841-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="6c841-113">sendProhibited</span></span>        | <span data-ttu-id="6c841-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6c841-114">Int64</span></span>  |
| <span data-ttu-id="6c841-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="6c841-115">sendReceiveProhibited</span></span> | <span data-ttu-id="6c841-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6c841-116">Int64</span></span>  |
| <span data-ttu-id="6c841-117">indeterminado</span><span class="sxs-lookup"><span data-stu-id="6c841-117">indeterminate</span></span>         | <span data-ttu-id="6c841-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6c841-118">Int64</span></span>  |
| <span data-ttu-id="6c841-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="6c841-119">reportDate</span></span>            | <span data-ttu-id="6c841-120">Data</span><span class="sxs-lookup"><span data-stu-id="6c841-120">Date</span></span>   |
| <span data-ttu-id="6c841-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6c841-121">reportPeriod</span></span>          | <span data-ttu-id="6c841-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c841-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6c841-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c841-123">JSON representation</span></span>

<span data-ttu-id="6c841-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c841-124">The following is a JSON representation of the resource.</span></span>

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
