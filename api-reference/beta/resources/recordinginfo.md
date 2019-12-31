---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e924ea98bb0f9ac8e0b610a4672cbed83d83d0bc
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913440"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="b4381-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="b4381-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4381-104">Informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="b4381-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="b4381-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4381-105">Properties</span></span>

| <span data-ttu-id="b4381-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4381-106">Property</span></span>        | <span data-ttu-id="b4381-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4381-107">Type</span></span>    | <span data-ttu-id="b4381-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4381-108">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="b4381-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="b4381-109">initiatedBy</span></span>     | [<span data-ttu-id="b4381-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="b4381-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="b4381-111">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="b4381-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="b4381-112">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="b4381-112">recordingStatus</span></span> | <span data-ttu-id="b4381-113">String</span><span class="sxs-lookup"><span data-stu-id="b4381-113">String</span></span> | <span data-ttu-id="b4381-114">Os valores possíveis são `unknown`: `notRecording`, `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="b4381-114">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b4381-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4381-115">JSON representation</span></span>

<span data-ttu-id="b4381-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4381-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

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
