---
title: tipo de recurso participant
description: O tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dc1038e80566cab0ce37eaa40b4f5c391a625824
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943721"
---
# <a name="participant-resource-type"></a><span data-ttu-id="1b403-103">tipo de recurso participant</span><span class="sxs-lookup"><span data-stu-id="1b403-103">participant resource type</span></span>

<span data-ttu-id="1b403-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b403-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b403-105">Representa um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="1b403-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="1b403-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b403-106">Methods</span></span>

| <span data-ttu-id="1b403-107">Método</span><span class="sxs-lookup"><span data-stu-id="1b403-107">Method</span></span>                                                 | <span data-ttu-id="1b403-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b403-108">Return Type</span></span>                                                 | <span data-ttu-id="1b403-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b403-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="1b403-110">Listar participantes</span><span class="sxs-lookup"><span data-stu-id="1b403-110">List participant</span></span>](../api/participant-get.md)         | [<span data-ttu-id="1b403-111">participante</span><span class="sxs-lookup"><span data-stu-id="1b403-111">participant</span></span>](participant.md)                               | <span data-ttu-id="1b403-112">Recupere uma lista de **objetos** de participante na chamada.</span><span class="sxs-lookup"><span data-stu-id="1b403-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="1b403-113">Obter participante</span><span class="sxs-lookup"><span data-stu-id="1b403-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="1b403-114">participante</span><span class="sxs-lookup"><span data-stu-id="1b403-114">participant</span></span>](participant.md)                               | <span data-ttu-id="1b403-115">Leia as propriedades do **objeto participante.**</span><span class="sxs-lookup"><span data-stu-id="1b403-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="1b403-116">Excluir participante</span><span class="sxs-lookup"><span data-stu-id="1b403-116">Delete participant</span></span>](../api/participant-delete.md)     | <span data-ttu-id="1b403-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b403-117">None</span></span>   | <span data-ttu-id="1b403-118">Exclua um participante de uma chamada.</span><span class="sxs-lookup"><span data-stu-id="1b403-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="1b403-119">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="1b403-119">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="1b403-120">commsOperation</span><span class="sxs-lookup"><span data-stu-id="1b403-120">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="1b403-121">Configure o mixer de áudio do participante.</span><span class="sxs-lookup"><span data-stu-id="1b403-121">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="1b403-122">Convidar</span><span class="sxs-lookup"><span data-stu-id="1b403-122">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="1b403-123">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="1b403-123">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                         | <span data-ttu-id="1b403-124">Convide um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="1b403-124">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="1b403-125">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="1b403-125">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="1b403-126">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="1b403-126">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="1b403-127">Silenciar um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="1b403-127">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="1b403-128">Ativar mudo para todos os participantes</span><span class="sxs-lookup"><span data-stu-id="1b403-128">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="1b403-129">commsOperation</span><span class="sxs-lookup"><span data-stu-id="1b403-129">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="1b403-130">Aumente todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="1b403-130">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="1b403-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b403-131">Properties</span></span>

| <span data-ttu-id="1b403-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b403-132">Property</span></span>             | <span data-ttu-id="1b403-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b403-133">Type</span></span>                                     | <span data-ttu-id="1b403-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b403-134">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="1b403-135">id</span><span class="sxs-lookup"><span data-stu-id="1b403-135">id</span></span>                   | <span data-ttu-id="1b403-136">String</span><span class="sxs-lookup"><span data-stu-id="1b403-136">String</span></span>                                   | <span data-ttu-id="1b403-137">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="1b403-137">The participant ID.</span></span>                                          |
| <span data-ttu-id="1b403-138">informações </span><span class="sxs-lookup"><span data-stu-id="1b403-138">info</span></span>                 | [<span data-ttu-id="1b403-139">participantInfo</span><span class="sxs-lookup"><span data-stu-id="1b403-139">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="1b403-140">Informações sobre o participante.</span><span class="sxs-lookup"><span data-stu-id="1b403-140">Information about the participant.</span></span>                          |
| <span data-ttu-id="1b403-141">isInLobby</span><span class="sxs-lookup"><span data-stu-id="1b403-141">isInLobby</span></span>            | <span data-ttu-id="1b403-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b403-142">Boolean</span></span>                                  | <span data-ttu-id="1b403-143">`true` se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="1b403-143">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="1b403-144">isMuted</span><span class="sxs-lookup"><span data-stu-id="1b403-144">isMuted</span></span>              | <span data-ttu-id="1b403-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b403-145">Boolean</span></span>                                  | <span data-ttu-id="1b403-146">`true` se o participante estiver sem som (cliente ou servidor mudo).</span><span class="sxs-lookup"><span data-stu-id="1b403-146">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="1b403-147">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="1b403-147">mediaStreams</span></span>         | <span data-ttu-id="1b403-148">[Coleção mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="1b403-148">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="1b403-149">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="1b403-149">The list of media streams.</span></span>                                   |
| <span data-ttu-id="1b403-150">metadados</span><span class="sxs-lookup"><span data-stu-id="1b403-150">metadata</span></span>             | <span data-ttu-id="1b403-151">String</span><span class="sxs-lookup"><span data-stu-id="1b403-151">String</span></span>                                   | <span data-ttu-id="1b403-152">Um blob de dados fornecido pelo participante na lista de participação.</span><span class="sxs-lookup"><span data-stu-id="1b403-152">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="1b403-153">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="1b403-153">recordingInfo</span></span>        | [<span data-ttu-id="1b403-154">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="1b403-154">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="1b403-155">Informações sobre se o participante tem capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="1b403-155">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1b403-156">Relações</span><span class="sxs-lookup"><span data-stu-id="1b403-156">Relationships</span></span>
<span data-ttu-id="1b403-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b403-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b403-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b403-158">JSON representation</span></span>

<span data-ttu-id="1b403-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b403-159">The following is a JSON representation of the resource.</span></span>

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


