---
title: tipo de recurso mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457127"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="1b698-103">tipo de recurso mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="1b698-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1b698-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b698-104">Properties</span></span>

| <span data-ttu-id="1b698-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b698-105">Property</span></span>              | <span data-ttu-id="1b698-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b698-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="1b698-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1b698-107">reportRefreshDate</span></span>     | <span data-ttu-id="1b698-108">Data</span><span class="sxs-lookup"><span data-stu-id="1b698-108">Date</span></span>   |
| <span data-ttu-id="1b698-109">Limite máximo</span><span class="sxs-lookup"><span data-stu-id="1b698-109">underLimit</span></span>            | <span data-ttu-id="1b698-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1b698-110">Int64</span></span>  |
| <span data-ttu-id="1b698-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="1b698-111">warningIssued</span></span>         | <span data-ttu-id="1b698-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1b698-112">Int64</span></span>  |
| <span data-ttu-id="1b698-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="1b698-113">sendProhibited</span></span>        | <span data-ttu-id="1b698-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1b698-114">Int64</span></span>  |
| <span data-ttu-id="1b698-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="1b698-115">sendReceiveProhibited</span></span> | <span data-ttu-id="1b698-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1b698-116">Int64</span></span>  |
| <span data-ttu-id="1b698-117">determinado</span><span class="sxs-lookup"><span data-stu-id="1b698-117">indeterminate</span></span>         | <span data-ttu-id="1b698-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1b698-118">Int64</span></span>  |
| <span data-ttu-id="1b698-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="1b698-119">reportDate</span></span>            | <span data-ttu-id="1b698-120">Data</span><span class="sxs-lookup"><span data-stu-id="1b698-120">Date</span></span>   |
| <span data-ttu-id="1b698-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1b698-121">reportPeriod</span></span>          | <span data-ttu-id="1b698-122">String</span><span class="sxs-lookup"><span data-stu-id="1b698-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1b698-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b698-123">JSON representation</span></span>

<span data-ttu-id="1b698-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b698-124">The following is a JSON representation of the resource.</span></span>

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
