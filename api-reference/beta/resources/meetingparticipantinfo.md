---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3df338760bd1d2ff74cc79c706944c9b5fa7104d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342391"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="54e96-103">tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="54e96-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54e96-104">Informações sobre um participante de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="54e96-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="54e96-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54e96-105">Properties</span></span>

| <span data-ttu-id="54e96-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54e96-106">Property</span></span>       | <span data-ttu-id="54e96-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="54e96-107">Type</span></span>                          | <span data-ttu-id="54e96-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="54e96-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="54e96-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="54e96-109">identity</span></span>       | [<span data-ttu-id="54e96-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="54e96-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="54e96-111">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="54e96-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="54e96-112">UPN</span><span class="sxs-lookup"><span data-stu-id="54e96-112">upn</span></span>            | <span data-ttu-id="54e96-113">String</span><span class="sxs-lookup"><span data-stu-id="54e96-113">String</span></span>                        | <span data-ttu-id="54e96-114">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="54e96-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="54e96-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54e96-115">JSON representation</span></span>

<span data-ttu-id="54e96-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54e96-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
