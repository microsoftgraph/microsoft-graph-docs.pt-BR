---
title: tipo de recurso participante
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c4bcaca9ea85a85d87e0584f37f0efeb89ed3773
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748011"
---
# <a name="participant-resource-type"></a><span data-ttu-id="3f55c-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="3f55c-103">participant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f55c-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="3f55c-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="3f55c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="3f55c-105">Methods</span></span>

| <span data-ttu-id="3f55c-106">Método</span><span class="sxs-lookup"><span data-stu-id="3f55c-106">Method</span></span>                                                 | <span data-ttu-id="3f55c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3f55c-107">Return Type</span></span>                                                 | <span data-ttu-id="3f55c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f55c-108">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="3f55c-109">Obter participante</span><span class="sxs-lookup"><span data-stu-id="3f55c-109">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="3f55c-110">participante</span><span class="sxs-lookup"><span data-stu-id="3f55c-110">participant</span></span>](participant.md)                               | <span data-ttu-id="3f55c-111">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="3f55c-111">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="3f55c-112">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="3f55c-112">ConfigureMixer</span></span>](../api/participant-configuremixer.md) | [<span data-ttu-id="3f55c-113">commsOperation</span><span class="sxs-lookup"><span data-stu-id="3f55c-113">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="3f55c-114">Configure o mixer de áudio do participante.</span><span class="sxs-lookup"><span data-stu-id="3f55c-114">Configure the participant audio mixer.</span></span>         |
| [<span data-ttu-id="3f55c-115">Convidar</span><span class="sxs-lookup"><span data-stu-id="3f55c-115">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="3f55c-116">commsOperation</span><span class="sxs-lookup"><span data-stu-id="3f55c-116">commsOperation</span></span>](commsoperation.md)                         | <span data-ttu-id="3f55c-117">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="3f55c-117">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="3f55c-118">Participante sem áudio</span><span class="sxs-lookup"><span data-stu-id="3f55c-118">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="3f55c-119">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="3f55c-119">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="3f55c-120">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="3f55c-120">Mute a participant in a call.</span></span>                  |
| [<span data-ttu-id="3f55c-121">Ativar mudo de todos os participantes</span><span class="sxs-lookup"><span data-stu-id="3f55c-121">Mute all participants</span></span>](../api/participant-muteall.md) | [<span data-ttu-id="3f55c-122">commsOperation</span><span class="sxs-lookup"><span data-stu-id="3f55c-122">commsOperation</span></span>](commsoperation.md) | <span data-ttu-id="3f55c-123">Ativar mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="3f55c-123">Mute all the participants in the meeting.</span></span>      |

## <a name="properties"></a><span data-ttu-id="3f55c-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f55c-124">Properties</span></span>

| <span data-ttu-id="3f55c-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f55c-125">Property</span></span>             | <span data-ttu-id="3f55c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f55c-126">Type</span></span>                                     | <span data-ttu-id="3f55c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f55c-127">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="3f55c-128">id</span><span class="sxs-lookup"><span data-stu-id="3f55c-128">id</span></span>                   | <span data-ttu-id="3f55c-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f55c-129">String</span></span>                                   | <span data-ttu-id="3f55c-130">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="3f55c-130">The participant ID.</span></span>                                          |
| <span data-ttu-id="3f55c-131">informações </span><span class="sxs-lookup"><span data-stu-id="3f55c-131">info</span></span>                 | [<span data-ttu-id="3f55c-132">participantInfo</span><span class="sxs-lookup"><span data-stu-id="3f55c-132">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="3f55c-133">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="3f55c-133">The participant of the participant.</span></span>                          |
| <span data-ttu-id="3f55c-134">isInLobby</span><span class="sxs-lookup"><span data-stu-id="3f55c-134">isInLobby</span></span>            | <span data-ttu-id="3f55c-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f55c-135">Boolean</span></span>                                  | <span data-ttu-id="3f55c-136">`true`Se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="3f55c-136">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="3f55c-137">IsMuted</span><span class="sxs-lookup"><span data-stu-id="3f55c-137">isMuted</span></span>              | <span data-ttu-id="3f55c-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f55c-138">Boolean</span></span>                                  | <span data-ttu-id="3f55c-139">`true`Se o participante estiver com mudo ativado (cliente ou servidor sem som).</span><span class="sxs-lookup"><span data-stu-id="3f55c-139">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="3f55c-140">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="3f55c-140">mediaStreams</span></span>         | <span data-ttu-id="3f55c-141">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="3f55c-141">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="3f55c-142">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="3f55c-142">The list of media streams.</span></span>                                   |
| <span data-ttu-id="3f55c-143">los</span><span class="sxs-lookup"><span data-stu-id="3f55c-143">metadata</span></span>             | <span data-ttu-id="3f55c-144">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3f55c-144">String</span></span>                                   | <span data-ttu-id="3f55c-145">Um blob de dados fornecido pelo participante na lista.</span><span class="sxs-lookup"><span data-stu-id="3f55c-145">A blob of data provided by the participant in the roster.</span></span>     |
| <span data-ttu-id="3f55c-146">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="3f55c-146">recordingInfo</span></span>        | [<span data-ttu-id="3f55c-147">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="3f55c-147">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="3f55c-148">Informações sobre o fato de o participante ter capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="3f55c-148">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3f55c-149">Relações</span><span class="sxs-lookup"><span data-stu-id="3f55c-149">Relationships</span></span>
<span data-ttu-id="3f55c-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f55c-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f55c-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f55c-151">JSON representation</span></span>

<span data-ttu-id="3f55c-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f55c-152">The following is a JSON representation of the resource.</span></span>

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
