---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 62ce735d5719ef05c5f96de546adcd5518a72786
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521226"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="851e1-103">tipo de recurso recordingInfo</span><span class="sxs-lookup"><span data-stu-id="851e1-103">recordingInfo resource type</span></span>

<span data-ttu-id="851e1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="851e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="851e1-105">Informações de gravação de um participante.</span><span class="sxs-lookup"><span data-stu-id="851e1-105">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="851e1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="851e1-106">Properties</span></span>

| <span data-ttu-id="851e1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="851e1-107">Property</span></span>        | <span data-ttu-id="851e1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="851e1-108">Type</span></span>    | <span data-ttu-id="851e1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="851e1-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="851e1-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="851e1-110">initiatedBy</span></span>     | [<span data-ttu-id="851e1-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="851e1-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="851e1-112">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="851e1-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="851e1-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="851e1-113">recordingStatus</span></span> | <span data-ttu-id="851e1-114">String</span><span class="sxs-lookup"><span data-stu-id="851e1-114">String</span></span> | <span data-ttu-id="851e1-115">Os valores possíveis são `unknown`: `notRecording`, `recording`,, `failed`ou.</span><span class="sxs-lookup"><span data-stu-id="851e1-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |
| <span data-ttu-id="851e1-116">Iniciador</span><span class="sxs-lookup"><span data-stu-id="851e1-116">initiator</span></span> | [<span data-ttu-id="851e1-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="851e1-117">identitySet</span></span>](identitySet.md) | <span data-ttu-id="851e1-118">As identidades do iniciador de gravação.</span><span class="sxs-lookup"><span data-stu-id="851e1-118">The identities of recording initiator.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="851e1-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="851e1-119">JSON representation</span></span>

<span data-ttu-id="851e1-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="851e1-120">The following is a JSON representation of the resource.</span></span>

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
