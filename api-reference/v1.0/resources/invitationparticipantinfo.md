---
title: tipo de recurso invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b42e89f89332e58fa2f7edcf39c774446c6b9d9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913398"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="0e03c-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="0e03c-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="0e03c-104">Este recurso é usado para representar a entidade que está sendo convidada para uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="0e03c-104">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="0e03c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e03c-105">Properties</span></span>

| <span data-ttu-id="0e03c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e03c-106">Property</span></span>                           | <span data-ttu-id="0e03c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e03c-107">Type</span></span>                          | <span data-ttu-id="0e03c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e03c-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="0e03c-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="0e03c-109">identity</span></span>                           | [<span data-ttu-id="0e03c-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="0e03c-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="0e03c-111">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="0e03c-111">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="0e03c-112">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="0e03c-112">replacesCallId</span></span>                     | <span data-ttu-id="0e03c-113">String</span><span class="sxs-lookup"><span data-stu-id="0e03c-113">String</span></span>                        | <span data-ttu-id="0e03c-114">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0e03c-114">Optional.</span></span> <span data-ttu-id="0e03c-115">A chamada na qual a identidade de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="0e03c-115">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="0e03c-116">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="0e03c-116">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0e03c-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e03c-117">JSON representation</span></span>

<span data-ttu-id="0e03c-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e03c-118">The following is a JSON representation of the resource.</span></span>

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
