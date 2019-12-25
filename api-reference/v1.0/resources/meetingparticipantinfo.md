---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6f3b8bc4b373f28f8f35fe891f7498a0560c38b9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865655"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="9ffaf-103">tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="9ffaf-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="9ffaf-104">Informações sobre um participante de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-104">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="9ffaf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ffaf-105">Properties</span></span>

| <span data-ttu-id="9ffaf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ffaf-106">Property</span></span>       | <span data-ttu-id="9ffaf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ffaf-107">Type</span></span>                          | <span data-ttu-id="9ffaf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ffaf-108">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="9ffaf-109">ladrões</span><span class="sxs-lookup"><span data-stu-id="9ffaf-109">identity</span></span>       | [<span data-ttu-id="9ffaf-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="9ffaf-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="9ffaf-111">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-111">Identity information of the participant.</span></span> |
| <span data-ttu-id="9ffaf-112">UPN</span><span class="sxs-lookup"><span data-stu-id="9ffaf-112">upn</span></span>            | <span data-ttu-id="9ffaf-113">String</span><span class="sxs-lookup"><span data-stu-id="9ffaf-113">String</span></span>                        | <span data-ttu-id="9ffaf-114">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-114">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9ffaf-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ffaf-115">JSON representation</span></span>

<span data-ttu-id="9ffaf-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ffaf-116">The following is a JSON representation of the resource.</span></span>

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
