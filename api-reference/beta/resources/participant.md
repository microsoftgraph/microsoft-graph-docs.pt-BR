---
title: tipo de recurso participante
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568608"
---
# <a name="participant-resource-type"></a><span data-ttu-id="a2ff6-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="a2ff6-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2ff6-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="a2ff6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="a2ff6-105">Methods</span></span>

| <span data-ttu-id="a2ff6-106">Método</span><span class="sxs-lookup"><span data-stu-id="a2ff6-106">Method</span></span>                                                          | <span data-ttu-id="a2ff6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2ff6-107">Return Type</span></span>                              | <span data-ttu-id="a2ff6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ff6-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="a2ff6-109">Obter participante</span><span class="sxs-lookup"><span data-stu-id="a2ff6-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="a2ff6-110">participante</span><span class="sxs-lookup"><span data-stu-id="a2ff6-110">participant</span></span>](participant.md)            | <span data-ttu-id="a2ff6-111">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="a2ff6-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="a2ff6-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="a2ff6-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="a2ff6-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="a2ff6-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="a2ff6-114">Configure o mixer de áudio do participante.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="a2ff6-115">Convidar</span><span class="sxs-lookup"><span data-stu-id="a2ff6-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="a2ff6-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="a2ff6-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="a2ff6-117">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="a2ff6-118">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="a2ff6-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="a2ff6-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="a2ff6-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="a2ff6-120">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="a2ff6-121">Ativar mudo em todos os participantes</span><span class="sxs-lookup"><span data-stu-id="a2ff6-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="a2ff6-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="a2ff6-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="a2ff6-123">Ativar mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="a2ff6-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2ff6-124">Properties</span></span>

| <span data-ttu-id="a2ff6-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2ff6-125">Property</span></span>             | <span data-ttu-id="a2ff6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2ff6-126">Type</span></span>                                     | <span data-ttu-id="a2ff6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ff6-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="a2ff6-128">id</span><span class="sxs-lookup"><span data-stu-id="a2ff6-128">id</span></span>                   | <span data-ttu-id="a2ff6-129">String</span><span class="sxs-lookup"><span data-stu-id="a2ff6-129">String</span></span>                                   | <span data-ttu-id="a2ff6-130">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-130">The participant id.</span></span>                                          |
| <span data-ttu-id="a2ff6-131">informações </span><span class="sxs-lookup"><span data-stu-id="a2ff6-131">info</span></span>                 | [<span data-ttu-id="a2ff6-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="a2ff6-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="a2ff6-133">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="a2ff6-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="a2ff6-134">isInLobby</span></span>            | <span data-ttu-id="a2ff6-135">booliano</span><span class="sxs-lookup"><span data-stu-id="a2ff6-135">boolean</span></span>                                  | <span data-ttu-id="a2ff6-136">true se o participante está no lobby</span><span class="sxs-lookup"><span data-stu-id="a2ff6-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="a2ff6-137">IsMuted</span><span class="sxs-lookup"><span data-stu-id="a2ff6-137">isMuted</span></span>              | <span data-ttu-id="a2ff6-138">booliano</span><span class="sxs-lookup"><span data-stu-id="a2ff6-138">boolean</span></span>                                  | <span data-ttu-id="a2ff6-139">true se o participante estiver mudo (cliente ou servidor sem som)</span><span class="sxs-lookup"><span data-stu-id="a2ff6-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="a2ff6-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="a2ff6-140">mediaStreams</span></span>         | <span data-ttu-id="a2ff6-141">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="a2ff6-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="a2ff6-142">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="a2ff6-143">los</span><span class="sxs-lookup"><span data-stu-id="a2ff6-143">metadata</span></span>             | <span data-ttu-id="a2ff6-144">String</span><span class="sxs-lookup"><span data-stu-id="a2ff6-144">String</span></span>                                   | <span data-ttu-id="a2ff6-145">Um blob de dados fornecido pelo participante na lista</span><span class="sxs-lookup"><span data-stu-id="a2ff6-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="a2ff6-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="a2ff6-146">recordingInfo</span></span>        | [<span data-ttu-id="a2ff6-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="a2ff6-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="a2ff6-148">Informações sobre o fato de o participante ter capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a2ff6-149">Relações</span><span class="sxs-lookup"><span data-stu-id="a2ff6-149">Relationships</span></span>
<span data-ttu-id="a2ff6-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2ff6-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2ff6-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2ff6-151">JSON representation</span></span>

<span data-ttu-id="a2ff6-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2ff6-152">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="a2ff6-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2ff6-153">Example</span></span>

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
  "suppressions": []
}
-->
