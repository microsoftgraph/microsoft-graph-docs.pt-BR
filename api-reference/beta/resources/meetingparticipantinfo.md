---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2775dd3af7940f9022b9e7090125ed52fce397d6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006631"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="80f6a-103">tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="80f6a-103">meetingParticipantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f6a-104">Informações sobre um participante de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="80f6a-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="80f6a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80f6a-105">Properties</span></span>

| <span data-ttu-id="80f6a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80f6a-106">Property</span></span>       | <span data-ttu-id="80f6a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="80f6a-107">Type</span></span>                          | <span data-ttu-id="80f6a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="80f6a-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="80f6a-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="80f6a-109">identity</span></span>       | [<span data-ttu-id="80f6a-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="80f6a-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="80f6a-111">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="80f6a-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="80f6a-112">UPN</span><span class="sxs-lookup"><span data-stu-id="80f6a-112">upn</span></span>            | <span data-ttu-id="80f6a-113">String</span><span class="sxs-lookup"><span data-stu-id="80f6a-113">String</span></span>                        | <span data-ttu-id="80f6a-114">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="80f6a-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="80f6a-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80f6a-115">JSON representation</span></span>

<span data-ttu-id="80f6a-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80f6a-116">The following is a JSON representation of the resource.</span></span>

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
