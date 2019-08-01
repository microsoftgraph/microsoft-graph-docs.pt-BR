---
title: Tipo de recurso responseStatus
description: O status de resposta de uma solicitação de reunião.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 03deeabfd789fe3e8912d5a431af21bc2c8e5256
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034661"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="6db52-103">Tipo de recurso responseStatus</span><span class="sxs-lookup"><span data-stu-id="6db52-103">responseStatus resource type</span></span>

<span data-ttu-id="6db52-104">O status de resposta de uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="6db52-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="6db52-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6db52-105">Properties</span></span>

| <span data-ttu-id="6db52-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6db52-106">Property</span></span> | <span data-ttu-id="6db52-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6db52-107">Type</span></span>           | <span data-ttu-id="6db52-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db52-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="6db52-109">response</span><span class="sxs-lookup"><span data-stu-id="6db52-109">response</span></span> | <span data-ttu-id="6db52-110">responseType</span><span class="sxs-lookup"><span data-stu-id="6db52-110">responseType</span></span>   | <span data-ttu-id="6db52-111">O tipo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6db52-111">The response type.</span></span> <span data-ttu-id="6db52-112">Os valores possíveis são: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="6db52-112">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="6db52-113">time</span><span class="sxs-lookup"><span data-stu-id="6db52-113">time</span></span>     | <span data-ttu-id="6db52-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6db52-114">DateTimeOffset</span></span> | <span data-ttu-id="6db52-p102">A data e hora em que a resposta retornou. Usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6db52-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="6db52-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6db52-118">JSON representation</span></span>

<span data-ttu-id="6db52-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6db52-119">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
