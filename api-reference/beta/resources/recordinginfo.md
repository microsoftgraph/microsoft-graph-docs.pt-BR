---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2da0dd44ca1dc7ffd8d6ee13b1289e75c87f7cd6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006561"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="30356-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="30356-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30356-104">Informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="30356-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="30356-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30356-105">Properties</span></span>

| <span data-ttu-id="30356-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30356-106">Property</span></span>       | <span data-ttu-id="30356-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="30356-107">Type</span></span>    | <span data-ttu-id="30356-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="30356-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="30356-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="30356-109">initiatedBy</span></span> | [<span data-ttu-id="30356-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="30356-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="30356-111">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="30356-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="30356-112">status</span><span class="sxs-lookup"><span data-stu-id="30356-112">status</span></span> | <span data-ttu-id="30356-113">String</span><span class="sxs-lookup"><span data-stu-id="30356-113">String</span></span> | <span data-ttu-id="30356-114">Os valores possíveis são: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="30356-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30356-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30356-115">JSON representation</span></span>

<span data-ttu-id="30356-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30356-116">The following is a JSON representation of the resource.</span></span>

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
