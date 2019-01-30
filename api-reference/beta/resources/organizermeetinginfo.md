---
title: tipo de recurso de organizerMeetingInfo
description: Informações da reunião que contém o organizador da reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3b7d21a313d8744f18c8b96549bc9470b587361c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641992"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="1a6b8-103">tipo de recurso de organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="1a6b8-103">organizerMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a6b8-104">Informações da reunião que contém o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="1a6b8-104">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="1a6b8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a6b8-105">Properties</span></span>

| <span data-ttu-id="1a6b8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a6b8-106">Property</span></span>                     | <span data-ttu-id="1a6b8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a6b8-107">Type</span></span>                          | <span data-ttu-id="1a6b8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a6b8-108">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="1a6b8-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="1a6b8-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="1a6b8-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a6b8-110">Boolean</span></span>                       | <span data-ttu-id="1a6b8-111">Indica se uma conversa pode continuar depois que deixa o host da conversa.</span><span class="sxs-lookup"><span data-stu-id="1a6b8-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="1a6b8-112">organizer</span><span class="sxs-lookup"><span data-stu-id="1a6b8-112">organizer</span></span>                    | [<span data-ttu-id="1a6b8-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="1a6b8-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="1a6b8-114">O organizador da identidade do Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1a6b8-114">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1a6b8-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a6b8-115">JSON representation</span></span>

<span data-ttu-id="1a6b8-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a6b8-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="1a6b8-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a6b8-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/organizermeetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
