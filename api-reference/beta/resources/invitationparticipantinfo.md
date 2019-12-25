---
title: tipo de recurso invitationParticipantInfo
description: Representa uma entidade que está sendo convidada para uma chamada de grupo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bddce0358bfa0ec46d8231958817002cb4ca8c20
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870219"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="eeedb-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="eeedb-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeedb-104">Representa uma entidade que está sendo convidada para uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="eeedb-104">Represents an entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="eeedb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eeedb-105">Properties</span></span>

| <span data-ttu-id="eeedb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeedb-106">Property</span></span>                           | <span data-ttu-id="eeedb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeedb-107">Type</span></span>                          | <span data-ttu-id="eeedb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeedb-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="eeedb-109">EndpointType</span><span class="sxs-lookup"><span data-stu-id="eeedb-109">endpointType</span></span>                       | <span data-ttu-id="eeedb-110">String</span><span class="sxs-lookup"><span data-stu-id="eeedb-110">String</span></span>                        | <span data-ttu-id="eeedb-111">O tipo de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="eeedb-111">The type of endpoint.</span></span> <span data-ttu-id="eeedb-112">Os valores possíveis são: `default` e `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="eeedb-112">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="eeedb-113">ladrões</span><span class="sxs-lookup"><span data-stu-id="eeedb-113">identity</span></span>                           | [<span data-ttu-id="eeedb-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="eeedb-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="eeedb-115">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="eeedb-115">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="eeedb-116">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="eeedb-116">replacesCallId</span></span>                     | <span data-ttu-id="eeedb-117">String</span><span class="sxs-lookup"><span data-stu-id="eeedb-117">String</span></span>                        | <span data-ttu-id="eeedb-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eeedb-118">Optional.</span></span> <span data-ttu-id="eeedb-119">A chamada na qual o idenity de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="eeedb-119">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="eeedb-120">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="eeedb-120">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eeedb-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eeedb-121">JSON representation</span></span>

<span data-ttu-id="eeedb-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eeedb-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "endpointType",
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
