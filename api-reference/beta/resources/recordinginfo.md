---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9e9a17a9afb197333e677547f3fa5dca22df9b2
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39637042"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="7ba0f-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="7ba0f-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ba0f-104">Informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="7ba0f-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="7ba0f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ba0f-105">Properties</span></span>

| <span data-ttu-id="7ba0f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ba0f-106">Property</span></span>        | <span data-ttu-id="7ba0f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ba0f-107">Type</span></span>    | <span data-ttu-id="7ba0f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ba0f-108">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="7ba0f-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="7ba0f-109">initiatedBy</span></span>     | [<span data-ttu-id="7ba0f-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="7ba0f-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="7ba0f-111">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="7ba0f-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="7ba0f-112">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="7ba0f-112">recordingStatus</span></span> | <span data-ttu-id="7ba0f-113">String</span><span class="sxs-lookup"><span data-stu-id="7ba0f-113">String</span></span> | <span data-ttu-id="7ba0f-114">Os valores possíveis são `unknown`: `notRecording`, `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="7ba0f-114">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ba0f-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ba0f-115">JSON representation</span></span>

<span data-ttu-id="7ba0f-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ba0f-116">The following is a JSON representation of the resource.</span></span>

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
