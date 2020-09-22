---
title: tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6c67de6592d32c15e7d64112ce9ac31b6a5d4c41
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092423"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="de910-103">tipo de recurso office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="de910-103">office365GroupsActivityCounts resource type</span></span>

<span data-ttu-id="de910-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de910-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="de910-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de910-105">Properties</span></span>

| <span data-ttu-id="de910-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de910-106">Property</span></span>               | <span data-ttu-id="de910-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="de910-107">Type</span></span>   | <span data-ttu-id="de910-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="de910-108">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="de910-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="de910-109">reportRefreshDate</span></span>      | <span data-ttu-id="de910-110">Data</span><span class="sxs-lookup"><span data-stu-id="de910-110">Date</span></span>   | <span data-ttu-id="de910-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="de910-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="de910-112">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="de910-112">exchangeEmailsReceived</span></span> | <span data-ttu-id="de910-113">Int64</span><span class="sxs-lookup"><span data-stu-id="de910-113">Int64</span></span>  | <span data-ttu-id="de910-114">O número de emails recebidos por caixas de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="de910-114">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="de910-115">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="de910-115">yammerMessagesPosted</span></span>   | <span data-ttu-id="de910-116">Int64</span><span class="sxs-lookup"><span data-stu-id="de910-116">Int64</span></span>  | <span data-ttu-id="de910-117">O número de mensagens postadas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="de910-117">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="de910-118">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="de910-118">yammerMessagesRead</span></span>     | <span data-ttu-id="de910-119">Int64</span><span class="sxs-lookup"><span data-stu-id="de910-119">Int64</span></span>  | <span data-ttu-id="de910-120">O número de mensagens lidas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="de910-120">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="de910-121">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="de910-121">yammerMessagesLiked</span></span>    | <span data-ttu-id="de910-122">Int64</span><span class="sxs-lookup"><span data-stu-id="de910-122">Int64</span></span>  | <span data-ttu-id="de910-123">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="de910-123">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="de910-124">reportDate</span><span class="sxs-lookup"><span data-stu-id="de910-124">reportDate</span></span>             | <span data-ttu-id="de910-125">Data</span><span class="sxs-lookup"><span data-stu-id="de910-125">Date</span></span>   | <span data-ttu-id="de910-126">A data em que um número de emails foi enviado para uma caixa de correio de grupo ou várias mensagens foram postadas, lidas ou curtidas em um grupo do Yammer</span><span class="sxs-lookup"><span data-stu-id="de910-126">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="de910-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="de910-127">reportPeriod</span></span>           | <span data-ttu-id="de910-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de910-128">String</span></span> | <span data-ttu-id="de910-129">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="de910-129">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="de910-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de910-130">JSON representation</span></span>

<span data-ttu-id="de910-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de910-131">The following is a JSON representation of the resource.</span></span>

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


