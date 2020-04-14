---
title: tipo de recurso mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1ebbfe0f134848d78e9c42a159c1c56bdbd21b39
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473422"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="c3ed9-103">tipo de recurso mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="c3ed9-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="c3ed9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3ed9-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c3ed9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3ed9-105">Properties</span></span>

| <span data-ttu-id="c3ed9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3ed9-106">Property</span></span>              | <span data-ttu-id="c3ed9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3ed9-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="c3ed9-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c3ed9-108">reportRefreshDate</span></span>     | <span data-ttu-id="c3ed9-109">Data</span><span class="sxs-lookup"><span data-stu-id="c3ed9-109">Date</span></span>   |
| <span data-ttu-id="c3ed9-110">Limite máximo</span><span class="sxs-lookup"><span data-stu-id="c3ed9-110">underLimit</span></span>            | <span data-ttu-id="c3ed9-111">Int64</span><span class="sxs-lookup"><span data-stu-id="c3ed9-111">Int64</span></span>  |
| <span data-ttu-id="c3ed9-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="c3ed9-112">warningIssued</span></span>         | <span data-ttu-id="c3ed9-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c3ed9-113">Int64</span></span>  |
| <span data-ttu-id="c3ed9-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="c3ed9-114">sendProhibited</span></span>        | <span data-ttu-id="c3ed9-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c3ed9-115">Int64</span></span>  |
| <span data-ttu-id="c3ed9-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="c3ed9-116">sendReceiveProhibited</span></span> | <span data-ttu-id="c3ed9-117">Int64</span><span class="sxs-lookup"><span data-stu-id="c3ed9-117">Int64</span></span>  |
| <span data-ttu-id="c3ed9-118">determinado</span><span class="sxs-lookup"><span data-stu-id="c3ed9-118">indeterminate</span></span>         | <span data-ttu-id="c3ed9-119">Int64</span><span class="sxs-lookup"><span data-stu-id="c3ed9-119">Int64</span></span>  |
| <span data-ttu-id="c3ed9-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="c3ed9-120">reportDate</span></span>            | <span data-ttu-id="c3ed9-121">Data</span><span class="sxs-lookup"><span data-stu-id="c3ed9-121">Date</span></span>   |
| <span data-ttu-id="c3ed9-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c3ed9-122">reportPeriod</span></span>          | <span data-ttu-id="c3ed9-123">String</span><span class="sxs-lookup"><span data-stu-id="c3ed9-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3ed9-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3ed9-124">JSON representation</span></span>

<span data-ttu-id="c3ed9-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3ed9-125">The following is a JSON representation of the resource.</span></span>

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
