---
title: tipo de recurso de office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 87867071545a36f7aca1833a369f919317153bc6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874106"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="68708-103">tipo de recurso de office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="68708-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="68708-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68708-104">Properties</span></span>

| <span data-ttu-id="68708-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68708-105">Property</span></span>               | <span data-ttu-id="68708-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="68708-106">Type</span></span>   | <span data-ttu-id="68708-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="68708-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="68708-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="68708-108">reportRefreshDate</span></span>      | <span data-ttu-id="68708-109">Data</span><span class="sxs-lookup"><span data-stu-id="68708-109">Date</span></span>   | <span data-ttu-id="68708-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="68708-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="68708-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="68708-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="68708-112">Int64</span><span class="sxs-lookup"><span data-stu-id="68708-112">Int64</span></span>  | <span data-ttu-id="68708-113">O número de emails recebidos por caixas de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="68708-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="68708-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="68708-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="68708-115">Int64</span><span class="sxs-lookup"><span data-stu-id="68708-115">Int64</span></span>  | <span data-ttu-id="68708-116">O número de mensagens postadas em grupos de Yammer.</span><span class="sxs-lookup"><span data-stu-id="68708-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="68708-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="68708-117">yammerMessagesRead</span></span>     | <span data-ttu-id="68708-118">Int64</span><span class="sxs-lookup"><span data-stu-id="68708-118">Int64</span></span>  | <span data-ttu-id="68708-119">O número de mensagens lidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="68708-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="68708-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="68708-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="68708-121">Int64</span><span class="sxs-lookup"><span data-stu-id="68708-121">Int64</span></span>  | <span data-ttu-id="68708-122">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="68708-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="68708-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="68708-123">reportDate</span></span>             | <span data-ttu-id="68708-124">Data</span><span class="sxs-lookup"><span data-stu-id="68708-124">Date</span></span>   | <span data-ttu-id="68708-125">A data em que um número de emails que foram enviado para uma caixa de correio de grupo ou um número de mensagens publicado, ler ou curtidas em um grupo do Yammer</span><span class="sxs-lookup"><span data-stu-id="68708-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="68708-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="68708-126">reportPeriod</span></span>           | <span data-ttu-id="68708-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68708-127">String</span></span> | <span data-ttu-id="68708-128">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="68708-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="68708-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68708-129">JSON representation</span></span>

<span data-ttu-id="68708-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68708-130">The following is a JSON representation of the resource.</span></span>

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
