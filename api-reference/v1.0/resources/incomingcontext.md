---
title: tipo de recurso incomingContext
description: Representa o contexto associado a uma chamada de entrada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6acd1928b223789df7580a5f74eefc723570ca93
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962527"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="64144-103">tipo de recurso incomingContext</span><span class="sxs-lookup"><span data-stu-id="64144-103">incomingContext resource type</span></span>

<span data-ttu-id="64144-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64144-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64144-105">Representa o contexto associado a uma chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="64144-105">Represents the context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="64144-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64144-106">Properties</span></span>

| <span data-ttu-id="64144-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64144-107">Property</span></span>              | <span data-ttu-id="64144-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="64144-108">Type</span></span>                          | <span data-ttu-id="64144-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="64144-109">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="64144-110">sourceParticipantId</span><span class="sxs-lookup"><span data-stu-id="64144-110">sourceParticipantId</span></span>   | <span data-ttu-id="64144-111">String</span><span class="sxs-lookup"><span data-stu-id="64144-111">String</span></span>                        | <span data-ttu-id="64144-112">A ID do participante que disparou a chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="64144-112">The ID of the participant that triggered the incoming call.</span></span> <span data-ttu-id="64144-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64144-113">Read-only.</span></span>  |
| <span data-ttu-id="64144-114">observedParticipantId</span><span class="sxs-lookup"><span data-stu-id="64144-114">observedParticipantId</span></span> | <span data-ttu-id="64144-115">String</span><span class="sxs-lookup"><span data-stu-id="64144-115">String</span></span>                        | <span data-ttu-id="64144-116">A ID do participante que está sob observação.</span><span class="sxs-lookup"><span data-stu-id="64144-116">The ID of the participant that is under observation.</span></span> <span data-ttu-id="64144-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64144-117">Read-only.</span></span>         |
| <span data-ttu-id="64144-118">onBehalfOf</span><span class="sxs-lookup"><span data-stu-id="64144-118">onBehalfOf</span></span>            | [<span data-ttu-id="64144-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="64144-119">identitySet</span></span>](identityset.md) | <span data-ttu-id="64144-120">A identidade em que a chamada está acontecendo em nome de.</span><span class="sxs-lookup"><span data-stu-id="64144-120">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="64144-121">transferidar</span><span class="sxs-lookup"><span data-stu-id="64144-121">transferor</span></span>            | [<span data-ttu-id="64144-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="64144-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="64144-123">A identidade que transferiu a chamada.</span><span class="sxs-lookup"><span data-stu-id="64144-123">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="64144-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64144-124">JSON representation</span></span>

<span data-ttu-id="64144-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64144-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sourceParticipantId",
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "sourceParticipantId": "String",
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
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
