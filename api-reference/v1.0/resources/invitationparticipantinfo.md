---
title: tipo de recurso invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1e1dc861fb1580744ed3b956338934a443f0e661
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865659"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="ab7e4-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="ab7e4-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="ab7e4-104">Este recurso é usado para representar a entidade que está sendo convidada para uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="ab7e4-104">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="ab7e4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab7e4-105">Properties</span></span>

| <span data-ttu-id="ab7e4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab7e4-106">Property</span></span>                           | <span data-ttu-id="ab7e4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab7e4-107">Type</span></span>                          | <span data-ttu-id="ab7e4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab7e4-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="ab7e4-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="ab7e4-109">identity</span></span>                           | [<span data-ttu-id="ab7e4-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="ab7e4-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="ab7e4-111">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="ab7e4-111">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="ab7e4-112">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="ab7e4-112">replacesCallId</span></span>                     | <span data-ttu-id="ab7e4-113">String</span><span class="sxs-lookup"><span data-stu-id="ab7e4-113">String</span></span>                        | <span data-ttu-id="ab7e4-114">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ab7e4-114">Optional.</span></span> <span data-ttu-id="ab7e4-115">A chamada na qual a identidade de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="ab7e4-115">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="ab7e4-116">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="ab7e4-116">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab7e4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab7e4-117">JSON representation</span></span>

<span data-ttu-id="ab7e4-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab7e4-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
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
