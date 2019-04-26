---
title: tipo de recurso invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 56eb1ad90410edca795a8e29ecaa4b8b94e915ee
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345418"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="60c81-103">tipo de recurso invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="60c81-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60c81-104">O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.</span><span class="sxs-lookup"><span data-stu-id="60c81-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="60c81-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60c81-105">Properties</span></span>

| <span data-ttu-id="60c81-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60c81-106">Property</span></span>                           | <span data-ttu-id="60c81-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="60c81-107">Type</span></span>                          | <span data-ttu-id="60c81-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="60c81-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="60c81-109">EndpointType</span><span class="sxs-lookup"><span data-stu-id="60c81-109">endpointType</span></span>                       | <span data-ttu-id="60c81-110">String</span><span class="sxs-lookup"><span data-stu-id="60c81-110">String</span></span>                        | <span data-ttu-id="60c81-111">Os valores possíveis são: `default` e `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="60c81-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="60c81-112">ladrões</span><span class="sxs-lookup"><span data-stu-id="60c81-112">identity</span></span>                           | [<span data-ttu-id="60c81-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="60c81-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="60c81-114">O [identityset](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="60c81-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="60c81-115">languageId</span><span class="sxs-lookup"><span data-stu-id="60c81-115">languageId</span></span>                         | <span data-ttu-id="60c81-116">String</span><span class="sxs-lookup"><span data-stu-id="60c81-116">String</span></span>                        | <span data-ttu-id="60c81-117">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="60c81-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="60c81-118">região</span><span class="sxs-lookup"><span data-stu-id="60c81-118">region</span></span>                             | <span data-ttu-id="60c81-119">String</span><span class="sxs-lookup"><span data-stu-id="60c81-119">String</span></span>                        | <span data-ttu-id="60c81-120">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="60c81-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="60c81-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="60c81-121">replacesCallId</span></span>                     | <span data-ttu-id="60c81-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60c81-122">String</span></span>                        | <span data-ttu-id="60c81-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="60c81-123">Optional.</span></span> <span data-ttu-id="60c81-124">A chamada na qual o idenity de destino faz parte no momento.</span><span class="sxs-lookup"><span data-stu-id="60c81-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="60c81-125">Essa chamada será cancelada quando o participante for adicionado.</span><span class="sxs-lookup"><span data-stu-id="60c81-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60c81-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60c81-126">JSON representation</span></span>

<span data-ttu-id="60c81-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60c81-127">The following is a JSON representation of the resource.</span></span>

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
