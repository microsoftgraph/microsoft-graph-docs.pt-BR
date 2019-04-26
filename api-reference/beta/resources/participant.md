---
title: tipo de recurso participante
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4a138267529127562fa9df42d8b20a985939b50e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345006"
---
# <a name="participant-resource-type"></a><span data-ttu-id="c7397-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="c7397-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7397-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="c7397-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="c7397-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c7397-105">Methods</span></span>

| <span data-ttu-id="c7397-106">Método</span><span class="sxs-lookup"><span data-stu-id="c7397-106">Method</span></span>                                                          | <span data-ttu-id="c7397-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c7397-107">Return Type</span></span>                              | <span data-ttu-id="c7397-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7397-108">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="c7397-109">Obter participante</span><span class="sxs-lookup"><span data-stu-id="c7397-109">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="c7397-110">participante</span><span class="sxs-lookup"><span data-stu-id="c7397-110">participant</span></span>](participant.md)            | <span data-ttu-id="c7397-111">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="c7397-111">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="c7397-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="c7397-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="c7397-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="c7397-113">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="c7397-114">Configure o mixer de áudio do participante.</span><span class="sxs-lookup"><span data-stu-id="c7397-114">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="c7397-115">Convidar</span><span class="sxs-lookup"><span data-stu-id="c7397-115">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="c7397-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="c7397-116">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="c7397-117">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="c7397-117">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="c7397-118">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="c7397-118">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="c7397-119">commsOperation</span><span class="sxs-lookup"><span data-stu-id="c7397-119">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="c7397-120">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="c7397-120">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="c7397-121">Ativar mudo de todos os participantes</span><span class="sxs-lookup"><span data-stu-id="c7397-121">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="c7397-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="c7397-122">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="c7397-123">Ativar mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="c7397-123">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="c7397-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7397-124">Properties</span></span>

| <span data-ttu-id="c7397-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7397-125">Property</span></span>             | <span data-ttu-id="c7397-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7397-126">Type</span></span>                                     | <span data-ttu-id="c7397-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7397-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="c7397-128">id</span><span class="sxs-lookup"><span data-stu-id="c7397-128">id</span></span>                   | <span data-ttu-id="c7397-129">String</span><span class="sxs-lookup"><span data-stu-id="c7397-129">String</span></span>                                   | <span data-ttu-id="c7397-130">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="c7397-130">The participant id.</span></span>                                          |
| <span data-ttu-id="c7397-131">informações </span><span class="sxs-lookup"><span data-stu-id="c7397-131">info</span></span>                 | [<span data-ttu-id="c7397-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="c7397-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="c7397-133">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="c7397-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="c7397-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="c7397-134">isInLobby</span></span>            | <span data-ttu-id="c7397-135">booliano</span><span class="sxs-lookup"><span data-stu-id="c7397-135">boolean</span></span>                                  | <span data-ttu-id="c7397-136">true se o participante está no lobby</span><span class="sxs-lookup"><span data-stu-id="c7397-136">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="c7397-137">IsMuted</span><span class="sxs-lookup"><span data-stu-id="c7397-137">isMuted</span></span>              | <span data-ttu-id="c7397-138">booliano</span><span class="sxs-lookup"><span data-stu-id="c7397-138">boolean</span></span>                                  | <span data-ttu-id="c7397-139">true se o participante estiver mudo (cliente ou servidor sem som)</span><span class="sxs-lookup"><span data-stu-id="c7397-139">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="c7397-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="c7397-140">mediaStreams</span></span>         | <span data-ttu-id="c7397-141">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="c7397-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="c7397-142">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="c7397-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="c7397-143">los</span><span class="sxs-lookup"><span data-stu-id="c7397-143">metadata</span></span>             | <span data-ttu-id="c7397-144">String</span><span class="sxs-lookup"><span data-stu-id="c7397-144">String</span></span>                                   | <span data-ttu-id="c7397-145">Um blob de dados fornecido pelo participante na lista</span><span class="sxs-lookup"><span data-stu-id="c7397-145">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="c7397-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="c7397-146">recordingInfo</span></span>        | [<span data-ttu-id="c7397-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="c7397-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="c7397-148">Informações sobre o fato de o participante ter capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="c7397-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c7397-149">Relações</span><span class="sxs-lookup"><span data-stu-id="c7397-149">Relationships</span></span>
<span data-ttu-id="c7397-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7397-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7397-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7397-151">JSON representation</span></span>

<span data-ttu-id="c7397-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7397-152">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="c7397-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7397-153">Example</span></span>

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
