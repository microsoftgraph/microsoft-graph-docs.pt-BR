---
title: tipo de recurso de participantes
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508143"
---
# <a name="participant-resource-type"></a><span data-ttu-id="ac0f0-103">tipo de recurso de participantes</span><span class="sxs-lookup"><span data-stu-id="ac0f0-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac0f0-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="ac0f0-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ac0f0-105">Methods</span></span>

| <span data-ttu-id="ac0f0-106">Método</span><span class="sxs-lookup"><span data-stu-id="ac0f0-106">Method</span></span>                                                          | <span data-ttu-id="ac0f0-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ac0f0-107">Return Type</span></span>                              | <span data-ttu-id="ac0f0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac0f0-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="ac0f0-109">Obtenha um participante</span><span class="sxs-lookup"><span data-stu-id="ac0f0-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="ac0f0-110">participante</span><span class="sxs-lookup"><span data-stu-id="ac0f0-110">participant</span></span>](participant.md)            | <span data-ttu-id="ac0f0-111">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="ac0f0-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="ac0f0-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="ac0f0-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="ac0f0-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="ac0f0-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="ac0f0-114">Configure o participante mixer de áudio.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="ac0f0-115">Convidar</span><span class="sxs-lookup"><span data-stu-id="ac0f0-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="ac0f0-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="ac0f0-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="ac0f0-117">Convide um participante à chamada.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="ac0f0-118">Ativar Mudo participante</span><span class="sxs-lookup"><span data-stu-id="ac0f0-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="ac0f0-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="ac0f0-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="ac0f0-120">Ativar Mudo de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="ac0f0-121">Ativar Mudo de todos os participantes</span><span class="sxs-lookup"><span data-stu-id="ac0f0-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="ac0f0-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="ac0f0-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="ac0f0-123">Ativar Mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="ac0f0-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac0f0-124">Properties</span></span>

| <span data-ttu-id="ac0f0-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac0f0-125">Property</span></span>             | <span data-ttu-id="ac0f0-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac0f0-126">Type</span></span>                                     | <span data-ttu-id="ac0f0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac0f0-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="ac0f0-128">id</span><span class="sxs-lookup"><span data-stu-id="ac0f0-128">id</span></span>                   | <span data-ttu-id="ac0f0-129">String</span><span class="sxs-lookup"><span data-stu-id="ac0f0-129">String</span></span>                                   | <span data-ttu-id="ac0f0-130">A identificação dos participantes.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-130">The participant id.</span></span>                                          |
| <span data-ttu-id="ac0f0-131">Info</span><span class="sxs-lookup"><span data-stu-id="ac0f0-131">info</span></span>                 | [<span data-ttu-id="ac0f0-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="ac0f0-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="ac0f0-133">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="ac0f0-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="ac0f0-134">isInLobby</span></span>            | <span data-ttu-id="ac0f0-135">booliano</span><span class="sxs-lookup"><span data-stu-id="ac0f0-135">boolean</span></span>                                  | <span data-ttu-id="ac0f0-136">True se o participante estiver no lobby</span><span class="sxs-lookup"><span data-stu-id="ac0f0-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="ac0f0-137">isMuted</span><span class="sxs-lookup"><span data-stu-id="ac0f0-137">isMuted</span></span>              | <span data-ttu-id="ac0f0-138">booliano</span><span class="sxs-lookup"><span data-stu-id="ac0f0-138">boolean</span></span>                                  | <span data-ttu-id="ac0f0-139">True se o participante está sem som (cliente ou servidor sem áudio)</span><span class="sxs-lookup"><span data-stu-id="ac0f0-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="ac0f0-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="ac0f0-140">mediaStreams</span></span>         | <span data-ttu-id="ac0f0-141">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="ac0f0-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="ac0f0-142">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="ac0f0-143">Metadata</span><span class="sxs-lookup"><span data-stu-id="ac0f0-143">metadata</span></span>             | <span data-ttu-id="ac0f0-144">String</span><span class="sxs-lookup"><span data-stu-id="ac0f0-144">String</span></span>                                   | <span data-ttu-id="ac0f0-145">Um blob de dados fornecidos pelo participante na lista</span><span class="sxs-lookup"><span data-stu-id="ac0f0-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="ac0f0-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="ac0f0-146">recordingInfo</span></span>        | [<span data-ttu-id="ac0f0-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="ac0f0-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="ac0f0-148">Informações sobre se o participante tenha o recurso de gravação.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ac0f0-149">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="ac0f0-149">Relationships</span></span>
<span data-ttu-id="ac0f0-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac0f0-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac0f0-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac0f0-151">JSON representation</span></span>

<span data-ttu-id="ac0f0-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac0f0-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
}
```

## <a name="example"></a><span data-ttu-id="ac0f0-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac0f0-153">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
