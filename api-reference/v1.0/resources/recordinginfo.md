---
title: tipo de recurso recordingInfo
description: Representa informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7044f13f16a9d1126a5b1c72cdc86c3527f6b37
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543265"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="8f9f1-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="8f9f1-103">recordingInfo resource type</span></span>

<span data-ttu-id="8f9f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f9f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f9f1-105">Representa informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="8f9f1-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="8f9f1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f9f1-106">Properties</span></span>

| <span data-ttu-id="8f9f1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f9f1-107">Property</span></span>        | <span data-ttu-id="8f9f1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f9f1-108">Type</span></span>    | <span data-ttu-id="8f9f1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f9f1-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="8f9f1-110">Iniciador</span><span class="sxs-lookup"><span data-stu-id="8f9f1-110">initiator</span></span>     | [<span data-ttu-id="8f9f1-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="8f9f1-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="8f9f1-112">As identidades do iniciador de gravação.</span><span class="sxs-lookup"><span data-stu-id="8f9f1-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="8f9f1-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="8f9f1-113">recordingStatus</span></span> | <span data-ttu-id="8f9f1-114">String</span><span class="sxs-lookup"><span data-stu-id="8f9f1-114">String</span></span> | <span data-ttu-id="8f9f1-115">Os valores possíveis são `unknown`: `notRecording`, `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="8f9f1-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8f9f1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f9f1-116">JSON representation</span></span>

<span data-ttu-id="8f9f1-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f9f1-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiator": {"@odata.type": "#microsoft.graph.identitySet"},
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
