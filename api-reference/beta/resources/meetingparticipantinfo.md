---
title: tipo de recurso de meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ba727344b1f653125a482b592e7d28c11d1d3d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515024"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="23764-103">tipo de recurso de meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="23764-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23764-104">Informações sobre um participante em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="23764-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="23764-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23764-105">Properties</span></span>

| <span data-ttu-id="23764-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23764-106">Property</span></span>       | <span data-ttu-id="23764-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="23764-107">Type</span></span>                          | <span data-ttu-id="23764-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="23764-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="23764-109">[-Identity]</span><span class="sxs-lookup"><span data-stu-id="23764-109">identity</span></span>       | [<span data-ttu-id="23764-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="23764-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="23764-111">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="23764-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="23764-112">UPN</span><span class="sxs-lookup"><span data-stu-id="23764-112">upn</span></span>            | <span data-ttu-id="23764-113">String</span><span class="sxs-lookup"><span data-stu-id="23764-113">String</span></span>                        | <span data-ttu-id="23764-114">Nome principal de usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="23764-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="23764-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23764-115">JSON representation</span></span>

<span data-ttu-id="23764-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23764-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
