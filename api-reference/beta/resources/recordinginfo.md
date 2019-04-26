---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 17da055e1cf40922075ba06de3e229c669d2e40f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343926"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="1152e-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="1152e-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1152e-104">Informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="1152e-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="1152e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1152e-105">Properties</span></span>

| <span data-ttu-id="1152e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1152e-106">Property</span></span>       | <span data-ttu-id="1152e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1152e-107">Type</span></span>    | <span data-ttu-id="1152e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1152e-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1152e-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="1152e-109">initiatedBy</span></span> | [<span data-ttu-id="1152e-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="1152e-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="1152e-111">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="1152e-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="1152e-112">status</span><span class="sxs-lookup"><span data-stu-id="1152e-112">status</span></span> | <span data-ttu-id="1152e-113">String</span><span class="sxs-lookup"><span data-stu-id="1152e-113">String</span></span> | <span data-ttu-id="1152e-114">Os valores possíveis são: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="1152e-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1152e-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1152e-115">JSON representation</span></span>

<span data-ttu-id="1152e-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1152e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
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
