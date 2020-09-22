---
title: tipo de recurso meetingCapability
description: Contém os recursos de uma reunião
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 29da5c8d4796e393bfead08979aca8e58a95024d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971682"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="801b2-103">tipo de recurso meetingCapability</span><span class="sxs-lookup"><span data-stu-id="801b2-103">meetingCapability resource type</span></span>

<span data-ttu-id="801b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="801b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="801b2-105">Contém os recursos de uma reunião</span><span class="sxs-lookup"><span data-stu-id="801b2-105">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="801b2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="801b2-106">Properties</span></span>

| <span data-ttu-id="801b2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="801b2-107">Property</span></span>                          | <span data-ttu-id="801b2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="801b2-108">Type</span></span>    | <span data-ttu-id="801b2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="801b2-109">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="801b2-110">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="801b2-110">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="801b2-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="801b2-111">Boolean</span></span> | <span data-ttu-id="801b2-112">Indica se os usuários anônimos de discagem são permitidos em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="801b2-112">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="801b2-113">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="801b2-113">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="801b2-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="801b2-114">Boolean</span></span> | <span data-ttu-id="801b2-115">Indica se os usuários anônimos podem iniciar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="801b2-115">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="801b2-116">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="801b2-116">autoAdmittedUsers</span></span>                 | <span data-ttu-id="801b2-117">String</span><span class="sxs-lookup"><span data-stu-id="801b2-117">String</span></span>  | <span data-ttu-id="801b2-118">Os valores possíveis são: `everyoneInCompany` e `everyone`.</span><span class="sxs-lookup"><span data-stu-id="801b2-118">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="801b2-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="801b2-119">JSON representation</span></span>

<span data-ttu-id="801b2-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="801b2-120">The following is a JSON representation of the resource.</span></span>

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


