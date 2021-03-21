---
title: Tipo de recurso meetingCapability
description: Contém os recursos de uma reunião
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d8e1d3985f95ecc28bd986218d7ff668f65b1db8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960401"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="fc3b4-103">Tipo de recurso meetingCapability</span><span class="sxs-lookup"><span data-stu-id="fc3b4-103">meetingCapability resource type</span></span>

<span data-ttu-id="fc3b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc3b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc3b4-105">Contém os recursos de uma reunião</span><span class="sxs-lookup"><span data-stu-id="fc3b4-105">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="fc3b4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc3b4-106">Properties</span></span>

| <span data-ttu-id="fc3b4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc3b4-107">Property</span></span>                          | <span data-ttu-id="fc3b4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc3b4-108">Type</span></span>    | <span data-ttu-id="fc3b4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc3b4-109">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="fc3b4-110">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="fc3b4-110">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="fc3b4-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc3b4-111">Boolean</span></span> | <span data-ttu-id="fc3b4-112">Indica se o discagem de usuários anônimos é permitido em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="fc3b4-112">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="fc3b4-113">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="fc3b4-113">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="fc3b4-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc3b4-114">Boolean</span></span> | <span data-ttu-id="fc3b4-115">Indica se os usuários anônimos têm permissão para iniciar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="fc3b4-115">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="fc3b4-116">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="fc3b4-116">autoAdmittedUsers</span></span>                 | <span data-ttu-id="fc3b4-117">autoAdmittedUsersType</span><span class="sxs-lookup"><span data-stu-id="fc3b4-117">autoAdmittedUsersType</span></span>  | <span data-ttu-id="fc3b4-118">Os valores possíveis são: `everyoneInCompany` e `everyone`.</span><span class="sxs-lookup"><span data-stu-id="fc3b4-118">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="fc3b4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc3b4-119">JSON representation</span></span>

<span data-ttu-id="fc3b4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc3b4-120">The following is a JSON representation of the resource.</span></span>

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


