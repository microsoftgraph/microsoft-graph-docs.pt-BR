---
title: tipo de recurso de recordOperation
description: O tipo de recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6b9deb566e5b527a9f20db69441fa96908212a38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512504"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="cbf09-103">tipo de recurso de recordOperation</span><span class="sxs-lookup"><span data-stu-id="cbf09-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbf09-104">O tipo de recordOperation</span><span class="sxs-lookup"><span data-stu-id="cbf09-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="cbf09-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbf09-105">Properties</span></span>

| <span data-ttu-id="cbf09-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbf09-106">Property</span></span>                       | <span data-ttu-id="cbf09-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbf09-107">Type</span></span>                        | <span data-ttu-id="cbf09-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbf09-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cbf09-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="cbf09-109">clientContext</span></span>                  | <span data-ttu-id="cbf09-110">String</span><span class="sxs-lookup"><span data-stu-id="cbf09-110">String</span></span>                      | <span data-ttu-id="cbf09-111">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="cbf09-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="cbf09-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="cbf09-112">completionReason</span></span>               | <span data-ttu-id="cbf09-113">String</span><span class="sxs-lookup"><span data-stu-id="cbf09-113">String</span></span>                      | <span data-ttu-id="cbf09-114">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="cbf09-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="cbf09-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbf09-115">createdDateTime</span></span>                | <span data-ttu-id="cbf09-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbf09-116">DateTimeOffset</span></span>              | <span data-ttu-id="cbf09-117">A hora em que a gravação foi criada.</span><span class="sxs-lookup"><span data-stu-id="cbf09-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="cbf09-118">id</span><span class="sxs-lookup"><span data-stu-id="cbf09-118">id</span></span>                             | <span data-ttu-id="cbf09-119">String</span><span class="sxs-lookup"><span data-stu-id="cbf09-119">String</span></span>                      | <span data-ttu-id="cbf09-120">A identificação de operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cbf09-120">The server operation id. Read-only.</span></span> <span data-ttu-id="cbf09-121">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="cbf09-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="cbf09-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="cbf09-122">lastActionDateTime</span></span>             | <span data-ttu-id="cbf09-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbf09-123">DateTimeOffset</span></span>              | <span data-ttu-id="cbf09-124">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="cbf09-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="cbf09-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="cbf09-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="cbf09-126">String</span><span class="sxs-lookup"><span data-stu-id="cbf09-126">String</span></span>                      | <span data-ttu-id="cbf09-127">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="cbf09-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="cbf09-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="cbf09-128">recordResourceLocation</span></span>         | <span data-ttu-id="cbf09-129">String</span><span class="sxs-lookup"><span data-stu-id="cbf09-129">String</span></span>                      | <span data-ttu-id="cbf09-130">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="cbf09-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="cbf09-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cbf09-131">resultInfo</span></span>                     | [<span data-ttu-id="cbf09-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cbf09-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="cbf09-133">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="cbf09-133">The result information.</span></span>  <span data-ttu-id="cbf09-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cbf09-134">Read-only.</span></span> <span data-ttu-id="cbf09-135">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="cbf09-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="cbf09-136">status</span><span class="sxs-lookup"><span data-stu-id="cbf09-136">status</span></span>                         | <span data-ttu-id="cbf09-137">String</span><span class="sxs-lookup"><span data-stu-id="cbf09-137">String</span></span>                      | <span data-ttu-id="cbf09-138">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="cbf09-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="cbf09-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cbf09-139">Read-only.</span></span> <span data-ttu-id="cbf09-140">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="cbf09-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="cbf09-141">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="cbf09-141">Relationships</span></span>
<span data-ttu-id="cbf09-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbf09-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbf09-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbf09-143">JSON representation</span></span>

<span data-ttu-id="cbf09-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbf09-144">The following is a JSON representation of the resource.</span></span>

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
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="cbf09-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbf09-145">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "status": "completed"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/recordoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
