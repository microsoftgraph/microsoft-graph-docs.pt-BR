---
title: tipo de recurso invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7e25e65fb87f664788b0649f188def29b62c13d2
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006688"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="ddee0-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="ddee0-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddee0-104">Este recurso é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.</span><span class="sxs-lookup"><span data-stu-id="ddee0-104">This resource is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="ddee0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddee0-105">Properties</span></span>

| <span data-ttu-id="ddee0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddee0-106">Property</span></span>                           | <span data-ttu-id="ddee0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddee0-107">Type</span></span>                          | <span data-ttu-id="ddee0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddee0-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="ddee0-109">EndpointType</span><span class="sxs-lookup"><span data-stu-id="ddee0-109">endpointType</span></span>                       | <span data-ttu-id="ddee0-110">String</span><span class="sxs-lookup"><span data-stu-id="ddee0-110">String</span></span>                        | <span data-ttu-id="ddee0-111">O tipo de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ddee0-111">The type of endpoint.</span></span> <span data-ttu-id="ddee0-112">Os valores possíveis são: `default` e `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="ddee0-112">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="ddee0-113">ladrões</span><span class="sxs-lookup"><span data-stu-id="ddee0-113">identity</span></span>                           | [<span data-ttu-id="ddee0-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="ddee0-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="ddee0-115">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="ddee0-115">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="ddee0-116">languageId</span><span class="sxs-lookup"><span data-stu-id="ddee0-116">languageId</span></span>                         | <span data-ttu-id="ddee0-117">String</span><span class="sxs-lookup"><span data-stu-id="ddee0-117">String</span></span>                        | <span data-ttu-id="ddee0-118">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="ddee0-118">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="ddee0-119">região</span><span class="sxs-lookup"><span data-stu-id="ddee0-119">region</span></span>                             | <span data-ttu-id="ddee0-120">String</span><span class="sxs-lookup"><span data-stu-id="ddee0-120">String</span></span>                        | <span data-ttu-id="ddee0-121">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="ddee0-121">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="ddee0-122">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="ddee0-122">replacesCallId</span></span>                     | <span data-ttu-id="ddee0-123">String</span><span class="sxs-lookup"><span data-stu-id="ddee0-123">String</span></span>                        | <span data-ttu-id="ddee0-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ddee0-124">Optional.</span></span> <span data-ttu-id="ddee0-125">A chamada na qual o idenity de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="ddee0-125">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="ddee0-126">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="ddee0-126">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ddee0-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddee0-127">JSON representation</span></span>

<span data-ttu-id="ddee0-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ddee0-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
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
