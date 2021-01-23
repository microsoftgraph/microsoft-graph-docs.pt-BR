---
title: tipo de recurso participant
description: Representa o tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 99f165f2f3e99ab424a318b053a060ccda8fdc1c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943714"
---
# <a name="participant-resource-type"></a><span data-ttu-id="1d0d5-103">tipo de recurso participant</span><span class="sxs-lookup"><span data-stu-id="1d0d5-103">participant resource type</span></span>

<span data-ttu-id="1d0d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d0d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d0d5-105">Representa um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-105">Represents a participant in a call.</span></span>

## <a name="methods"></a><span data-ttu-id="1d0d5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d0d5-106">Methods</span></span>

| <span data-ttu-id="1d0d5-107">Método</span><span class="sxs-lookup"><span data-stu-id="1d0d5-107">Method</span></span>                                                 | <span data-ttu-id="1d0d5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d0d5-108">Return Type</span></span>                                                 | <span data-ttu-id="1d0d5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d0d5-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="1d0d5-110">Listar participantes</span><span class="sxs-lookup"><span data-stu-id="1d0d5-110">List participant</span></span>](../api/participant-get.md)          | [<span data-ttu-id="1d0d5-111">participante</span><span class="sxs-lookup"><span data-stu-id="1d0d5-111">participant</span></span>](participant.md)                               | <span data-ttu-id="1d0d5-112">Recupere uma lista de **objetos** de participante na chamada.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-112">Retrieve a list of **participant** objects in the call.</span></span> |
| [<span data-ttu-id="1d0d5-113">Obter participante</span><span class="sxs-lookup"><span data-stu-id="1d0d5-113">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="1d0d5-114">participante</span><span class="sxs-lookup"><span data-stu-id="1d0d5-114">participant</span></span>](participant.md)                               | <span data-ttu-id="1d0d5-115">Leia as propriedades do **objeto participante.**</span><span class="sxs-lookup"><span data-stu-id="1d0d5-115">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="1d0d5-116">Excluir participante</span><span class="sxs-lookup"><span data-stu-id="1d0d5-116">Delete participant</span></span>](../api/participant-delete.md)         | <span data-ttu-id="1d0d5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d0d5-117">None</span></span>   | <span data-ttu-id="1d0d5-118">Exclua um participante de uma chamada.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-118">Delete a participant in a call.</span></span>                  |
| [<span data-ttu-id="1d0d5-119">Convidar</span><span class="sxs-lookup"><span data-stu-id="1d0d5-119">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="1d0d5-120">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="1d0d5-120">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="1d0d5-121">Convide um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-121">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="1d0d5-122">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="1d0d5-122">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="1d0d5-123">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="1d0d5-123">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="1d0d5-124">Silenciar um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-124">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="1d0d5-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d0d5-125">Properties</span></span>

| <span data-ttu-id="1d0d5-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d0d5-126">Property</span></span>             | <span data-ttu-id="1d0d5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d0d5-127">Type</span></span>                                     | <span data-ttu-id="1d0d5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d0d5-128">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="1d0d5-129">id</span><span class="sxs-lookup"><span data-stu-id="1d0d5-129">id</span></span>                   | <span data-ttu-id="1d0d5-130">String</span><span class="sxs-lookup"><span data-stu-id="1d0d5-130">String</span></span>                                   | <span data-ttu-id="1d0d5-131">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-131">The participant ID.</span></span>                                          |
| <span data-ttu-id="1d0d5-132">informações </span><span class="sxs-lookup"><span data-stu-id="1d0d5-132">info</span></span>                 | [<span data-ttu-id="1d0d5-133">participantInfo</span><span class="sxs-lookup"><span data-stu-id="1d0d5-133">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="1d0d5-134">Informações sobre o participante.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-134">Information about the participant.</span></span>                          |
| <span data-ttu-id="1d0d5-135">isInLobby</span><span class="sxs-lookup"><span data-stu-id="1d0d5-135">isInLobby</span></span>            | <span data-ttu-id="1d0d5-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d0d5-136">Boolean</span></span>                                  | <span data-ttu-id="1d0d5-137">`true` se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-137">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="1d0d5-138">isMuted</span><span class="sxs-lookup"><span data-stu-id="1d0d5-138">isMuted</span></span>              | <span data-ttu-id="1d0d5-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d0d5-139">Boolean</span></span>                                  | <span data-ttu-id="1d0d5-140">`true` se o participante estiver sem som (cliente ou servidor mudo).</span><span class="sxs-lookup"><span data-stu-id="1d0d5-140">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="1d0d5-141">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="1d0d5-141">mediaStreams</span></span>         | <span data-ttu-id="1d0d5-142">[Coleção mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="1d0d5-142">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="1d0d5-143">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-143">The list of media streams.</span></span>                                   |
| <span data-ttu-id="1d0d5-144">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="1d0d5-144">recordingInfo</span></span>        | [<span data-ttu-id="1d0d5-145">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="1d0d5-145">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="1d0d5-146">Informações sobre se o participante tem capacidade de gravação.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-146">Information about whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1d0d5-147">Relações</span><span class="sxs-lookup"><span data-stu-id="1d0d5-147">Relationships</span></span>
<span data-ttu-id="1d0d5-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d0d5-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d0d5-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d0d5-149">JSON representation</span></span>

<span data-ttu-id="1d0d5-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d0d5-150">The following is a JSON representation of the resource.</span></span>

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

