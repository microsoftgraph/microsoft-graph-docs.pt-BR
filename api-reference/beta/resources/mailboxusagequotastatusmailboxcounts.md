---
title: tipo de recurso de mailboxUsageQuotaStatusMailboxCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921231"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="66302-103">tipo de recurso de mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="66302-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="66302-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66302-104">Properties</span></span>

| <span data-ttu-id="66302-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66302-105">Property</span></span>              | <span data-ttu-id="66302-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="66302-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="66302-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="66302-107">reportRefreshDate</span></span>     | <span data-ttu-id="66302-108">Data</span><span class="sxs-lookup"><span data-stu-id="66302-108">Date</span></span>   |
| <span data-ttu-id="66302-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="66302-109">underLimit</span></span>            | <span data-ttu-id="66302-110">Int64</span><span class="sxs-lookup"><span data-stu-id="66302-110">Int64</span></span>  |
| <span data-ttu-id="66302-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="66302-111">warningIssued</span></span>         | <span data-ttu-id="66302-112">Int64</span><span class="sxs-lookup"><span data-stu-id="66302-112">Int64</span></span>  |
| <span data-ttu-id="66302-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="66302-113">sendProhibited</span></span>        | <span data-ttu-id="66302-114">Int64</span><span class="sxs-lookup"><span data-stu-id="66302-114">Int64</span></span>  |
| <span data-ttu-id="66302-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="66302-115">sendReceiveProhibited</span></span> | <span data-ttu-id="66302-116">Int64</span><span class="sxs-lookup"><span data-stu-id="66302-116">Int64</span></span>  |
| <span data-ttu-id="66302-117">indeterminado</span><span class="sxs-lookup"><span data-stu-id="66302-117">indeterminate</span></span>         | <span data-ttu-id="66302-118">Int64</span><span class="sxs-lookup"><span data-stu-id="66302-118">Int64</span></span>  |
| <span data-ttu-id="66302-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="66302-119">reportDate</span></span>            | <span data-ttu-id="66302-120">Data</span><span class="sxs-lookup"><span data-stu-id="66302-120">Date</span></span>   |
| <span data-ttu-id="66302-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="66302-121">reportPeriod</span></span>          | <span data-ttu-id="66302-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66302-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="66302-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66302-123">JSON representation</span></span>

<span data-ttu-id="66302-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66302-124">The following is a JSON representation of the resource.</span></span>

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
