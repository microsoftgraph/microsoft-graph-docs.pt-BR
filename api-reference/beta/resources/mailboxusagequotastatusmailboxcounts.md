---
title: tipo de recurso de mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: ac6c597cad9d28f985da97d6f55a5726ebbf491e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036038"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="08e91-103">tipo de recurso de mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="08e91-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="08e91-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08e91-104">Properties</span></span>

| <span data-ttu-id="08e91-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08e91-105">Property</span></span>              | <span data-ttu-id="08e91-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="08e91-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="08e91-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="08e91-107">reportRefreshDate</span></span>     | <span data-ttu-id="08e91-108">Data</span><span class="sxs-lookup"><span data-stu-id="08e91-108">Date</span></span>   |
| <span data-ttu-id="08e91-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="08e91-109">underLimit</span></span>            | <span data-ttu-id="08e91-110">Int64</span><span class="sxs-lookup"><span data-stu-id="08e91-110">Int64</span></span>  |
| <span data-ttu-id="08e91-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="08e91-111">warningIssued</span></span>         | <span data-ttu-id="08e91-112">Int64</span><span class="sxs-lookup"><span data-stu-id="08e91-112">Int64</span></span>  |
| <span data-ttu-id="08e91-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="08e91-113">sendProhibited</span></span>        | <span data-ttu-id="08e91-114">Int64</span><span class="sxs-lookup"><span data-stu-id="08e91-114">Int64</span></span>  |
| <span data-ttu-id="08e91-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="08e91-115">sendReceiveProhibited</span></span> | <span data-ttu-id="08e91-116">Int64</span><span class="sxs-lookup"><span data-stu-id="08e91-116">Int64</span></span>  |
| <span data-ttu-id="08e91-117">indeterminado</span><span class="sxs-lookup"><span data-stu-id="08e91-117">indeterminate</span></span>         | <span data-ttu-id="08e91-118">Int64</span><span class="sxs-lookup"><span data-stu-id="08e91-118">Int64</span></span>  |
| <span data-ttu-id="08e91-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="08e91-119">reportDate</span></span>            | <span data-ttu-id="08e91-120">Data</span><span class="sxs-lookup"><span data-stu-id="08e91-120">Date</span></span>   |
| <span data-ttu-id="08e91-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="08e91-121">reportPeriod</span></span>          | <span data-ttu-id="08e91-122">String</span><span class="sxs-lookup"><span data-stu-id="08e91-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08e91-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08e91-123">JSON representation</span></span>

<span data-ttu-id="08e91-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08e91-124">The following is a JSON representation of the resource.</span></span>

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
