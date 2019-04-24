---
title: tipo de recurso meetingCapability
description: Contém os recursos de uma reunião
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e71d7c8c6489d5856e5f2441cd93c7fdea033bd4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457141"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="2f210-103">tipo de recurso meetingCapability</span><span class="sxs-lookup"><span data-stu-id="2f210-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f210-104">Contém os recursos de uma reunião</span><span class="sxs-lookup"><span data-stu-id="2f210-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="2f210-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f210-105">Properties</span></span>

| <span data-ttu-id="2f210-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f210-106">Property</span></span>                          | <span data-ttu-id="2f210-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f210-107">Type</span></span>    | <span data-ttu-id="2f210-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f210-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="2f210-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="2f210-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="2f210-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f210-110">Boolean</span></span> | <span data-ttu-id="2f210-111">Indica se os usuários anônimos de discagem são permitidos em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="2f210-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="2f210-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="2f210-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="2f210-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f210-113">Boolean</span></span> | <span data-ttu-id="2f210-114">Indica se os usuários anônimos podem iniciar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="2f210-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="2f210-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="2f210-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="2f210-116">String</span><span class="sxs-lookup"><span data-stu-id="2f210-116">String</span></span>  | <span data-ttu-id="2f210-117">Os valores possíveis são: `everyoneInCompany` e `everyone`.</span><span class="sxs-lookup"><span data-stu-id="2f210-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="2f210-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f210-118">JSON representation</span></span>

<span data-ttu-id="2f210-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f210-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingcapability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
