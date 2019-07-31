---
title: tipo de recurso meetingCapability
description: Contém os recursos de uma reunião
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1de406cf0614a4cbb64749cef763a97a3723eb48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966837"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="887ca-103">tipo de recurso meetingCapability</span><span class="sxs-lookup"><span data-stu-id="887ca-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="887ca-104">Contém os recursos de uma reunião</span><span class="sxs-lookup"><span data-stu-id="887ca-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="887ca-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="887ca-105">Properties</span></span>

| <span data-ttu-id="887ca-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="887ca-106">Property</span></span>                          | <span data-ttu-id="887ca-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="887ca-107">Type</span></span>    | <span data-ttu-id="887ca-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="887ca-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="887ca-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="887ca-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="887ca-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="887ca-110">Boolean</span></span> | <span data-ttu-id="887ca-111">Indica se os usuários anônimos de discagem são permitidos em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="887ca-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="887ca-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="887ca-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="887ca-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="887ca-113">Boolean</span></span> | <span data-ttu-id="887ca-114">Indica se os usuários anônimos podem iniciar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="887ca-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="887ca-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="887ca-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="887ca-116">String</span><span class="sxs-lookup"><span data-stu-id="887ca-116">String</span></span>  | <span data-ttu-id="887ca-117">Os valores possíveis são: `everyoneInCompany` e `everyone`.</span><span class="sxs-lookup"><span data-stu-id="887ca-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="887ca-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="887ca-118">JSON representation</span></span>

<span data-ttu-id="887ca-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="887ca-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
