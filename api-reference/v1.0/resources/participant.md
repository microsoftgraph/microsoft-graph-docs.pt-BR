---
title: tipo de recurso participante
description: Representa o tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0c5004ea45cf44818c30ffe02dc48a1f6851e64a
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137110"
---
# <a name="participant-resource-type"></a><span data-ttu-id="a1644-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="a1644-103">participant resource type</span></span>

<span data-ttu-id="a1644-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1644-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1644-105">Representa um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="a1644-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="a1644-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a1644-106">Methods</span></span>

| <span data-ttu-id="a1644-107">Método</span><span class="sxs-lookup"><span data-stu-id="a1644-107">Method</span></span>                                                 | <span data-ttu-id="a1644-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a1644-108">Return Type</span></span>                                                 | <span data-ttu-id="a1644-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1644-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="a1644-110">Lista de participantes</span><span class="sxs-lookup"><span data-stu-id="a1644-110">List participant</span></span>](../api/participant-get.md)          | [<span data-ttu-id="a1644-111">participante</span><span class="sxs-lookup"><span data-stu-id="a1644-111">participant</span></span>](participant.md)                               | <span data-ttu-id="a1644-112">Recupere uma lista de objetos **participantes** na chamada.</span><span class="sxs-lookup"><span data-stu-id="a1644-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="a1644-113">Obter participante</span><span class="sxs-lookup"><span data-stu-id="a1644-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="a1644-114">participante</span><span class="sxs-lookup"><span data-stu-id="a1644-114">participant</span></span>](participant.md)                               | <span data-ttu-id="a1644-115">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="a1644-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="a1644-116">Excluir participante</span><span class="sxs-lookup"><span data-stu-id="a1644-116">Delete participant</span></span>](../api/participant-delete.md)         | <span data-ttu-id="a1644-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1644-117">None</span></span>   | <span data-ttu-id="a1644-118">Excluir um participante de uma chamada.</span><span class="sxs-lookup"><span data-stu-id="a1644-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="a1644-119">Convidar</span><span class="sxs-lookup"><span data-stu-id="a1644-119">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="a1644-120">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="a1644-120">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="a1644-121">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="a1644-121">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="a1644-122">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="a1644-122">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="a1644-123">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="a1644-123">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="a1644-124">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="a1644-124">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="a1644-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1644-125">Properties</span></span>

| <span data-ttu-id="a1644-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1644-126">Property</span></span>             | <span data-ttu-id="a1644-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1644-127">Type</span></span>                                     | <span data-ttu-id="a1644-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1644-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="a1644-129">id</span><span class="sxs-lookup"><span data-stu-id="a1644-129">id</span></span>                   | <span data-ttu-id="a1644-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1644-130">String</span></span>                                   | <span data-ttu-id="a1644-131">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="a1644-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="a1644-132">informações </span><span class="sxs-lookup"><span data-stu-id="a1644-132">info</span></span>                 | [<span data-ttu-id="a1644-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="a1644-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="a1644-134">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="a1644-134">The participant of the participant.</span></span>                          |
| <span data-ttu-id="a1644-135">isInLobby</span><span class="sxs-lookup"><span data-stu-id="a1644-135">isInLobby</span></span>            | <span data-ttu-id="a1644-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1644-136">Boolean</span></span>                                  | <span data-ttu-id="a1644-137">`true` Se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="a1644-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="a1644-138">IsMuted</span><span class="sxs-lookup"><span data-stu-id="a1644-138">isMuted</span></span>              | <span data-ttu-id="a1644-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1644-139">Boolean</span></span>                                  | <span data-ttu-id="a1644-140">`true` Se o participante estiver com mudo ativado (cliente ou servidor sem som).</span><span class="sxs-lookup"><span data-stu-id="a1644-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="a1644-141">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="a1644-141">mediaStreams</span></span>         | <span data-ttu-id="a1644-142">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="a1644-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="a1644-143">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="a1644-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="a1644-144">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="a1644-144">recordingInfo</span></span>        | [<span data-ttu-id="a1644-145">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="a1644-145">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="a1644-146">Informação que especifica se o participante tem capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="a1644-146">Information about whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a1644-147">Relações</span><span class="sxs-lookup"><span data-stu-id="a1644-147">Relationships</span></span>
<span data-ttu-id="a1644-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1644-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1644-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1644-149">JSON representation</span></span>

<span data-ttu-id="a1644-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1644-150">The following is a JSON representation of the resource.</span></span>

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
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ]
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

