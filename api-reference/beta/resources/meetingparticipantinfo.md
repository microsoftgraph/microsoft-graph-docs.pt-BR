---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a4c9e350d75783208a14310605540ab110f64f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971661"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="f20e2-103">tipo de recurso meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="f20e2-103">meetingParticipantInfo resource type</span></span>

<span data-ttu-id="f20e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f20e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f20e2-105">Informações sobre um participante de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="f20e2-105">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="f20e2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f20e2-106">Properties</span></span>

| <span data-ttu-id="f20e2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f20e2-107">Property</span></span>       | <span data-ttu-id="f20e2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f20e2-108">Type</span></span>                          | <span data-ttu-id="f20e2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f20e2-109">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="f20e2-110">ladrões</span><span class="sxs-lookup"><span data-stu-id="f20e2-110">identity</span></span>       | [<span data-ttu-id="f20e2-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="f20e2-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="f20e2-112">Informações de identidade do participante.</span><span class="sxs-lookup"><span data-stu-id="f20e2-112">Identity information of the participant.</span></span> |
| <span data-ttu-id="f20e2-113">UPN</span><span class="sxs-lookup"><span data-stu-id="f20e2-113">upn</span></span>            | <span data-ttu-id="f20e2-114">String</span><span class="sxs-lookup"><span data-stu-id="f20e2-114">String</span></span>                        | <span data-ttu-id="f20e2-115">Nome principal do usuário do participante.</span><span class="sxs-lookup"><span data-stu-id="f20e2-115">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f20e2-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f20e2-116">JSON representation</span></span>

<span data-ttu-id="f20e2-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f20e2-117">The following is a JSON representation of the resource.</span></span>

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


