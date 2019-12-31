---
title: tipo de recurso incomingContext
description: O contexto associado a uma chamada recebida.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4ade91c621dabdb7867ff5a4586276265d73ca81
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913524"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="ee924-103">tipo de recurso incomingContext</span><span class="sxs-lookup"><span data-stu-id="ee924-103">incomingContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee924-104">O contexto associado a uma chamada recebida.</span><span class="sxs-lookup"><span data-stu-id="ee924-104">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="ee924-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee924-105">Properties</span></span>

| <span data-ttu-id="ee924-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee924-106">Property</span></span>              | <span data-ttu-id="ee924-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee924-107">Type</span></span>                          | <span data-ttu-id="ee924-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee924-108">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="ee924-109">observedParticipantId</span><span class="sxs-lookup"><span data-stu-id="ee924-109">observedParticipantId</span></span> | <span data-ttu-id="ee924-110">String</span><span class="sxs-lookup"><span data-stu-id="ee924-110">String</span></span>                        | <span data-ttu-id="ee924-111">A ID do participante que está sob observação.</span><span class="sxs-lookup"><span data-stu-id="ee924-111">The id of the participant that is under observation.</span></span> <span data-ttu-id="ee924-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee924-112">Read-only.</span></span>         |
| <span data-ttu-id="ee924-113">onBehalfOf</span><span class="sxs-lookup"><span data-stu-id="ee924-113">onBehalfOf</span></span>            | [<span data-ttu-id="ee924-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee924-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="ee924-115">A identidade em que a chamada está acontecendo em nome de.</span><span class="sxs-lookup"><span data-stu-id="ee924-115">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="ee924-116">sourceParticipantId</span><span class="sxs-lookup"><span data-stu-id="ee924-116">sourceParticipantId</span></span>   | <span data-ttu-id="ee924-117">String</span><span class="sxs-lookup"><span data-stu-id="ee924-117">String</span></span>                        | <span data-ttu-id="ee924-118">A ID do participante que disparou a chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="ee924-118">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="ee924-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee924-119">Read-only.</span></span>  |
| <span data-ttu-id="ee924-120">transferidar</span><span class="sxs-lookup"><span data-stu-id="ee924-120">transferor</span></span>            | [<span data-ttu-id="ee924-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee924-121">identitySet</span></span>](identityset.md) | <span data-ttu-id="ee924-122">A identidade que transferiu a chamada.</span><span class="sxs-lookup"><span data-stu-id="ee924-122">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="ee924-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee924-123">JSON representation</span></span>

<span data-ttu-id="ee924-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee924-124">The following is a JSON representation of the resource.</span></span>

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
