---
title: tipo de recurso incomingContext
description: O contexto associado a uma chamada recebida.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a7eba09d18b2b60c3a5ae45a8ad335d8971d2c77
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496373"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="1a080-103">tipo de recurso incomingContext</span><span class="sxs-lookup"><span data-stu-id="1a080-103">incomingContext resource type</span></span>

<span data-ttu-id="1a080-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1a080-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a080-105">O contexto associado a uma chamada recebida.</span><span class="sxs-lookup"><span data-stu-id="1a080-105">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="1a080-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a080-106">Properties</span></span>

| <span data-ttu-id="1a080-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a080-107">Property</span></span>              | <span data-ttu-id="1a080-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a080-108">Type</span></span>                          | <span data-ttu-id="1a080-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a080-109">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="1a080-110">observedParticipantId</span><span class="sxs-lookup"><span data-stu-id="1a080-110">observedParticipantId</span></span> | <span data-ttu-id="1a080-111">String</span><span class="sxs-lookup"><span data-stu-id="1a080-111">String</span></span>                        | <span data-ttu-id="1a080-112">A ID do participante que está sob observação.</span><span class="sxs-lookup"><span data-stu-id="1a080-112">The id of the participant that is under observation.</span></span> <span data-ttu-id="1a080-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a080-113">Read-only.</span></span>         |
| <span data-ttu-id="1a080-114">onBehalfOf</span><span class="sxs-lookup"><span data-stu-id="1a080-114">onBehalfOf</span></span>            | [<span data-ttu-id="1a080-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="1a080-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="1a080-116">A identidade em que a chamada está acontecendo em nome de.</span><span class="sxs-lookup"><span data-stu-id="1a080-116">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="1a080-117">sourceParticipantId</span><span class="sxs-lookup"><span data-stu-id="1a080-117">sourceParticipantId</span></span>   | <span data-ttu-id="1a080-118">String</span><span class="sxs-lookup"><span data-stu-id="1a080-118">String</span></span>                        | <span data-ttu-id="1a080-119">A ID do participante que disparou a chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="1a080-119">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="1a080-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a080-120">Read-only.</span></span>  |
| <span data-ttu-id="1a080-121">transferidar</span><span class="sxs-lookup"><span data-stu-id="1a080-121">transferor</span></span>            | [<span data-ttu-id="1a080-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="1a080-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="1a080-123">A identidade que transferiu a chamada.</span><span class="sxs-lookup"><span data-stu-id="1a080-123">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="1a080-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a080-124">JSON representation</span></span>

<span data-ttu-id="1a080-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a080-125">The following is a JSON representation of the resource.</span></span>

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
