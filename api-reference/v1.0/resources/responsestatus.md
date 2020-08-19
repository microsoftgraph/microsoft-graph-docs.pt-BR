---
title: Tipo de recurso responseStatus
description: O status de resposta de uma solicitação de reunião.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 77adc43ef3485f7fcf42a8c1c77edc5d123a3424
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812657"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="1846e-103">Tipo de recurso responseStatus</span><span class="sxs-lookup"><span data-stu-id="1846e-103">responseStatus resource type</span></span>

<span data-ttu-id="1846e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1846e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1846e-105">O status de resposta de uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="1846e-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="1846e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1846e-106">Properties</span></span>

| <span data-ttu-id="1846e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1846e-107">Property</span></span> | <span data-ttu-id="1846e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1846e-108">Type</span></span>           | <span data-ttu-id="1846e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1846e-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="1846e-110">response</span><span class="sxs-lookup"><span data-stu-id="1846e-110">response</span></span> | <span data-ttu-id="1846e-111">responseType</span><span class="sxs-lookup"><span data-stu-id="1846e-111">responseType</span></span>   | <span data-ttu-id="1846e-112">O tipo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1846e-112">The response type.</span></span> <span data-ttu-id="1846e-113">Os valores possíveis são: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span><span class="sxs-lookup"><span data-stu-id="1846e-113">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="1846e-114">time</span><span class="sxs-lookup"><span data-stu-id="1846e-114">time</span></span>     | <span data-ttu-id="1846e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1846e-115">DateTimeOffset</span></span> | <span data-ttu-id="1846e-p102">A data e hora em que a resposta retornou. Usa o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1846e-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="1846e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1846e-119">JSON representation</span></span>

<span data-ttu-id="1846e-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1846e-120">Here is a JSON representation of the resource</span></span>

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
