---
title: Tipo de recurso followupFlag
description: 'Permite definir um sinalizador em um item para que o usuário acompanhe mais tarde. '
localization_priority: Normal
ms.openlocfilehash: 60d2e40a10c3ba5b2af9aa798b84aadaebedd57a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541994"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="1ca67-103">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="1ca67-103">followupFlag resource type</span></span>


<span data-ttu-id="1ca67-104">Permite definir um sinalizador em um item para que o usuário acompanhe mais tarde.</span><span class="sxs-lookup"><span data-stu-id="1ca67-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="1ca67-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ca67-105">Properties</span></span>
| <span data-ttu-id="1ca67-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ca67-106">Property</span></span>     | <span data-ttu-id="1ca67-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ca67-107">Type</span></span>   |<span data-ttu-id="1ca67-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ca67-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ca67-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ca67-109">completedDateTime</span></span>|[<span data-ttu-id="1ca67-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1ca67-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="1ca67-111">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="1ca67-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="1ca67-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="1ca67-112">dueDateTime</span></span>|<span data-ttu-id="1ca67-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="1ca67-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="1ca67-114">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="1ca67-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="1ca67-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="1ca67-115">flagStatus</span></span>|<span data-ttu-id="1ca67-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="1ca67-116">followupFlagStatus</span></span>|<span data-ttu-id="1ca67-117">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="1ca67-117">The status for follow-up for an item.</span></span> <span data-ttu-id="1ca67-118">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="1ca67-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="1ca67-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1ca67-119">startDateTime</span></span>|<span data-ttu-id="1ca67-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="1ca67-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="1ca67-121">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="1ca67-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ca67-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ca67-122">JSON representation</span></span>

<span data-ttu-id="1ca67-123">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1ca67-123">Here is a JSON representation of the resource</span></span>

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
