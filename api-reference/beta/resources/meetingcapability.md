---
title: tipo de recurso meetingCapability
description: Contém os recursos de uma reunião
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b891a9e6d0eb90a527c79528e9fd595c2f8ca5b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913622"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="fb2fa-103">tipo de recurso meetingCapability</span><span class="sxs-lookup"><span data-stu-id="fb2fa-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb2fa-104">Contém os recursos de uma reunião</span><span class="sxs-lookup"><span data-stu-id="fb2fa-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="fb2fa-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb2fa-105">Properties</span></span>

| <span data-ttu-id="fb2fa-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb2fa-106">Property</span></span>                          | <span data-ttu-id="fb2fa-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb2fa-107">Type</span></span>    | <span data-ttu-id="fb2fa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb2fa-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="fb2fa-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="fb2fa-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="fb2fa-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="fb2fa-110">Boolean</span></span> | <span data-ttu-id="fb2fa-111">Indica se os usuários anônimos de discagem são permitidos em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="fb2fa-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="fb2fa-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="fb2fa-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="fb2fa-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="fb2fa-113">Boolean</span></span> | <span data-ttu-id="fb2fa-114">Indica se os usuários anônimos podem iniciar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="fb2fa-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="fb2fa-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="fb2fa-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="fb2fa-116">String</span><span class="sxs-lookup"><span data-stu-id="fb2fa-116">String</span></span>  | <span data-ttu-id="fb2fa-117">Os valores possíveis são: `everyoneInCompany` e `everyone`.</span><span class="sxs-lookup"><span data-stu-id="fb2fa-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="fb2fa-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb2fa-118">JSON representation</span></span>

<span data-ttu-id="fb2fa-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb2fa-119">The following is a JSON representation of the resource.</span></span>

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
