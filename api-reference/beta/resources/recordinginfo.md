---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ebb9e7d6a5c62b12073d6fa26e76147eb0cbb137
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965478"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="658bf-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="658bf-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="658bf-104">Informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="658bf-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="658bf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="658bf-105">Properties</span></span>

| <span data-ttu-id="658bf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="658bf-106">Property</span></span>       | <span data-ttu-id="658bf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="658bf-107">Type</span></span>    | <span data-ttu-id="658bf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="658bf-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="658bf-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="658bf-109">initiatedBy</span></span> | [<span data-ttu-id="658bf-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="658bf-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="658bf-111">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="658bf-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="658bf-112">status</span><span class="sxs-lookup"><span data-stu-id="658bf-112">status</span></span> | <span data-ttu-id="658bf-113">String</span><span class="sxs-lookup"><span data-stu-id="658bf-113">String</span></span> | <span data-ttu-id="658bf-114">Os valores possíveis são: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="658bf-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="658bf-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="658bf-115">JSON representation</span></span>

<span data-ttu-id="658bf-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="658bf-116">The following is a JSON representation of the resource.</span></span>

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
