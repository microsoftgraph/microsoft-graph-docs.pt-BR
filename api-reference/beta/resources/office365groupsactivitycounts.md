---
title: Tipo de recurso office365GroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: a212028e4ba9d38ea38e99c835d89fe1fe7d850b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980693"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="8f658-103">Tipo de recurso office365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="8f658-103">office365GroupsActivityCounts resource type</span></span>

<span data-ttu-id="8f658-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f658-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="8f658-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f658-105">Properties</span></span>

| <span data-ttu-id="8f658-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f658-106">Property</span></span>               | <span data-ttu-id="8f658-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f658-107">Type</span></span>   | <span data-ttu-id="8f658-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f658-108">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="8f658-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8f658-109">reportRefreshDate</span></span>      | <span data-ttu-id="8f658-110">Data</span><span class="sxs-lookup"><span data-stu-id="8f658-110">Date</span></span>   | <span data-ttu-id="8f658-111">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8f658-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="8f658-112">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="8f658-112">exchangeEmailsReceived</span></span> | <span data-ttu-id="8f658-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8f658-113">Int64</span></span>  | <span data-ttu-id="8f658-114">O número de emails recebidos pelas caixas de correio de Grupo.</span><span class="sxs-lookup"><span data-stu-id="8f658-114">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="8f658-115">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="8f658-115">yammerMessagesPosted</span></span>   | <span data-ttu-id="8f658-116">Int64</span><span class="sxs-lookup"><span data-stu-id="8f658-116">Int64</span></span>  | <span data-ttu-id="8f658-117">O número de mensagens postadas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="8f658-117">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="8f658-118">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="8f658-118">yammerMessagesRead</span></span>     | <span data-ttu-id="8f658-119">Int64</span><span class="sxs-lookup"><span data-stu-id="8f658-119">Int64</span></span>  | <span data-ttu-id="8f658-120">O número de mensagens lidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="8f658-120">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="8f658-121">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="8f658-121">yammerMessagesLiked</span></span>    | <span data-ttu-id="8f658-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8f658-122">Int64</span></span>  | <span data-ttu-id="8f658-123">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="8f658-123">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="8f658-124">reportDate</span><span class="sxs-lookup"><span data-stu-id="8f658-124">reportDate</span></span>             | <span data-ttu-id="8f658-125">Data</span><span class="sxs-lookup"><span data-stu-id="8f658-125">Date</span></span>   | <span data-ttu-id="8f658-126">A data em que vários emails foram enviados para uma caixa de correio de grupo ou várias mensagens postadas, lidas ou curtidas em um grupo do Yammer</span><span class="sxs-lookup"><span data-stu-id="8f658-126">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="8f658-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8f658-127">reportPeriod</span></span>           | <span data-ttu-id="8f658-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f658-128">String</span></span> | <span data-ttu-id="8f658-129">O número de dias que o relatório abrange.</span><span class="sxs-lookup"><span data-stu-id="8f658-129">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="8f658-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f658-130">JSON representation</span></span>

<span data-ttu-id="8f658-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f658-131">The following is a JSON representation of the resource.</span></span>

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


