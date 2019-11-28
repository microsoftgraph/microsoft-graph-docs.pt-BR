---
title: tipo de recurso incomingContext
description: O contexto associado a uma chamada de entrada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0afe972be631a2048b2a1970b1fda41e8cb72920
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636894"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="be53c-103">tipo de recurso incomingContext</span><span class="sxs-lookup"><span data-stu-id="be53c-103">incomingContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be53c-104">O contexto associado a uma chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="be53c-104">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="be53c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be53c-105">Properties</span></span>

| <span data-ttu-id="be53c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be53c-106">Property</span></span>              | <span data-ttu-id="be53c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="be53c-107">Type</span></span>                          | <span data-ttu-id="be53c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="be53c-108">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="be53c-109">observedParticipantId</span><span class="sxs-lookup"><span data-stu-id="be53c-109">observedParticipantId</span></span> | <span data-ttu-id="be53c-110">String</span><span class="sxs-lookup"><span data-stu-id="be53c-110">String</span></span>                        | <span data-ttu-id="be53c-111">A ID do participante que está sob observação.</span><span class="sxs-lookup"><span data-stu-id="be53c-111">The id of the participant that is under observation.</span></span> <span data-ttu-id="be53c-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be53c-112">Read-only.</span></span>         |
| <span data-ttu-id="be53c-113">onBehalfOf</span><span class="sxs-lookup"><span data-stu-id="be53c-113">onBehalfOf</span></span>            | [<span data-ttu-id="be53c-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="be53c-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="be53c-115">A identidade em que a chamada está acontecendo em nome de.</span><span class="sxs-lookup"><span data-stu-id="be53c-115">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="be53c-116">sourceParticipantId</span><span class="sxs-lookup"><span data-stu-id="be53c-116">sourceParticipantId</span></span>   | <span data-ttu-id="be53c-117">String</span><span class="sxs-lookup"><span data-stu-id="be53c-117">String</span></span>                        | <span data-ttu-id="be53c-118">A ID do participante que disparou a chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="be53c-118">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="be53c-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be53c-119">Read-only.</span></span>  |
| <span data-ttu-id="be53c-120">transferidar</span><span class="sxs-lookup"><span data-stu-id="be53c-120">transferor</span></span>            | [<span data-ttu-id="be53c-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="be53c-121">identitySet</span></span>](identityset.md) | <span data-ttu-id="be53c-122">A identidade que transferiu a chamada.</span><span class="sxs-lookup"><span data-stu-id="be53c-122">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="be53c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be53c-123">JSON representation</span></span>

<span data-ttu-id="be53c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be53c-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
  "sourceParticipantId": "String",
  "transferor": {"@odata.type": "#microsoft.graph.identitySet"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "incomingContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
