---
title: Tipo de recurso followupFlag
description: Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente. Os itens com suporte incluem message e contact.
localization_priority: Normal
ms.openlocfilehash: aa056d141bfac82b9f039ed705f6de49893783fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869374"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="dcf69-104">Tipo de recurso followupFlag</span><span class="sxs-lookup"><span data-stu-id="dcf69-104">followupFlag resource type</span></span>

> <span data-ttu-id="dcf69-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dcf69-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dcf69-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dcf69-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dcf69-107">Permite definir um sinalizador para que o usuário possa acompanhar um item posteriormente.</span><span class="sxs-lookup"><span data-stu-id="dcf69-107">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="dcf69-108">Os itens com suporte incluem [message](message.md) e [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="dcf69-108">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dcf69-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dcf69-109">Properties</span></span>
| <span data-ttu-id="dcf69-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dcf69-110">Property</span></span>     | <span data-ttu-id="dcf69-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcf69-111">Type</span></span>   |<span data-ttu-id="dcf69-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcf69-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcf69-113">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcf69-113">completedDateTime</span></span>|[<span data-ttu-id="dcf69-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="dcf69-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="dcf69-115">Data e hora em que o acompanhamento foi concluído.</span><span class="sxs-lookup"><span data-stu-id="dcf69-115">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="dcf69-116">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="dcf69-116">dueDateTime</span></span>|<span data-ttu-id="dcf69-117">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="dcf69-117">**dateTimeTimeZone**</span></span>|<span data-ttu-id="dcf69-118">Data e hora em que o acompanhamento deve ser concluído.</span><span class="sxs-lookup"><span data-stu-id="dcf69-118">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="dcf69-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="dcf69-119">flagStatus</span></span>|<span data-ttu-id="dcf69-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcf69-120">String</span></span>|<span data-ttu-id="dcf69-121">O status de acompanhamento de um item.</span><span class="sxs-lookup"><span data-stu-id="dcf69-121">The status for follow-up for an item.</span></span> <span data-ttu-id="dcf69-122">Os valores possíveis são: `notFlagged`, `complete` e `flagged`.</span><span class="sxs-lookup"><span data-stu-id="dcf69-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="dcf69-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dcf69-123">startDateTime</span></span>|<span data-ttu-id="dcf69-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="dcf69-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="dcf69-125">Data e hora em que o acompanhamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="dcf69-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dcf69-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dcf69-126">JSON representation</span></span>

<span data-ttu-id="dcf69-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="dcf69-127">Here is a JSON representation of the resource</span></span>

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
