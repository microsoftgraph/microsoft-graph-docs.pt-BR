---
title: tipo de recurso de recordOperation
description: O tipo de recordOperation
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: be6a124fcd7175489679a8c2392218530d510e9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880014"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="4c2ff-103">tipo de recurso de recordOperation</span><span class="sxs-lookup"><span data-stu-id="4c2ff-103">recordOperation resource type</span></span>

> <span data-ttu-id="4c2ff-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c2ff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c2ff-106">O tipo de recordOperation</span><span class="sxs-lookup"><span data-stu-id="4c2ff-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="4c2ff-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c2ff-107">Properties</span></span>

| <span data-ttu-id="4c2ff-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c2ff-108">Property</span></span>                       | <span data-ttu-id="4c2ff-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c2ff-109">Type</span></span>                        | <span data-ttu-id="4c2ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c2ff-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4c2ff-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="4c2ff-111">clientContext</span></span>                  | <span data-ttu-id="4c2ff-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c2ff-112">String</span></span>                      | <span data-ttu-id="4c2ff-113">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="4c2ff-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="4c2ff-114">completionReason</span></span>               | <span data-ttu-id="4c2ff-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c2ff-115">String</span></span>                      | <span data-ttu-id="4c2ff-116">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`, `none`.</span></span> |
| <span data-ttu-id="4c2ff-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c2ff-117">createdDateTime</span></span>                | <span data-ttu-id="4c2ff-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c2ff-118">DateTimeOffset</span></span>              | <span data-ttu-id="4c2ff-119">A hora em que a gravação foi criada.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="4c2ff-120">id</span><span class="sxs-lookup"><span data-stu-id="4c2ff-120">id</span></span>                             | <span data-ttu-id="4c2ff-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c2ff-121">String</span></span>                      | <span data-ttu-id="4c2ff-122">A identificação de operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-122">The server operation id. Read-only.</span></span> <span data-ttu-id="4c2ff-123">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="4c2ff-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="4c2ff-124">lastActionDateTime</span></span>             | <span data-ttu-id="4c2ff-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c2ff-125">DateTimeOffset</span></span>              | <span data-ttu-id="4c2ff-126">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="4c2ff-127">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="4c2ff-127">recordResourceAccessToken</span></span>      | <span data-ttu-id="4c2ff-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c2ff-128">String</span></span>                      | <span data-ttu-id="4c2ff-129">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-129">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="4c2ff-130">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="4c2ff-130">recordResourceLocation</span></span>         | <span data-ttu-id="4c2ff-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c2ff-131">String</span></span>                      | <span data-ttu-id="4c2ff-132">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-132">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="4c2ff-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4c2ff-133">resultInfo</span></span>                     | [<span data-ttu-id="4c2ff-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="4c2ff-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="4c2ff-135">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-135">The result information.</span></span>  <span data-ttu-id="4c2ff-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-136">Read-only.</span></span> <span data-ttu-id="4c2ff-137">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="4c2ff-138">status</span><span class="sxs-lookup"><span data-stu-id="4c2ff-138">status</span></span>                         | <span data-ttu-id="4c2ff-139">String</span><span class="sxs-lookup"><span data-stu-id="4c2ff-139">String</span></span>                      | <span data-ttu-id="4c2ff-140">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="4c2ff-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-141">Read-only.</span></span> <span data-ttu-id="4c2ff-142">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="4c2ff-143">Relações</span><span class="sxs-lookup"><span data-stu-id="4c2ff-143">Relationships</span></span>
<span data-ttu-id="4c2ff-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c2ff-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c2ff-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c2ff-145">JSON representation</span></span>

<span data-ttu-id="4c2ff-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c2ff-146">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="4c2ff-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c2ff-147">Example</span></span>

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
