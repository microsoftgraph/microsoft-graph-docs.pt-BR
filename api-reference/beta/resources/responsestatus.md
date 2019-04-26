---
title: Tipo de recurso responseStatus
description: O status de resposta de uma solicitação de reunião.
localization_priority: Normal
ms.openlocfilehash: 8ec4b5f74fa8d83369c23f829b34dfa0ed53a1a1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343574"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="5fa56-103">Tipo de recurso responseStatus</span><span class="sxs-lookup"><span data-stu-id="5fa56-103">responseStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fa56-104">O status de resposta de uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="5fa56-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="5fa56-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fa56-105">Properties</span></span>

| <span data-ttu-id="5fa56-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fa56-106">Property</span></span> | <span data-ttu-id="5fa56-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fa56-107">Type</span></span>           | <span data-ttu-id="5fa56-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fa56-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="5fa56-109">response</span><span class="sxs-lookup"><span data-stu-id="5fa56-109">response</span></span> | <span data-ttu-id="5fa56-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fa56-110">String</span></span>         | <span data-ttu-id="5fa56-111">O tipo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5fa56-111">The response type.</span></span> <span data-ttu-id="5fa56-112">Os valores possíveis são: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="5fa56-112">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="5fa56-113">time</span><span class="sxs-lookup"><span data-stu-id="5fa56-113">time</span></span>     | <span data-ttu-id="5fa56-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fa56-114">DateTimeOffset</span></span> | <span data-ttu-id="5fa56-p102">A data e hora em que a resposta retornou. Usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5fa56-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fa56-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fa56-118">JSON representation</span></span>

<span data-ttu-id="5fa56-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5fa56-119">Here is a JSON representation of the resource</span></span>

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
