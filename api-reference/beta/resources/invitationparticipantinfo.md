---
title: tipo de recurso de invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associado a um convite para conversa e fornece os parâmetros adicionais de convite.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520673"
---
# <a name="invitationparticipantinfo-resource-type"></a><span data-ttu-id="0c2b5-103">tipo de recurso de invitationParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="0c2b5-103">invitationParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c2b5-104">O **InvitationParticipant** é usado para representar um conjunto de identidades associado a um convite para conversa e fornece os parâmetros adicionais de convite.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-104">The **InvitationParticipant** is used to represent a set of identities associated with a conversation invitation, and provides additional invitation parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="0c2b5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c2b5-105">Properties</span></span>

| <span data-ttu-id="0c2b5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c2b5-106">Property</span></span>                           | <span data-ttu-id="0c2b5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c2b5-107">Type</span></span>                          | <span data-ttu-id="0c2b5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c2b5-108">Description</span></span>                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| <span data-ttu-id="0c2b5-109">endpointType</span><span class="sxs-lookup"><span data-stu-id="0c2b5-109">endpointType</span></span>                       | <span data-ttu-id="0c2b5-110">String</span><span class="sxs-lookup"><span data-stu-id="0c2b5-110">String</span></span>                        | <span data-ttu-id="0c2b5-111">Os valores possíveis são: `default` e `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-111">Possible values are: `default`, `voicemail`.</span></span> |
| <span data-ttu-id="0c2b5-112">identity</span><span class="sxs-lookup"><span data-stu-id="0c2b5-112">identity</span></span>                           | [<span data-ttu-id="0c2b5-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="0c2b5-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="0c2b5-114">O [identitySet](identityset.md) associado a este convite.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-114">The [identitySet](identityset.md) associated with this invitation.</span></span>                   |
| <span data-ttu-id="0c2b5-115">languageId</span><span class="sxs-lookup"><span data-stu-id="0c2b5-115">languageId</span></span>                         | <span data-ttu-id="0c2b5-116">String</span><span class="sxs-lookup"><span data-stu-id="0c2b5-116">String</span></span>                        | <span data-ttu-id="0c2b5-117">A cadeia de caracteres de cultura do idioma.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-117">The language culture string.</span></span>                                                                                     |
| <span data-ttu-id="0c2b5-118">Região</span><span class="sxs-lookup"><span data-stu-id="0c2b5-118">region</span></span>                             | <span data-ttu-id="0c2b5-119">String</span><span class="sxs-lookup"><span data-stu-id="0c2b5-119">String</span></span>                        | <span data-ttu-id="0c2b5-120">Região do participante.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-120">Region of the participant.</span></span>                                                           |
| <span data-ttu-id="0c2b5-121">replacesCallId</span><span class="sxs-lookup"><span data-stu-id="0c2b5-121">replacesCallId</span></span>                     | <span data-ttu-id="0c2b5-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c2b5-122">String</span></span>                        | <span data-ttu-id="0c2b5-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-123">Optional.</span></span> <span data-ttu-id="0c2b5-124">A chamada que o idenity de destino no momento é parte do.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-124">The call which the target idenity is currently a part of.</span></span> <span data-ttu-id="0c2b5-125">Essa chamada será descartada depois que o participante é adicionado.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-125">This call will be dropped once the participant is added.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0c2b5-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c2b5-126">JSON representation</span></span>

<span data-ttu-id="0c2b5-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c2b5-127">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
