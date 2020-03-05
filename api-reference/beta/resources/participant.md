---
title: tipo de recurso participante
description: O tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6ae920e35c3ba7c2b31c5947f15b3e9d6585a21c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522036"
---
# <a name="participant-resource-type"></a><span data-ttu-id="38371-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="38371-103">participant resource type</span></span>

<span data-ttu-id="38371-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="38371-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38371-105">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="38371-105">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="38371-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="38371-106">Methods</span></span>

| <span data-ttu-id="38371-107">Método</span><span class="sxs-lookup"><span data-stu-id="38371-107">Method</span></span>                                                 | <span data-ttu-id="38371-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38371-108">Return Type</span></span>                                                 | <span data-ttu-id="38371-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="38371-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="38371-110">Obter participante</span><span class="sxs-lookup"><span data-stu-id="38371-110">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="38371-111">participante</span><span class="sxs-lookup"><span data-stu-id="38371-111">participant</span></span>](participant.md)                               | <span data-ttu-id="38371-112">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="38371-112">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="38371-113">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="38371-113">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="38371-114">commsOperation</span><span class="sxs-lookup"><span data-stu-id="38371-114">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="38371-115">Configure o mixer de áudio do participante.</span><span class="sxs-lookup"><span data-stu-id="38371-115">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="38371-116">Convidar</span><span class="sxs-lookup"><span data-stu-id="38371-116">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="38371-117">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="38371-117">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="38371-118">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="38371-118">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="38371-119">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="38371-119">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="38371-120">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="38371-120">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="38371-121">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="38371-121">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="38371-122">Ativar mudo para todos os participantes</span><span class="sxs-lookup"><span data-stu-id="38371-122">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="38371-123">commsOperation</span><span class="sxs-lookup"><span data-stu-id="38371-123">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="38371-124">Ativar mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="38371-124">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="38371-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38371-125">Properties</span></span>

| <span data-ttu-id="38371-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38371-126">Property</span></span>             | <span data-ttu-id="38371-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="38371-127">Type</span></span>                                     | <span data-ttu-id="38371-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="38371-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="38371-129">id</span><span class="sxs-lookup"><span data-stu-id="38371-129">id</span></span>                   | <span data-ttu-id="38371-130">String</span><span class="sxs-lookup"><span data-stu-id="38371-130">String</span></span>                                   | <span data-ttu-id="38371-131">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="38371-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="38371-132">informações </span><span class="sxs-lookup"><span data-stu-id="38371-132">info</span></span>                 | [<span data-ttu-id="38371-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="38371-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="38371-134">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="38371-134">The participant of the participant.</span></span>                          |
| <span data-ttu-id="38371-135">isInLobby</span><span class="sxs-lookup"><span data-stu-id="38371-135">isInLobby</span></span>            | <span data-ttu-id="38371-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="38371-136">Boolean</span></span>                                  | <span data-ttu-id="38371-137">`true`Se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="38371-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="38371-138">IsMuted</span><span class="sxs-lookup"><span data-stu-id="38371-138">isMuted</span></span>              | <span data-ttu-id="38371-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="38371-139">Boolean</span></span>                                  | <span data-ttu-id="38371-140">`true`Se o participante estiver com mudo ativado (cliente ou servidor sem som).</span><span class="sxs-lookup"><span data-stu-id="38371-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="38371-141">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="38371-141">mediaStreams</span></span>         | <span data-ttu-id="38371-142">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="38371-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="38371-143">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="38371-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="38371-144">los</span><span class="sxs-lookup"><span data-stu-id="38371-144">metadata</span></span>             | <span data-ttu-id="38371-145">String</span><span class="sxs-lookup"><span data-stu-id="38371-145">String</span></span>                                   | <span data-ttu-id="38371-146">Um blob de dados fornecido pelo participante na lista.</span><span class="sxs-lookup"><span data-stu-id="38371-146">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="38371-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="38371-147">recordingInfo</span></span>        | [<span data-ttu-id="38371-148">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="38371-148">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="38371-149">Informações sobre o fato de o participante ter capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="38371-149">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="38371-150">Relações</span><span class="sxs-lookup"><span data-stu-id="38371-150">Relationships</span></span>
<span data-ttu-id="38371-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38371-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38371-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38371-152">JSON representation</span></span>

<span data-ttu-id="38371-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38371-153">The following is a JSON representation of the resource.</span></span>

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
