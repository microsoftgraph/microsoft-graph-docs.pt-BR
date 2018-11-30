---
title: tipo de recurso de recordOperation
description: O tipo de recordOperation
ms.openlocfilehash: 5863e5ef84b00c65cd0806af8a3364fe3d1ab73f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034492"
---
# <a name="recordoperation-resource-type"></a><span data-ttu-id="90e66-103">tipo de recurso de recordOperation</span><span class="sxs-lookup"><span data-stu-id="90e66-103">recordOperation resource type</span></span>

> <span data-ttu-id="90e66-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="90e66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90e66-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="90e66-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90e66-106">O tipo de recordOperation</span><span class="sxs-lookup"><span data-stu-id="90e66-106">The recordOperation type</span></span>

## <a name="properties"></a><span data-ttu-id="90e66-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90e66-107">Properties</span></span>

| <span data-ttu-id="90e66-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90e66-108">Property</span></span>                       | <span data-ttu-id="90e66-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="90e66-109">Type</span></span>                        | <span data-ttu-id="90e66-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="90e66-110">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="90e66-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="90e66-111">clientContext</span></span>                  | <span data-ttu-id="90e66-112">String</span><span class="sxs-lookup"><span data-stu-id="90e66-112">String</span></span>                      | <span data-ttu-id="90e66-113">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="90e66-113">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="90e66-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="90e66-114">completionReason</span></span>               | <span data-ttu-id="90e66-115">String</span><span class="sxs-lookup"><span data-stu-id="90e66-115">String</span></span>                      | <span data-ttu-id="90e66-116">Os valores possíveis são: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`.</span><span class="sxs-lookup"><span data-stu-id="90e66-116">Possible values are: `operationCanceled`, `stopToneDetected`, `maxRecordDurationReached`, `initialSilenceTimeout`, `maxSilenceTimeout`, `playPromptFailed`, `playBeepFailed`, `mediaReceiveTimeout`, `unspecifiedError`.</span></span> |
| <span data-ttu-id="90e66-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90e66-117">createdDateTime</span></span>                | <span data-ttu-id="90e66-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90e66-118">DateTimeOffset</span></span>              | <span data-ttu-id="90e66-119">A hora em que a gravação foi criada.</span><span class="sxs-lookup"><span data-stu-id="90e66-119">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="90e66-120">id</span><span class="sxs-lookup"><span data-stu-id="90e66-120">id</span></span>                             | <span data-ttu-id="90e66-121">String</span><span class="sxs-lookup"><span data-stu-id="90e66-121">String</span></span>                      | <span data-ttu-id="90e66-122">A identificação de operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90e66-122">The server operation id. Read-only.</span></span> <span data-ttu-id="90e66-123">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="90e66-123">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="90e66-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="90e66-124">lastActionDateTime</span></span>             | <span data-ttu-id="90e66-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90e66-125">DateTimeOffset</span></span>              | <span data-ttu-id="90e66-126">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="90e66-126">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="90e66-127">recordResourceLocation</span><span class="sxs-lookup"><span data-stu-id="90e66-127">recordResourceLocation</span></span>         | <span data-ttu-id="90e66-128">String</span><span class="sxs-lookup"><span data-stu-id="90e66-128">String</span></span>                      | <span data-ttu-id="90e66-129">O local onde a gravação está localizada.</span><span class="sxs-lookup"><span data-stu-id="90e66-129">The location where the recording is located.</span></span>                                                                                                      |
| <span data-ttu-id="90e66-130">recordResourceAccessToken</span><span class="sxs-lookup"><span data-stu-id="90e66-130">recordResourceAccessToken</span></span>      | <span data-ttu-id="90e66-131">String</span><span class="sxs-lookup"><span data-stu-id="90e66-131">String</span></span>                      | <span data-ttu-id="90e66-132">O token de acesso necessário para recuperar a gravação.</span><span class="sxs-lookup"><span data-stu-id="90e66-132">The access token required to retrieve the recording.</span></span>                                                                                              |
| <span data-ttu-id="90e66-133">resultInfo</span><span class="sxs-lookup"><span data-stu-id="90e66-133">resultInfo</span></span>                     | [<span data-ttu-id="90e66-134">resultInfo</span><span class="sxs-lookup"><span data-stu-id="90e66-134">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="90e66-135">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="90e66-135">The result information.</span></span>  <span data-ttu-id="90e66-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90e66-136">Read-only.</span></span> <span data-ttu-id="90e66-137">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="90e66-137">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="90e66-138">status</span><span class="sxs-lookup"><span data-stu-id="90e66-138">status</span></span>                         | <span data-ttu-id="90e66-139">String</span><span class="sxs-lookup"><span data-stu-id="90e66-139">String</span></span>                      | <span data-ttu-id="90e66-140">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="90e66-140">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="90e66-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90e66-141">Read-only.</span></span> <span data-ttu-id="90e66-142">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="90e66-142">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="90e66-143">Relações</span><span class="sxs-lookup"><span data-stu-id="90e66-143">Relationships</span></span>
<span data-ttu-id="90e66-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90e66-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90e66-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90e66-145">JSON representation</span></span>

<span data-ttu-id="90e66-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90e66-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "recordResourceLocation": "String",
  "recordResourceAccessToken": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="90e66-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90e66-147">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.recordOperation",
  "truncated": true
}-->
```json
{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceLocation": "https://resource.location/ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "recordResourceAccessToken": "<access-token>",
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
