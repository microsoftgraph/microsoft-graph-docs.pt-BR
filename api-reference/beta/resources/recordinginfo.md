---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 644ba7fbd762acde7f5229d15267de5352f03ca8
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268318"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="87275-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="87275-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87275-104">Informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="87275-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="87275-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87275-105">Properties</span></span>

| <span data-ttu-id="87275-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87275-106">Property</span></span>        | <span data-ttu-id="87275-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="87275-107">Type</span></span>    | <span data-ttu-id="87275-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="87275-108">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="87275-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="87275-109">initiatedBy</span></span>     | [<span data-ttu-id="87275-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="87275-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="87275-111">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="87275-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="87275-112">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="87275-112">recordingStatus</span></span> | <span data-ttu-id="87275-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87275-113">String</span></span> | <span data-ttu-id="87275-114">Os valores possíveis são `unknown`: `notRecording`, `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="87275-114">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |
| <span data-ttu-id="87275-115">Iniciador</span><span class="sxs-lookup"><span data-stu-id="87275-115">initiator</span></span> | [<span data-ttu-id="87275-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="87275-116">identitySet</span></span>](identitySet.md) | <span data-ttu-id="87275-117">As identidades do iniciador de gravação.</span><span class="sxs-lookup"><span data-stu-id="87275-117">The identities of recording initiator.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="87275-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87275-118">JSON representation</span></span>

<span data-ttu-id="87275-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87275-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed",
  "initiator": {"@odata.type": "#microsoft.graph.initiator"}
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
