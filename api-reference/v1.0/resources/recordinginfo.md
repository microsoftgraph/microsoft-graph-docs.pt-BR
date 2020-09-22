---
title: tipo de recurso recordingInfo
description: Representa informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd640e3ddef6b88f17449c31611ad6bd956ca0b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078973"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="54370-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="54370-103">recordingInfo resource type</span></span>

<span data-ttu-id="54370-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54370-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54370-105">Representa informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="54370-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="54370-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54370-106">Properties</span></span>

| <span data-ttu-id="54370-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54370-107">Property</span></span>        | <span data-ttu-id="54370-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="54370-108">Type</span></span>    | <span data-ttu-id="54370-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="54370-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="54370-110">Iniciador</span><span class="sxs-lookup"><span data-stu-id="54370-110">initiator</span></span>     | [<span data-ttu-id="54370-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="54370-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="54370-112">As identidades do iniciador de gravação.</span><span class="sxs-lookup"><span data-stu-id="54370-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="54370-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="54370-113">recordingStatus</span></span> | <span data-ttu-id="54370-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54370-114">String</span></span> | <span data-ttu-id="54370-115">Os valores possíveis são: `unknown` , `notRecording` , `recording` , ou `failed` .</span><span class="sxs-lookup"><span data-stu-id="54370-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54370-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54370-116">JSON representation</span></span>

<span data-ttu-id="54370-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54370-117">The following is a JSON representation of the resource.</span></span>

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

