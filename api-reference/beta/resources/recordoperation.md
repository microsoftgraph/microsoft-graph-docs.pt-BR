---
title: tipo de recurso de recordOperation
description: O tipo de recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 914b8d819fdbcc132d4e04cd12f5c0db9980f659
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577183"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="13875-103">tipo de recurso de recordOperation</span><span class="sxs-lookup"><span data-stu-id="13875-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13875-104">O tipo de recordOperation</span><span class="sxs-lookup"><span data-stu-id="13875-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="13875-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13875-105">Properties</span></span>

| <span data-ttu-id="13875-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13875-106">Property</span></span>                       | <span data-ttu-id="13875-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="13875-107">Type</span></span>                        | <span data-ttu-id="13875-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="13875-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="13875-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="13875-109">clientContext</span></span>                  | <span data-ttu-id="13875-110">String</span><span class="sxs-lookup"><span data-stu-id="13875-110">String</span></span>                      | <span data-ttu-id="13875-111">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="13875-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="13875-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="13875-112">completionReason</span></span>               | <span data-ttu-id="13875-113">String</span><span class="sxs-lookup"><span data-stu-id="13875-113">String</span></span>                      | <span data-ttu-id="13875-114">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="13875-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="13875-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13875-115">createdDateTime</span></span>                | <span data-ttu-id="13875-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13875-116">DateTimeOffset</span></span>              | <span data-ttu-id="13875-117">A hora em que a gravação foi criada.</span><span class="sxs-lookup"><span data-stu-id="13875-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="13875-118">id</span><span class="sxs-lookup"><span data-stu-id="13875-118">id</span></span>                             | <span data-ttu-id="13875-119">String</span><span class="sxs-lookup"><span data-stu-id="13875-119">String</span></span>                      | <span data-ttu-id="13875-120">A identificação de operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13875-120">The server operation id. Read-only.</span></span> <span data-ttu-id="13875-121">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="13875-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="13875-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="13875-122">lastActionDateTime</span></span>             | <span data-ttu-id="13875-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13875-123">DateTimeOffset</span></span>              | <span data-ttu-id="13875-124">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="13875-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="13875-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="13875-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="13875-126">String</span><span class="sxs-lookup"><span data-stu-id="13875-126">String</span></span>                      | <span data-ttu-id="13875-127">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="13875-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="13875-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="13875-128">recordResourceLocation</span></span>         | <span data-ttu-id="13875-129">String</span><span class="sxs-lookup"><span data-stu-id="13875-129">String</span></span>                      | <span data-ttu-id="13875-130">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="13875-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="13875-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="13875-131">resultInfo</span></span>                     | [<span data-ttu-id="13875-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="13875-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="13875-133">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="13875-133">The result information.</span></span>  <span data-ttu-id="13875-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="13875-134">Read-only.</span></span> <span data-ttu-id="13875-135">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="13875-135">Server generated.</span></span>                                                                                             |

## <a name="relationships"></a><span data-ttu-id="13875-136">Relações</span><span class="sxs-lookup"><span data-stu-id="13875-136">Relationships</span></span>
<span data-ttu-id="13875-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13875-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13875-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13875-138">JSON representation</span></span>

<span data-ttu-id="13875-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13875-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "recordCompletionReason",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceAccessToken": "String",
  "recordResourceLocation": "String",
  "resultInfo": {"@odata.type": "microsoft.graph.resultInfo"}
}
```

## <a name="example"></a><span data-ttu-id="13875-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13875-140">Example</span></span>

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
