---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 45d844329688e663c27ef5ecdf94282312baa53d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055169"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="c43bf-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="c43bf-103">recordingInfo resource type</span></span>

<span data-ttu-id="c43bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c43bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c43bf-105">Informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="c43bf-105">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="c43bf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c43bf-106">Properties</span></span>

| <span data-ttu-id="c43bf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c43bf-107">Property</span></span>        | <span data-ttu-id="c43bf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c43bf-108">Type</span></span>    | <span data-ttu-id="c43bf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c43bf-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="c43bf-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="c43bf-110">initiatedBy</span></span>     | [<span data-ttu-id="c43bf-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="c43bf-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="c43bf-112">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="c43bf-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="c43bf-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="c43bf-113">recordingStatus</span></span> | <span data-ttu-id="c43bf-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c43bf-114">String</span></span> | <span data-ttu-id="c43bf-115">Os valores possíveis são: `unknown` , `notRecording` , `recording` , ou `failed` .</span><span class="sxs-lookup"><span data-stu-id="c43bf-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |
| <span data-ttu-id="c43bf-116">Iniciador</span><span class="sxs-lookup"><span data-stu-id="c43bf-116">initiator</span></span> | [<span data-ttu-id="c43bf-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="c43bf-117">identitySet</span></span>](identitySet.md) | <span data-ttu-id="c43bf-118">As identidades do iniciador de gravação.</span><span class="sxs-lookup"><span data-stu-id="c43bf-118">The identities of recording initiator.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c43bf-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c43bf-119">JSON representation</span></span>

<span data-ttu-id="c43bf-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c43bf-120">The following is a JSON representation of the resource.</span></span>

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


