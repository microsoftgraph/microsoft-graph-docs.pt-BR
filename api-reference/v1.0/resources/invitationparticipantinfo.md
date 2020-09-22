---
title: tipo de recurso invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2425f7ebd6ac516a9100605c9ebfe47f1b87a114
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984247"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="67e86-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="67e86-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="67e86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67e86-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67e86-105">Este recurso é usado para representar a entidade que está sendo convidada para uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="67e86-105">This resource is used to represent the entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="67e86-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67e86-106">Properties</span></span>

| <span data-ttu-id="67e86-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67e86-107">Property</span></span>                           | <span data-ttu-id="67e86-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="67e86-108">Type</span></span>                          | <span data-ttu-id="67e86-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="67e86-109">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="67e86-110">ladrões</span><span class="sxs-lookup"><span data-stu-id="67e86-110">identity</span></span>                           | [<span data-ttu-id="67e86-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="67e86-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="67e86-112">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="67e86-112">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="67e86-113">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="67e86-113">replacesCallId</span></span>                     | <span data-ttu-id="67e86-114">String</span><span class="sxs-lookup"><span data-stu-id="67e86-114">String</span></span>                        | <span data-ttu-id="67e86-115">Opcional.</span><span class="sxs-lookup"><span data-stu-id="67e86-115">Optional.</span></span> <span data-ttu-id="67e86-116">A chamada na qual a identidade de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="67e86-116">The call which the target identity is currently a part of.</span></span> <span data-ttu-id="67e86-117">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="67e86-117">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67e86-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67e86-118">JSON representation</span></span>

<span data-ttu-id="67e86-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67e86-119">The following is a JSON representation of the resource.</span></span>

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

