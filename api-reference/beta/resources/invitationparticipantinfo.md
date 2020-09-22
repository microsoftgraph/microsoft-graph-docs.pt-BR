---
title: tipo de recurso invitationParticipantInfo
description: Representa uma entidade que está sendo convidada para uma chamada de grupo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9193ec70a3884ba9bf25e4f1c8c33eb7c77d838f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989035"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="2d74c-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="2d74c-103">invitationParticipantInfo resource type</span></span>

<span data-ttu-id="2d74c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d74c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d74c-105">Representa uma entidade que está sendo convidada para uma chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="2d74c-105">Represents an entity that is being invited to a group call.</span></span> 

## <a name="properties"></a><span data-ttu-id="2d74c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d74c-106">Properties</span></span>

| <span data-ttu-id="2d74c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d74c-107">Property</span></span>                           | <span data-ttu-id="2d74c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d74c-108">Type</span></span>                          | <span data-ttu-id="2d74c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d74c-109">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="2d74c-110">EndpointType</span><span class="sxs-lookup"><span data-stu-id="2d74c-110">endpointType</span></span>                       | <span data-ttu-id="2d74c-111">String</span><span class="sxs-lookup"><span data-stu-id="2d74c-111">String</span></span>                        | <span data-ttu-id="2d74c-112">O tipo de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="2d74c-112">The type of endpoint.</span></span> <span data-ttu-id="2d74c-113">Os valores possíveis são: `default` e `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="2d74c-113">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="2d74c-114">ladrões</span><span class="sxs-lookup"><span data-stu-id="2d74c-114">identity</span></span>                           | [<span data-ttu-id="2d74c-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="2d74c-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="2d74c-116">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="2d74c-116">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="2d74c-117">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="2d74c-117">replacesCallId</span></span>                     | <span data-ttu-id="2d74c-118">String</span><span class="sxs-lookup"><span data-stu-id="2d74c-118">String</span></span>                        | <span data-ttu-id="2d74c-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2d74c-119">Optional.</span></span> <span data-ttu-id="2d74c-120">A chamada na qual o idenity de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="2d74c-120">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="2d74c-121">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="2d74c-121">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2d74c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d74c-122">JSON representation</span></span>

<span data-ttu-id="2d74c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d74c-123">The following is a JSON representation of the resource.</span></span>

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


