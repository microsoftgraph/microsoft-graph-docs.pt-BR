---
title: tipo de recurso recordOperation
description: O tipo recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 00b05cd86eeb9cf8be26cdc09fb8a9b254b510db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008800"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="d1637-103">tipo de recurso recordOperation</span><span class="sxs-lookup"><span data-stu-id="d1637-103">recordOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1637-104">O tipo recordOperation</span><span class="sxs-lookup"><span data-stu-id="d1637-104">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="d1637-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1637-105">Properties</span></span>

| <span data-ttu-id="d1637-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1637-106">Property</span></span>                       | <span data-ttu-id="d1637-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1637-107">Type</span></span>                        | <span data-ttu-id="d1637-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1637-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d1637-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="d1637-109">clientContext</span></span>                  | <span data-ttu-id="d1637-110">String</span><span class="sxs-lookup"><span data-stu-id="d1637-110">String</span></span>                      | <span data-ttu-id="d1637-111">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="d1637-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="d1637-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="d1637-112">completionReason</span></span>               | <span data-ttu-id="d1637-113">String</span><span class="sxs-lookup"><span data-stu-id="d1637-113">String</span></span>                      | <span data-ttu-id="d1637-114">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="d1637-114">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="d1637-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1637-115">createdDateTime</span></span>                | <span data-ttu-id="d1637-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1637-116">DateTimeOffset</span></span>              | <span data-ttu-id="d1637-117">A hora em que a gravação foi criada.</span><span class="sxs-lookup"><span data-stu-id="d1637-117">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="d1637-118">id</span><span class="sxs-lookup"><span data-stu-id="d1637-118">id</span></span>                             | <span data-ttu-id="d1637-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1637-119">String</span></span>                      | <span data-ttu-id="d1637-120">A ID da operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1637-120">The server operation id. Read-only.</span></span> <span data-ttu-id="d1637-121">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="d1637-121">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="d1637-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d1637-122">lastActionDateTime</span></span>             | <span data-ttu-id="d1637-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1637-123">DateTimeOffset</span></span>              | <span data-ttu-id="d1637-124">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="d1637-124">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="d1637-125">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="d1637-125">recordResourceAccessToken</span></span>      | <span data-ttu-id="d1637-126">String</span><span class="sxs-lookup"><span data-stu-id="d1637-126">String</span></span>                      | <span data-ttu-id="d1637-127">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="d1637-127">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="d1637-128">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="d1637-128">recordResourceLocation</span></span>         | <span data-ttu-id="d1637-129">String</span><span class="sxs-lookup"><span data-stu-id="d1637-129">String</span></span>                      | <span data-ttu-id="d1637-130">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="d1637-130">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="d1637-131">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d1637-131">resultInfo</span></span>                     | [<span data-ttu-id="d1637-132">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d1637-132">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d1637-133">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="d1637-133">The result information.</span></span>  <span data-ttu-id="d1637-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1637-134">Read-only.</span></span> <span data-ttu-id="d1637-135">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="d1637-135">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="d1637-136">status</span><span class="sxs-lookup"><span data-stu-id="d1637-136">status</span></span>                         | <span data-ttu-id="d1637-137">String</span><span class="sxs-lookup"><span data-stu-id="d1637-137">String</span></span>                      | <span data-ttu-id="d1637-138">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d1637-138">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d1637-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1637-139">Read-only.</span></span> <span data-ttu-id="d1637-140">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="d1637-140">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="d1637-141">Relações</span><span class="sxs-lookup"><span data-stu-id="d1637-141">Relationships</span></span>
<span data-ttu-id="d1637-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1637-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1637-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1637-143">JSON representation</span></span>

<span data-ttu-id="d1637-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1637-144">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="d1637-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1637-145">Example</span></span>

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
  "suppressions": []
}
-->
