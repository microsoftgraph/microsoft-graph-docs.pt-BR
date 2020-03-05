---
title: tipo de recurso invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4a4d34e94fc54cd47ed6773e91c2fb62f0b62ce4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447707"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="65dae-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="65dae-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="65dae-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="65dae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65dae-105">Este recurso é usado para representar a entidade que está sendo convidada para uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="65dae-105">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="65dae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65dae-106">Properties</span></span>

| <span data-ttu-id="65dae-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65dae-107">Property</span></span>                           | <span data-ttu-id="65dae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="65dae-108">Type</span></span>                          | <span data-ttu-id="65dae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="65dae-109">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="65dae-110">ladrões</span><span class="sxs-lookup"><span data-stu-id="65dae-110">identity</span></span>                           | [<span data-ttu-id="65dae-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="65dae-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="65dae-112">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="65dae-112">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="65dae-113">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="65dae-113">replacesCallId</span></span>                     | <span data-ttu-id="65dae-114">String</span><span class="sxs-lookup"><span data-stu-id="65dae-114">String</span></span>                        | <span data-ttu-id="65dae-115">Opcional.</span><span class="sxs-lookup"><span data-stu-id="65dae-115">Optional.</span></span> <span data-ttu-id="65dae-116">A chamada na qual a identidade de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="65dae-116">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="65dae-117">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="65dae-117">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65dae-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65dae-118">JSON representation</span></span>

<span data-ttu-id="65dae-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65dae-119">The following is a JSON representation of the resource.</span></span>

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
