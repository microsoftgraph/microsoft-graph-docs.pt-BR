---
title: tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c1e441b142ef27abbdde4ac613ef8d75848f5001
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966549"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="17993-103">tipo de recurso office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="17993-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="17993-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17993-104">Properties</span></span>

| <span data-ttu-id="17993-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17993-105">Property</span></span>               | <span data-ttu-id="17993-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="17993-106">Type</span></span>   | <span data-ttu-id="17993-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="17993-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="17993-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="17993-108">reportRefreshDate</span></span>      | <span data-ttu-id="17993-109">Data</span><span class="sxs-lookup"><span data-stu-id="17993-109">Date</span></span>   | <span data-ttu-id="17993-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="17993-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="17993-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="17993-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="17993-112">Int64</span><span class="sxs-lookup"><span data-stu-id="17993-112">Int64</span></span>  | <span data-ttu-id="17993-113">O número de emails recebidos por caixas de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="17993-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="17993-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="17993-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="17993-115">Int64</span><span class="sxs-lookup"><span data-stu-id="17993-115">Int64</span></span>  | <span data-ttu-id="17993-116">O número de mensagens postadas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="17993-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="17993-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="17993-117">yammerMessagesRead</span></span>     | <span data-ttu-id="17993-118">Int64</span><span class="sxs-lookup"><span data-stu-id="17993-118">Int64</span></span>  | <span data-ttu-id="17993-119">O número de mensagens lidas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="17993-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="17993-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="17993-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="17993-121">Int64</span><span class="sxs-lookup"><span data-stu-id="17993-121">Int64</span></span>  | <span data-ttu-id="17993-122">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="17993-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="17993-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="17993-123">reportDate</span></span>             | <span data-ttu-id="17993-124">Data</span><span class="sxs-lookup"><span data-stu-id="17993-124">Date</span></span>   | <span data-ttu-id="17993-125">A data em que um número de emails foi enviado para uma caixa de correio de grupo ou várias mensagens foram postadas, lidas ou curtidas em um grupo do Yammer</span><span class="sxs-lookup"><span data-stu-id="17993-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="17993-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="17993-126">reportPeriod</span></span>           | <span data-ttu-id="17993-127">String</span><span class="sxs-lookup"><span data-stu-id="17993-127">String</span></span> | <span data-ttu-id="17993-128">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="17993-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="17993-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17993-129">JSON representation</span></span>

<span data-ttu-id="17993-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17993-130">The following is a JSON representation of the resource.</span></span>

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
