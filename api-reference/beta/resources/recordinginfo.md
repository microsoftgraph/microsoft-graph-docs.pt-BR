---
title: tipo de recurso de recordingInfo
description: Informações de gravação para um participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6025259bafdcff78c3c7dbfa19aa39f5f6648f84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525672"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="9ac73-103">tipo de recurso de recordingInfo</span><span class="sxs-lookup"><span data-stu-id="9ac73-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ac73-104">Informações de gravação para um participante.</span><span class="sxs-lookup"><span data-stu-id="9ac73-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="9ac73-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ac73-105">Properties</span></span>

| <span data-ttu-id="9ac73-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ac73-106">Property</span></span>       | <span data-ttu-id="9ac73-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ac73-107">Type</span></span>    | <span data-ttu-id="9ac73-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ac73-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9ac73-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="9ac73-109">initiatedBy</span></span> | [<span data-ttu-id="9ac73-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="9ac73-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="9ac73-111">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="9ac73-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="9ac73-112">status</span><span class="sxs-lookup"><span data-stu-id="9ac73-112">status</span></span> | <span data-ttu-id="9ac73-113">String</span><span class="sxs-lookup"><span data-stu-id="9ac73-113">String</span></span> | <span data-ttu-id="9ac73-114">Os valores possíveis são: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="9ac73-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9ac73-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ac73-115">JSON representation</span></span>

<span data-ttu-id="9ac73-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ac73-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/recordinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
