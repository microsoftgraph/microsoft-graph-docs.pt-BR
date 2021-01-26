---
title: Tipo de recurso mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 10ce05121ec900f5475a082191f4192974f980b4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983542"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="f5cec-103">Tipo de recurso mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="f5cec-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="f5cec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5cec-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f5cec-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5cec-105">Properties</span></span>

| <span data-ttu-id="f5cec-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5cec-106">Property</span></span>              | <span data-ttu-id="f5cec-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5cec-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="f5cec-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f5cec-108">reportRefreshDate</span></span>     | <span data-ttu-id="f5cec-109">Data</span><span class="sxs-lookup"><span data-stu-id="f5cec-109">Date</span></span>   |
| <span data-ttu-id="f5cec-110">underLimit</span><span class="sxs-lookup"><span data-stu-id="f5cec-110">underLimit</span></span>            | <span data-ttu-id="f5cec-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f5cec-111">Int64</span></span>  |
| <span data-ttu-id="f5cec-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="f5cec-112">warningIssued</span></span>         | <span data-ttu-id="f5cec-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f5cec-113">Int64</span></span>  |
| <span data-ttu-id="f5cec-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="f5cec-114">sendProhibited</span></span>        | <span data-ttu-id="f5cec-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f5cec-115">Int64</span></span>  |
| <span data-ttu-id="f5cec-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="f5cec-116">sendReceiveProhibited</span></span> | <span data-ttu-id="f5cec-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f5cec-117">Int64</span></span>  |
| <span data-ttu-id="f5cec-118">indeterminado</span><span class="sxs-lookup"><span data-stu-id="f5cec-118">indeterminate</span></span>         | <span data-ttu-id="f5cec-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f5cec-119">Int64</span></span>  |
| <span data-ttu-id="f5cec-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="f5cec-120">reportDate</span></span>            | <span data-ttu-id="f5cec-121">Data</span><span class="sxs-lookup"><span data-stu-id="f5cec-121">Date</span></span>   |
| <span data-ttu-id="f5cec-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f5cec-122">reportPeriod</span></span>          | <span data-ttu-id="f5cec-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5cec-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f5cec-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5cec-124">JSON representation</span></span>

<span data-ttu-id="f5cec-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5cec-125">The following is a JSON representation of the resource.</span></span>

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


