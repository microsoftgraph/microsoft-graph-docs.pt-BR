---
title: tipo de recurso recordOperation
description: Contém informações relacionadas à gravação de áudio.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aece896ffba60ca6b42a05569406a0646748039d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912941"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="551cd-103">tipo de recurso recordOperation</span><span class="sxs-lookup"><span data-stu-id="551cd-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="551cd-104">Contém informações relacionadas à gravação de áudio.</span><span class="sxs-lookup"><span data-stu-id="551cd-104">Contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="551cd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="551cd-105">Properties</span></span>

| <span data-ttu-id="551cd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="551cd-106">Property</span></span>                       | <span data-ttu-id="551cd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="551cd-107">Type</span></span>                        | <span data-ttu-id="551cd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="551cd-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="551cd-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="551cd-109">clientContext</span></span>                  | <span data-ttu-id="551cd-110">String</span><span class="sxs-lookup"><span data-stu-id="551cd-110">String</span></span>                      | <span data-ttu-id="551cd-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="551cd-111">Unique Client Context string.</span></span> <span data-ttu-id="551cd-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="551cd-112">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="551cd-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="551cd-113">completionReason</span></span>               | <span data-ttu-id="551cd-114">String</span><span class="sxs-lookup"><span data-stu-id="551cd-114">String</span></span>                      | <span data-ttu-id="551cd-115">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="551cd-115">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="551cd-116">id</span><span class="sxs-lookup"><span data-stu-id="551cd-116">id</span></span>                             | <span data-ttu-id="551cd-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="551cd-117">String</span></span>                      | <span data-ttu-id="551cd-118">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="551cd-118">The server operation ID.</span></span> <span data-ttu-id="551cd-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="551cd-119">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="551cd-120">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="551cd-120">recordingAccessToken</span></span>           | <span data-ttu-id="551cd-121">String</span><span class="sxs-lookup"><span data-stu-id="551cd-121">String</span></span>                      | <span data-ttu-id="551cd-122">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="551cd-122">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="551cd-123">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="551cd-123">recordingLocation</span></span>              | <span data-ttu-id="551cd-124">String</span><span class="sxs-lookup"><span data-stu-id="551cd-124">String</span></span>                      | <span data-ttu-id="551cd-125">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="551cd-125">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="551cd-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="551cd-126">resultInfo</span></span>                     | [<span data-ttu-id="551cd-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="551cd-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="551cd-128">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="551cd-128">The result information.</span></span>  <span data-ttu-id="551cd-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="551cd-129">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="551cd-130">status</span><span class="sxs-lookup"><span data-stu-id="551cd-130">status</span></span>                         | <span data-ttu-id="551cd-131">String</span><span class="sxs-lookup"><span data-stu-id="551cd-131">String</span></span>                      | <span data-ttu-id="551cd-132">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="551cd-132">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="551cd-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="551cd-133">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="551cd-134">Relações</span><span class="sxs-lookup"><span data-stu-id="551cd-134">Relationships</span></span>
<span data-ttu-id="551cd-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="551cd-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="551cd-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="551cd-136">JSON representation</span></span>

<span data-ttu-id="551cd-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="551cd-137">The following is a JSON representation of the resource.</span></span>

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
