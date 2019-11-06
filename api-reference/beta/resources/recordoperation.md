---
title: tipo de recurso recordOperation
description: O tipo recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 22b1fbd157b6b13d0b839a898440ee289aa2ec73
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006554"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="fd34a-103">tipo de recurso recordOperation</span><span class="sxs-lookup"><span data-stu-id="fd34a-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd34a-104">O tipo recordOperation</span><span class="sxs-lookup"><span data-stu-id="fd34a-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="fd34a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd34a-105">Properties</span></span>

| <span data-ttu-id="fd34a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd34a-106">Property</span></span>                       | <span data-ttu-id="fd34a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd34a-107">Type</span></span>                        | <span data-ttu-id="fd34a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd34a-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fd34a-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="fd34a-109">clientContext</span></span>                  | <span data-ttu-id="fd34a-110">String</span><span class="sxs-lookup"><span data-stu-id="fd34a-110">String</span></span>                      | <span data-ttu-id="fd34a-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="fd34a-111">Unique Client Context string.</span></span> <span data-ttu-id="fd34a-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="fd34a-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="fd34a-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="fd34a-113">completionReason</span></span>               | <span data-ttu-id="fd34a-114">String</span><span class="sxs-lookup"><span data-stu-id="fd34a-114">String</span></span>                      | <span data-ttu-id="fd34a-115">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="fd34a-115">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="fd34a-116">id</span><span class="sxs-lookup"><span data-stu-id="fd34a-116">id</span></span>                             | <span data-ttu-id="fd34a-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd34a-117">String</span></span>                      | <span data-ttu-id="fd34a-118">A ID da operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd34a-118">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="fd34a-119">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="fd34a-119">recordingAccessToken</span></span>           | <span data-ttu-id="fd34a-120">String</span><span class="sxs-lookup"><span data-stu-id="fd34a-120">String</span></span>                      | <span data-ttu-id="fd34a-121">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="fd34a-121">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="fd34a-122">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="fd34a-122">recordingLocation</span></span>              | <span data-ttu-id="fd34a-123">String</span><span class="sxs-lookup"><span data-stu-id="fd34a-123">String</span></span>                      | <span data-ttu-id="fd34a-124">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="fd34a-124">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="fd34a-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fd34a-125">resultInfo</span></span>                     | [<span data-ttu-id="fd34a-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="fd34a-126">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="fd34a-127">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="fd34a-127">The result information.</span></span>  <span data-ttu-id="fd34a-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd34a-128">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="fd34a-129">status</span><span class="sxs-lookup"><span data-stu-id="fd34a-129">status</span></span>                         | <span data-ttu-id="fd34a-130">String</span><span class="sxs-lookup"><span data-stu-id="fd34a-130">String</span></span>                      | <span data-ttu-id="fd34a-131">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="fd34a-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="fd34a-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd34a-132">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="fd34a-133">Relações</span><span class="sxs-lookup"><span data-stu-id="fd34a-133">Relationships</span></span>
<span data-ttu-id="fd34a-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd34a-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd34a-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd34a-135">JSON representation</span></span>

<span data-ttu-id="fd34a-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd34a-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
