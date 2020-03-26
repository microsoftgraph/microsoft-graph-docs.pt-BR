---
title: tipo de recurso recordingInfo
description: Representa informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6a41195705a46ac46bd085f3b4a655943b730ad3
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962526"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="fee5f-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="fee5f-103">recordingInfo resource type</span></span>

<span data-ttu-id="fee5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fee5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fee5f-105">Representa informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="fee5f-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="fee5f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fee5f-106">Properties</span></span>

| <span data-ttu-id="fee5f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fee5f-107">Property</span></span>        | <span data-ttu-id="fee5f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fee5f-108">Type</span></span>    | <span data-ttu-id="fee5f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee5f-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="fee5f-110">Iniciador</span><span class="sxs-lookup"><span data-stu-id="fee5f-110">initiator</span></span>     | [<span data-ttu-id="fee5f-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="fee5f-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="fee5f-112">As identidades do iniciador de gravação.</span><span class="sxs-lookup"><span data-stu-id="fee5f-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="fee5f-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="fee5f-113">recordingStatus</span></span> | <span data-ttu-id="fee5f-114">String</span><span class="sxs-lookup"><span data-stu-id="fee5f-114">String</span></span> | <span data-ttu-id="fee5f-115">Os valores possíveis são `unknown`: `notRecording`, `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="fee5f-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fee5f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fee5f-116">JSON representation</span></span>

<span data-ttu-id="fee5f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fee5f-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
