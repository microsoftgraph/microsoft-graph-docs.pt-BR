---
title: tipo de recurso de office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 4f3a5bf02f5f477ebab036fc9afa5d35a8061138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039928"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="b199b-103">tipo de recurso de office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="b199b-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b199b-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b199b-104">Properties</span></span>

| <span data-ttu-id="b199b-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b199b-105">Property</span></span>               | <span data-ttu-id="b199b-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b199b-106">Type</span></span>   | <span data-ttu-id="b199b-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b199b-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="b199b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b199b-108">reportRefreshDate</span></span>      | <span data-ttu-id="b199b-109">Data</span><span class="sxs-lookup"><span data-stu-id="b199b-109">Date</span></span>   | <span data-ttu-id="b199b-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b199b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="b199b-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="b199b-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="b199b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b199b-112">Int64</span></span>  | <span data-ttu-id="b199b-113">O número de emails recebidos por caixas de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="b199b-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="b199b-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="b199b-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="b199b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b199b-115">Int64</span></span>  | <span data-ttu-id="b199b-116">O número de mensagens postadas em grupos de Yammer.</span><span class="sxs-lookup"><span data-stu-id="b199b-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="b199b-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="b199b-117">yammerMessagesRead</span></span>     | <span data-ttu-id="b199b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b199b-118">Int64</span></span>  | <span data-ttu-id="b199b-119">O número de mensagens lidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="b199b-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="b199b-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="b199b-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="b199b-121">Int64</span><span class="sxs-lookup"><span data-stu-id="b199b-121">Int64</span></span>  | <span data-ttu-id="b199b-122">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="b199b-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="b199b-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="b199b-123">reportDate</span></span>             | <span data-ttu-id="b199b-124">Data</span><span class="sxs-lookup"><span data-stu-id="b199b-124">Date</span></span>   | <span data-ttu-id="b199b-125">A data em que um número de emails que foram enviado para uma caixa de correio de grupo ou um número de mensagens publicado, ler ou curtidas em um grupo do Yammer</span><span class="sxs-lookup"><span data-stu-id="b199b-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="b199b-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b199b-126">reportPeriod</span></span>           | <span data-ttu-id="b199b-127">String</span><span class="sxs-lookup"><span data-stu-id="b199b-127">String</span></span> | <span data-ttu-id="b199b-128">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="b199b-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="b199b-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b199b-129">JSON representation</span></span>

<span data-ttu-id="b199b-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b199b-130">The following is a JSON representation of the resource.</span></span>

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
