---
title: tipo de recurso participante
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d76dd0643d76d5899c5f46dceee6a5ecca21f389
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866655"
---
# <a name="participant-resource-type"></a><span data-ttu-id="eea7d-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="eea7d-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eea7d-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="eea7d-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="eea7d-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="eea7d-105">Methods</span></span>

| <span data-ttu-id="eea7d-106">Método</span><span class="sxs-lookup"><span data-stu-id="eea7d-106">Method</span></span>                                                 | <span data-ttu-id="eea7d-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eea7d-107">Return Type</span></span>                                                 | <span data-ttu-id="eea7d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="eea7d-108">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="eea7d-109">Obter participante</span><span class="sxs-lookup"><span data-stu-id="eea7d-109">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="eea7d-110">participante</span><span class="sxs-lookup"><span data-stu-id="eea7d-110">participant</span></span>](participant.md)                               | <span data-ttu-id="eea7d-111">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="eea7d-111">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="eea7d-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="eea7d-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="eea7d-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="eea7d-113">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="eea7d-114">Configure o mixer de áudio do participante.</span><span class="sxs-lookup"><span data-stu-id="eea7d-114">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="eea7d-115">Convidar</span><span class="sxs-lookup"><span data-stu-id="eea7d-115">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="eea7d-116">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="eea7d-116">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="eea7d-117">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="eea7d-117">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="eea7d-118">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="eea7d-118">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="eea7d-119">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="eea7d-119">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="eea7d-120">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="eea7d-120">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="eea7d-121">Ativar mudo para todos os participantes</span><span class="sxs-lookup"><span data-stu-id="eea7d-121">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="eea7d-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="eea7d-122">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="eea7d-123">Ativar mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="eea7d-123">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="eea7d-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eea7d-124">Properties</span></span>

| <span data-ttu-id="eea7d-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eea7d-125">Property</span></span>             | <span data-ttu-id="eea7d-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="eea7d-126">Type</span></span>                                     | <span data-ttu-id="eea7d-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="eea7d-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="eea7d-128">id</span><span class="sxs-lookup"><span data-stu-id="eea7d-128">id</span></span>                   | <span data-ttu-id="eea7d-129">String</span><span class="sxs-lookup"><span data-stu-id="eea7d-129">String</span></span>                                   | <span data-ttu-id="eea7d-130">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="eea7d-130">The participant ID.</span></span>                                          |
| <span data-ttu-id="eea7d-131">informações </span><span class="sxs-lookup"><span data-stu-id="eea7d-131">info</span></span>                 | [<span data-ttu-id="eea7d-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="eea7d-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="eea7d-133">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="eea7d-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="eea7d-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="eea7d-134">isInLobby</span></span>            | <span data-ttu-id="eea7d-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="eea7d-135">Boolean</span></span>                                  | <span data-ttu-id="eea7d-136">`true`Se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="eea7d-136">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="eea7d-137">IsMuted</span><span class="sxs-lookup"><span data-stu-id="eea7d-137">isMuted</span></span>              | <span data-ttu-id="eea7d-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="eea7d-138">Boolean</span></span>                                  | <span data-ttu-id="eea7d-139">`true`Se o participante estiver com mudo ativado (cliente ou servidor sem som).</span><span class="sxs-lookup"><span data-stu-id="eea7d-139">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="eea7d-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="eea7d-140">mediaStreams</span></span>         | <span data-ttu-id="eea7d-141">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="eea7d-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="eea7d-142">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="eea7d-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="eea7d-143">los</span><span class="sxs-lookup"><span data-stu-id="eea7d-143">metadata</span></span>             | <span data-ttu-id="eea7d-144">String</span><span class="sxs-lookup"><span data-stu-id="eea7d-144">String</span></span>                                   | <span data-ttu-id="eea7d-145">Um blob de dados fornecido pelo participante na lista.</span><span class="sxs-lookup"><span data-stu-id="eea7d-145">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="eea7d-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="eea7d-146">recordingInfo</span></span>        | [<span data-ttu-id="eea7d-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="eea7d-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="eea7d-148">Informações sobre o fato de o participante ter capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="eea7d-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="eea7d-149">Relações</span><span class="sxs-lookup"><span data-stu-id="eea7d-149">Relationships</span></span>
<span data-ttu-id="eea7d-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eea7d-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eea7d-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eea7d-151">JSON representation</span></span>

<span data-ttu-id="eea7d-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eea7d-152">The following is a JSON representation of the resource.</span></span>

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
