---
title: tipo de recurso invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 762e5dc75c03cda78581b90b54c3fea27a7f12f2
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636663"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="0e17a-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="0e17a-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e17a-104">Este recurso é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.</span><span class="sxs-lookup"><span data-stu-id="0e17a-104">This resource is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="0e17a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e17a-105">Properties</span></span>

| <span data-ttu-id="0e17a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e17a-106">Property</span></span>                           | <span data-ttu-id="0e17a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e17a-107">Type</span></span>                          | <span data-ttu-id="0e17a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e17a-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="0e17a-109">EndpointType</span><span class="sxs-lookup"><span data-stu-id="0e17a-109">endpointType</span></span>                       | <span data-ttu-id="0e17a-110">String</span><span class="sxs-lookup"><span data-stu-id="0e17a-110">String</span></span>                        | <span data-ttu-id="0e17a-111">O tipo de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="0e17a-111">The type of endpoint.</span></span> <span data-ttu-id="0e17a-112">Os valores possíveis são: `default` e `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="0e17a-112">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="0e17a-113">ladrões</span><span class="sxs-lookup"><span data-stu-id="0e17a-113">identity</span></span>                           | [<span data-ttu-id="0e17a-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="0e17a-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="0e17a-115">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="0e17a-115">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="0e17a-116">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="0e17a-116">replacesCallId</span></span>                     | <span data-ttu-id="0e17a-117">String</span><span class="sxs-lookup"><span data-stu-id="0e17a-117">String</span></span>                        | <span data-ttu-id="0e17a-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0e17a-118">Optional.</span></span> <span data-ttu-id="0e17a-119">A chamada na qual o idenity de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="0e17a-119">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="0e17a-120">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="0e17a-120">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0e17a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e17a-121">JSON representation</span></span>

<span data-ttu-id="0e17a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e17a-122">The following is a JSON representation of the resource.</span></span>

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
