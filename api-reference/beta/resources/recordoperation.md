---
title: tipo de recurso recordOperation
description: Contém informações relacionadas à gravação de áudio.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ccf7f4b196866ccc8f038047a29f4b3dabd96642
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055152"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="a3002-103">tipo de recurso recordOperation</span><span class="sxs-lookup"><span data-stu-id="a3002-103">recordOperation resource type</span></span>

<span data-ttu-id="a3002-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3002-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3002-105">Contém informações relacionadas à gravação de áudio.</span><span class="sxs-lookup"><span data-stu-id="a3002-105">Contains information related to audio recording.</span></span>

## <a name="properties"></a><span data-ttu-id="a3002-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3002-106">Properties</span></span>

| <span data-ttu-id="a3002-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3002-107">Property</span></span>                       | <span data-ttu-id="a3002-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3002-108">Type</span></span>                        | <span data-ttu-id="a3002-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3002-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a3002-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="a3002-110">clientContext</span></span>                  | <span data-ttu-id="a3002-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3002-111">String</span></span>                      | <span data-ttu-id="a3002-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="a3002-112">Unique Client Context string.</span></span> <span data-ttu-id="a3002-113">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a3002-113">Max limit is 256 chars.</span></span>                                                                                                                               |
| <span data-ttu-id="a3002-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="a3002-114">completionReason</span></span>               | <span data-ttu-id="a3002-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3002-115">String</span></span>                      | <span data-ttu-id="a3002-116">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="a3002-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="a3002-117">id</span><span class="sxs-lookup"><span data-stu-id="a3002-117">id</span></span>                             | <span data-ttu-id="a3002-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3002-118">String</span></span>                      | <span data-ttu-id="a3002-119">A ID da operação do servidor.</span><span class="sxs-lookup"><span data-stu-id="a3002-119">The server operation ID.</span></span> <span data-ttu-id="a3002-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3002-120">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="a3002-121">recordingAccessToken</span><span class="sxs-lookup"><span data-stu-id="a3002-121">recordingAccessToken</span></span>           | <span data-ttu-id="a3002-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3002-122">String</span></span>                      | <span data-ttu-id="a3002-123">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="a3002-123">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="a3002-124">recordingLocation</span><span class="sxs-lookup"><span data-stu-id="a3002-124">recordingLocation</span></span>              | <span data-ttu-id="a3002-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3002-125">String</span></span>                      | <span data-ttu-id="a3002-126">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="a3002-126">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="a3002-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a3002-127">resultInfo</span></span>                     | [<span data-ttu-id="a3002-128">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a3002-128">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="a3002-129">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="a3002-129">The result information.</span></span>  <span data-ttu-id="a3002-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3002-130">Read-only.</span></span>                                                                                              |
| <span data-ttu-id="a3002-131">status</span><span class="sxs-lookup"><span data-stu-id="a3002-131">status</span></span>                         | <span data-ttu-id="a3002-132">String</span><span class="sxs-lookup"><span data-stu-id="a3002-132">String</span></span>                      | <span data-ttu-id="a3002-133">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a3002-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="a3002-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3002-134">Read-only.</span></span>                                                |

## <a name="relationships"></a><span data-ttu-id="a3002-135">Relações</span><span class="sxs-lookup"><span data-stu-id="a3002-135">Relationships</span></span>
<span data-ttu-id="a3002-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3002-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3002-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3002-137">JSON representation</span></span>

<span data-ttu-id="a3002-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3002-138">The following is a JSON representation of the resource.</span></span>

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


