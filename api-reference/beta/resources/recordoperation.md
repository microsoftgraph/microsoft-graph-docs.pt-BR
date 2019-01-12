---
title: tipo de recurso de recordOperation
description: O tipo de recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2fdf8b6f1f00429e676d778c0095d4554fff4a18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948741"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="e796c-103">tipo de recurso de recordOperation</span><span class="sxs-lookup"><span data-stu-id="e796c-103">recordOperation resource type</span></span>

> <span data-ttu-id="e796c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e796c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e796c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e796c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e796c-106">O tipo de recordOperation</span><span class="sxs-lookup"><span data-stu-id="e796c-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="e796c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e796c-107">Properties</span></span>

| <span data-ttu-id="e796c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e796c-108">Property</span></span>                       | <span data-ttu-id="e796c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e796c-109">Type</span></span>                        | <span data-ttu-id="e796c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e796c-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e796c-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="e796c-111">clientContext</span></span>                  | <span data-ttu-id="e796c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e796c-112">String</span></span>                      | <span data-ttu-id="e796c-113">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="e796c-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="e796c-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="e796c-114">completionReason</span></span>               | <span data-ttu-id="e796c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e796c-115">String</span></span>                      | <span data-ttu-id="e796c-116">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e796c-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="e796c-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e796c-117">createdDateTime</span></span>                | <span data-ttu-id="e796c-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e796c-118">DateTimeOffset</span></span>              | <span data-ttu-id="e796c-119">A hora em que a gravação foi criada.</span><span class="sxs-lookup"><span data-stu-id="e796c-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="e796c-120">id</span><span class="sxs-lookup"><span data-stu-id="e796c-120">id</span></span>                             | <span data-ttu-id="e796c-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e796c-121">String</span></span>                      | <span data-ttu-id="e796c-122">A identificação de operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e796c-122">The server operation id. Read-only.</span></span> <span data-ttu-id="e796c-123">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="e796c-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="e796c-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="e796c-124">lastActionDateTime</span></span>             | <span data-ttu-id="e796c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e796c-125">DateTimeOffset</span></span>              | <span data-ttu-id="e796c-126">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="e796c-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="e796c-127">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="e796c-127">recordResourceAccessToken</span></span>      | <span data-ttu-id="e796c-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e796c-128">String</span></span>                      | <span data-ttu-id="e796c-129">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="e796c-129">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="e796c-130">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="e796c-130">recordResourceLocation</span></span>         | <span data-ttu-id="e796c-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e796c-131">String</span></span>                      | <span data-ttu-id="e796c-132">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="e796c-132">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="e796c-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e796c-133">resultInfo</span></span>                     | [<span data-ttu-id="e796c-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e796c-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="e796c-135">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="e796c-135">The result information.</span></span>  <span data-ttu-id="e796c-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e796c-136">Read-only.</span></span> <span data-ttu-id="e796c-137">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="e796c-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="e796c-138">status</span><span class="sxs-lookup"><span data-stu-id="e796c-138">status</span></span>                         | <span data-ttu-id="e796c-139">String</span><span class="sxs-lookup"><span data-stu-id="e796c-139">String</span></span>                      | <span data-ttu-id="e796c-140">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e796c-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="e796c-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e796c-141">Read-only.</span></span> <span data-ttu-id="e796c-142">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="e796c-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="e796c-143">Relações</span><span class="sxs-lookup"><span data-stu-id="e796c-143">Relationships</span></span>
<span data-ttu-id="e796c-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e796c-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e796c-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e796c-145">JSON representation</span></span>

<span data-ttu-id="e796c-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e796c-146">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e796c-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e796c-147">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
