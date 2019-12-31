---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 30b3ef3b3acd4f1cdaa7c7a0b4c63b4d8104c09b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913384"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="7a3bf-103">tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="7a3bf-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a3bf-104">Informações sobre um participante de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="7a3bf-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="7a3bf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a3bf-105">Properties</span></span>

| <span data-ttu-id="7a3bf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a3bf-106">Property</span></span>       | <span data-ttu-id="7a3bf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a3bf-107">Type</span></span>                          | <span data-ttu-id="7a3bf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a3bf-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="7a3bf-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="7a3bf-109">identity</span></span>       | [<span data-ttu-id="7a3bf-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="7a3bf-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="7a3bf-111">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="7a3bf-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="7a3bf-112">UPN</span><span class="sxs-lookup"><span data-stu-id="7a3bf-112">upn</span></span>            | <span data-ttu-id="7a3bf-113">String</span><span class="sxs-lookup"><span data-stu-id="7a3bf-113">String</span></span>                        | <span data-ttu-id="7a3bf-114">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="7a3bf-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7a3bf-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a3bf-115">JSON representation</span></span>

<span data-ttu-id="7a3bf-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a3bf-116">The following is a JSON representation of the resource.</span></span>

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
