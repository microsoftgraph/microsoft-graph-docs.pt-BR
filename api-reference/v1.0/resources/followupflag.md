---
title: Tipo de recurso followupFlag
description: 'Permite definir um sinalizador em um item para que o usuário acompanhe mais tarde. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 28734c08d4626805de467ebad8c640acf3bdf7f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531389"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="50be3-103">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="50be3-103">followupFlag resource type</span></span>

<span data-ttu-id="50be3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50be3-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="50be3-105">Permite definir um sinalizador em um item para que o usuário acompanhe mais tarde.</span><span class="sxs-lookup"><span data-stu-id="50be3-105">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="50be3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50be3-106">Properties</span></span>
| <span data-ttu-id="50be3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50be3-107">Property</span></span>     | <span data-ttu-id="50be3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="50be3-108">Type</span></span>   |<span data-ttu-id="50be3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="50be3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50be3-110">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="50be3-110">completedDateTime</span></span>|[<span data-ttu-id="50be3-111">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="50be3-111">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="50be3-112">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="50be3-112">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="50be3-113">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="50be3-113">dueDateTime</span></span>|<span data-ttu-id="50be3-114">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="50be3-114">**dateTimeTimeZone**</span></span>|<span data-ttu-id="50be3-115">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="50be3-115">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="50be3-116">flagStatus</span><span class="sxs-lookup"><span data-stu-id="50be3-116">flagStatus</span></span>|<span data-ttu-id="50be3-117">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="50be3-117">followupFlagStatus</span></span>|<span data-ttu-id="50be3-118">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="50be3-118">The status for follow-up for an item.</span></span> <span data-ttu-id="50be3-119">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="50be3-119">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="50be3-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="50be3-120">startDateTime</span></span>|<span data-ttu-id="50be3-121">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="50be3-121">**dateTimeTimeZone**</span></span>|<span data-ttu-id="50be3-122">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="50be3-122">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50be3-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50be3-123">JSON representation</span></span>

<span data-ttu-id="50be3-124">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="50be3-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
