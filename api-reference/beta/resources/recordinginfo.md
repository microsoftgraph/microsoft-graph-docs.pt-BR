---
title: tipo de recurso de recordingInfo
description: Informações de gravação para um participante.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 85c2710452905f97235928bae71ff60c2d22983f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891935"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="94be3-103">tipo de recurso de recordingInfo</span><span class="sxs-lookup"><span data-stu-id="94be3-103">recordingInfo resource type</span></span>

> <span data-ttu-id="94be3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="94be3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94be3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94be3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94be3-106">Informações de gravação para um participante.</span><span class="sxs-lookup"><span data-stu-id="94be3-106">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="94be3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94be3-107">Properties</span></span>

| <span data-ttu-id="94be3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94be3-108">Property</span></span>       | <span data-ttu-id="94be3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="94be3-109">Type</span></span>    | <span data-ttu-id="94be3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94be3-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94be3-111">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="94be3-111">initiatedBy</span></span> | [<span data-ttu-id="94be3-112">participantInfo</span><span class="sxs-lookup"><span data-stu-id="94be3-112">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="94be3-113">O participante que iniciou a gravação.</span><span class="sxs-lookup"><span data-stu-id="94be3-113">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="94be3-114">status</span><span class="sxs-lookup"><span data-stu-id="94be3-114">status</span></span> | <span data-ttu-id="94be3-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94be3-115">String</span></span> | <span data-ttu-id="94be3-116">Os valores possíveis são: `recordingCapable`, `notRecording`, `startedRecording`.</span><span class="sxs-lookup"><span data-stu-id="94be3-116">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="94be3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94be3-117">JSON representation</span></span>

<span data-ttu-id="94be3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94be3-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
