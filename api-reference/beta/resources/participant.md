---
title: tipo de recurso participante
description: O tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7598171b4d706a639a11d425ffa409e25126dcf8
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137145"
---
# <a name="participant-resource-type"></a><span data-ttu-id="523f5-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="523f5-103">participant resource type</span></span>

<span data-ttu-id="523f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="523f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="523f5-105">Representa um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="523f5-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="523f5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="523f5-106">Methods</span></span>

| <span data-ttu-id="523f5-107">Método</span><span class="sxs-lookup"><span data-stu-id="523f5-107">Method</span></span>                                                 | <span data-ttu-id="523f5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="523f5-108">Return Type</span></span>                                                 | <span data-ttu-id="523f5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="523f5-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="523f5-110">Lista de participantes</span><span class="sxs-lookup"><span data-stu-id="523f5-110">List participant</span></span>](../api/participant-get.md)         | [<span data-ttu-id="523f5-111">participante</span><span class="sxs-lookup"><span data-stu-id="523f5-111">participant</span></span>](participant.md)                               | <span data-ttu-id="523f5-112">Recupere uma lista de objetos **participantes** na chamada.</span><span class="sxs-lookup"><span data-stu-id="523f5-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="523f5-113">Obter participante</span><span class="sxs-lookup"><span data-stu-id="523f5-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="523f5-114">participante</span><span class="sxs-lookup"><span data-stu-id="523f5-114">participant</span></span>](participant.md)                               | <span data-ttu-id="523f5-115">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="523f5-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="523f5-116">Excluir participante</span><span class="sxs-lookup"><span data-stu-id="523f5-116">Delete participant</span></span>](../api/participant-delete.md)     | <span data-ttu-id="523f5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="523f5-117">None</span></span>   | <span data-ttu-id="523f5-118">Excluir um participante de uma chamada.</span><span class="sxs-lookup"><span data-stu-id="523f5-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="523f5-119">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="523f5-119">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="523f5-120">commsOperation</span><span class="sxs-lookup"><span data-stu-id="523f5-120">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="523f5-121">Configure o mixer de áudio do participante.</span><span class="sxs-lookup"><span data-stu-id="523f5-121">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="523f5-122">Convidar</span><span class="sxs-lookup"><span data-stu-id="523f5-122">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="523f5-123">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="523f5-123">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="523f5-124">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="523f5-124">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="523f5-125">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="523f5-125">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="523f5-126">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="523f5-126">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="523f5-127">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="523f5-127">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="523f5-128">Ativar mudo para todos os participantes</span><span class="sxs-lookup"><span data-stu-id="523f5-128">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="523f5-129">commsOperation</span><span class="sxs-lookup"><span data-stu-id="523f5-129">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="523f5-130">Ativar mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="523f5-130">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="523f5-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="523f5-131">Properties</span></span>

| <span data-ttu-id="523f5-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="523f5-132">Property</span></span>             | <span data-ttu-id="523f5-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="523f5-133">Type</span></span>                                     | <span data-ttu-id="523f5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="523f5-134">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="523f5-135">id</span><span class="sxs-lookup"><span data-stu-id="523f5-135">id</span></span>                   | <span data-ttu-id="523f5-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="523f5-136">String</span></span>                                   | <span data-ttu-id="523f5-137">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="523f5-137">The participant ID.</span></span>                                          |
| <span data-ttu-id="523f5-138">informações </span><span class="sxs-lookup"><span data-stu-id="523f5-138">info</span></span>                 | [<span data-ttu-id="523f5-139">participantInfo</span><span class="sxs-lookup"><span data-stu-id="523f5-139">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="523f5-140">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="523f5-140">The participant of the participant.</span></span>                          |
| <span data-ttu-id="523f5-141">isInLobby</span><span class="sxs-lookup"><span data-stu-id="523f5-141">isInLobby</span></span>            | <span data-ttu-id="523f5-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="523f5-142">Boolean</span></span>                                  | <span data-ttu-id="523f5-143">`true` Se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="523f5-143">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="523f5-144">IsMuted</span><span class="sxs-lookup"><span data-stu-id="523f5-144">isMuted</span></span>              | <span data-ttu-id="523f5-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="523f5-145">Boolean</span></span>                                  | <span data-ttu-id="523f5-146">`true` Se o participante estiver com mudo ativado (cliente ou servidor sem som).</span><span class="sxs-lookup"><span data-stu-id="523f5-146">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="523f5-147">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="523f5-147">mediaStreams</span></span>         | <span data-ttu-id="523f5-148">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="523f5-148">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="523f5-149">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="523f5-149">The list of media streams.</span></span>                                   |
| <span data-ttu-id="523f5-150">los</span><span class="sxs-lookup"><span data-stu-id="523f5-150">metadata</span></span>             | <span data-ttu-id="523f5-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="523f5-151">String</span></span>                                   | <span data-ttu-id="523f5-152">Um blob de dados fornecido pelo participante na lista.</span><span class="sxs-lookup"><span data-stu-id="523f5-152">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="523f5-153">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="523f5-153">recordingInfo</span></span>        | [<span data-ttu-id="523f5-154">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="523f5-154">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="523f5-155">Informações sobre o fato de o participante ter capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="523f5-155">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="523f5-156">Relações</span><span class="sxs-lookup"><span data-stu-id="523f5-156">Relationships</span></span>
<span data-ttu-id="523f5-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="523f5-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="523f5-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="523f5-158">JSON representation</span></span>

<span data-ttu-id="523f5-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="523f5-159">The following is a JSON representation of the resource.</span></span>

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


