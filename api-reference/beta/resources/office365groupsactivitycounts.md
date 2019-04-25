---
title: tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581720"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="e597e-103">tipo de recurso office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="e597e-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e597e-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e597e-104">Properties</span></span>

| <span data-ttu-id="e597e-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e597e-105">Property</span></span>               | <span data-ttu-id="e597e-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="e597e-106">Type</span></span>   | <span data-ttu-id="e597e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e597e-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="e597e-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e597e-108">reportRefreshDate</span></span>      | <span data-ttu-id="e597e-109">Data</span><span class="sxs-lookup"><span data-stu-id="e597e-109">Date</span></span>   | <span data-ttu-id="e597e-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e597e-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="e597e-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="e597e-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="e597e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e597e-112">Int64</span></span>  | <span data-ttu-id="e597e-113">O número de emails recebidos por caixas de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="e597e-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="e597e-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="e597e-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="e597e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="e597e-115">Int64</span></span>  | <span data-ttu-id="e597e-116">O número de mensagens postadas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="e597e-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="e597e-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="e597e-117">yammerMessagesRead</span></span>     | <span data-ttu-id="e597e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e597e-118">Int64</span></span>  | <span data-ttu-id="e597e-119">O número de mensagens lidas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="e597e-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="e597e-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="e597e-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="e597e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="e597e-121">Int64</span></span>  | <span data-ttu-id="e597e-122">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="e597e-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="e597e-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="e597e-123">reportDate</span></span>             | <span data-ttu-id="e597e-124">Data</span><span class="sxs-lookup"><span data-stu-id="e597e-124">Date</span></span>   | <span data-ttu-id="e597e-125">A data em que um número de emails foi enviado para uma caixa de correio de grupo ou várias mensagens foram postadas, lidas ou curtidas em um grupo do Yammer</span><span class="sxs-lookup"><span data-stu-id="e597e-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="e597e-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e597e-126">reportPeriod</span></span>           | <span data-ttu-id="e597e-127">String</span><span class="sxs-lookup"><span data-stu-id="e597e-127">String</span></span> | <span data-ttu-id="e597e-128">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="e597e-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="e597e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e597e-129">JSON representation</span></span>

<span data-ttu-id="e597e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e597e-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
