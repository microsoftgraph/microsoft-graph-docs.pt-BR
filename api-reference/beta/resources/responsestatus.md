---
title: Tipo de recurso responseStatus
description: O status de resposta de uma solicitação de reunião.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 0ee9c70baa5cdea45868feb1517623081f2b62b2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718457"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="b7ecb-103">Tipo de recurso responseStatus</span><span class="sxs-lookup"><span data-stu-id="b7ecb-103">responseStatus resource type</span></span>

<span data-ttu-id="b7ecb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7ecb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7ecb-105">O status de resposta de uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b7ecb-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="b7ecb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7ecb-106">Properties</span></span>

| <span data-ttu-id="b7ecb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7ecb-107">Property</span></span> | <span data-ttu-id="b7ecb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7ecb-108">Type</span></span>           | <span data-ttu-id="b7ecb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7ecb-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="b7ecb-110">response</span><span class="sxs-lookup"><span data-stu-id="b7ecb-110">response</span></span> | <span data-ttu-id="b7ecb-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7ecb-111">String</span></span>         | <span data-ttu-id="b7ecb-112">O tipo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b7ecb-112">The response type.</span></span> <span data-ttu-id="b7ecb-113">Os valores possíveis são: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="b7ecb-113">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="b7ecb-114">time</span><span class="sxs-lookup"><span data-stu-id="b7ecb-114">time</span></span>     | <span data-ttu-id="b7ecb-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7ecb-115">DateTimeOffset</span></span> | <span data-ttu-id="b7ecb-116">A data e hora em que a resposta retornou.</span><span class="sxs-lookup"><span data-stu-id="b7ecb-116">The date and time that the response was returned.</span></span> <span data-ttu-id="b7ecb-117">Usa o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b7ecb-117">It uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b7ecb-118">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b7ecb-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7ecb-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7ecb-119">JSON representation</span></span>

<span data-ttu-id="b7ecb-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b7ecb-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


