---
title: tipo de recurso participante
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a903eb34191401100d9b19aa17eba6fb9f5c6617
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009213"
---
# <a name="participant-resource-type"></a><span data-ttu-id="3a542-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="3a542-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a542-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="3a542-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="3a542-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="3a542-105">Methods</span></span>

| <span data-ttu-id="3a542-106">Método</span><span class="sxs-lookup"><span data-stu-id="3a542-106">Method</span></span>                                                          | <span data-ttu-id="3a542-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3a542-107">Return Type</span></span>                              | <span data-ttu-id="3a542-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a542-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="3a542-109">Obter participante</span><span class="sxs-lookup"><span data-stu-id="3a542-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="3a542-110">participante</span><span class="sxs-lookup"><span data-stu-id="3a542-110">participant</span></span>](participant.md)            | <span data-ttu-id="3a542-111">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="3a542-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="3a542-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="3a542-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="3a542-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="3a542-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="3a542-114">Configure o mixer de áudio do participante.</span><span class="sxs-lookup"><span data-stu-id="3a542-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="3a542-115">Convidar</span><span class="sxs-lookup"><span data-stu-id="3a542-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="3a542-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="3a542-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="3a542-117">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="3a542-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="3a542-118">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="3a542-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="3a542-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="3a542-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="3a542-120">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="3a542-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="3a542-121">Ativar mudo de todos os participantes</span><span class="sxs-lookup"><span data-stu-id="3a542-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="3a542-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="3a542-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="3a542-123">Ativar mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="3a542-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="3a542-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a542-124">Properties</span></span>

| <span data-ttu-id="3a542-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a542-125">Property</span></span>             | <span data-ttu-id="3a542-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a542-126">Type</span></span>                                     | <span data-ttu-id="3a542-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a542-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="3a542-128">id</span><span class="sxs-lookup"><span data-stu-id="3a542-128">id</span></span>                   | <span data-ttu-id="3a542-129">String</span><span class="sxs-lookup"><span data-stu-id="3a542-129">String</span></span>                                   | <span data-ttu-id="3a542-130">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="3a542-130">The participant id.</span></span>                                          |
| <span data-ttu-id="3a542-131">informações </span><span class="sxs-lookup"><span data-stu-id="3a542-131">info</span></span>                 | [<span data-ttu-id="3a542-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="3a542-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="3a542-133">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="3a542-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="3a542-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="3a542-134">isInLobby</span></span>            | <span data-ttu-id="3a542-135">booliano</span><span class="sxs-lookup"><span data-stu-id="3a542-135">boolean</span></span>                                  | <span data-ttu-id="3a542-136">true se o participante está no lobby</span><span class="sxs-lookup"><span data-stu-id="3a542-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="3a542-137">IsMuted</span><span class="sxs-lookup"><span data-stu-id="3a542-137">isMuted</span></span>              | <span data-ttu-id="3a542-138">booliano</span><span class="sxs-lookup"><span data-stu-id="3a542-138">boolean</span></span>                                  | <span data-ttu-id="3a542-139">true se o participante estiver mudo (cliente ou servidor sem som)</span><span class="sxs-lookup"><span data-stu-id="3a542-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="3a542-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="3a542-140">mediaStreams</span></span>         | <span data-ttu-id="3a542-141">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="3a542-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="3a542-142">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="3a542-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="3a542-143">los</span><span class="sxs-lookup"><span data-stu-id="3a542-143">metadata</span></span>             | <span data-ttu-id="3a542-144">String</span><span class="sxs-lookup"><span data-stu-id="3a542-144">String</span></span>                                   | <span data-ttu-id="3a542-145">Um blob de dados fornecido pelo participante na lista</span><span class="sxs-lookup"><span data-stu-id="3a542-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="3a542-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="3a542-146">recordingInfo</span></span>        | [<span data-ttu-id="3a542-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="3a542-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="3a542-148">Informações sobre o fato de o participante ter capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="3a542-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3a542-149">Relações</span><span class="sxs-lookup"><span data-stu-id="3a542-149">Relationships</span></span>
<span data-ttu-id="3a542-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a542-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a542-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a542-151">JSON representation</span></span>

<span data-ttu-id="3a542-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a542-152">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="3a542-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a542-153">Example</span></span>

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
