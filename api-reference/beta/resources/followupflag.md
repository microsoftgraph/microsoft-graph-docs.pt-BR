---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2b4b33fc17eb8dfb44e46ac18cb18aaeabe3d06c
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062592"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="d3fc9-104">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="d3fc9-104">followupFlag resource type</span></span>

<span data-ttu-id="d3fc9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3fc9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3fc9-106">Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente.</span><span class="sxs-lookup"><span data-stu-id="d3fc9-106">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="d3fc9-107">Os itens com suporte incluem [message](message.md) e [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="d3fc9-107">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d3fc9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3fc9-108">Properties</span></span>
| <span data-ttu-id="d3fc9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3fc9-109">Property</span></span>     | <span data-ttu-id="d3fc9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3fc9-110">Type</span></span>   |<span data-ttu-id="d3fc9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3fc9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3fc9-112">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3fc9-112">completedDateTime</span></span>|[<span data-ttu-id="d3fc9-113">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d3fc9-113">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d3fc9-114">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="d3fc9-114">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="d3fc9-115">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="d3fc9-115">dueDateTime</span></span>|<span data-ttu-id="d3fc9-116">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="d3fc9-116">**dateTimeTimeZone**</span></span>|<span data-ttu-id="d3fc9-117">A data e a hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="d3fc9-117">The date and time that the follow up is to be finished.</span></span> <span data-ttu-id="d3fc9-118">**Observação**: para definir a data de conclusão, você também deve especificar `startDateTime`o; caso contrário, você receberá `400 Bad Request` uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d3fc9-118">**Note**: To set the due date, you must also specify the `startDateTime`; otherwise, you will get a `400 Bad Request` response.</span></span>|
|<span data-ttu-id="d3fc9-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="d3fc9-119">flagStatus</span></span>|<span data-ttu-id="d3fc9-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3fc9-120">String</span></span>|<span data-ttu-id="d3fc9-121">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="d3fc9-121">The status for follow-up for an item.</span></span> <span data-ttu-id="d3fc9-122">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="d3fc9-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="d3fc9-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d3fc9-123">startDateTime</span></span>|<span data-ttu-id="d3fc9-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="d3fc9-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="d3fc9-125">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="d3fc9-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3fc9-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3fc9-126">JSON representation</span></span>

<span data-ttu-id="d3fc9-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d3fc9-127">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
