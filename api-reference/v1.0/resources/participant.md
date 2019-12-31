---
title: tipo de recurso participante
description: O tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3f9e861cc5427243b18ff920facab7544d6315ad
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913734"
---
# <a name="participant-resource-type"></a><span data-ttu-id="b020e-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="b020e-103">participant resource type</span></span>

<span data-ttu-id="b020e-104">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="b020e-104">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="b020e-105">Methods</span><span class="sxs-lookup"><span data-stu-id="b020e-105">Methods</span></span>

| <span data-ttu-id="b020e-106">Método</span><span class="sxs-lookup"><span data-stu-id="b020e-106">Method</span></span>                                                 | <span data-ttu-id="b020e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b020e-107">Return Type</span></span>                                                 | <span data-ttu-id="b020e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b020e-108">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="b020e-109">Obter participante</span><span class="sxs-lookup"><span data-stu-id="b020e-109">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="b020e-110">participante</span><span class="sxs-lookup"><span data-stu-id="b020e-110">participant</span></span>](participant.md)                               | <span data-ttu-id="b020e-111">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="b020e-111">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="b020e-112">Convidar</span><span class="sxs-lookup"><span data-stu-id="b020e-112">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="b020e-113">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="b020e-113">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="b020e-114">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="b020e-114">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="b020e-115">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="b020e-115">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="b020e-116">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="b020e-116">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="b020e-117">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="b020e-117">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="b020e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b020e-118">Properties</span></span>

| <span data-ttu-id="b020e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b020e-119">Property</span></span>             | <span data-ttu-id="b020e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b020e-120">Type</span></span>                                     | <span data-ttu-id="b020e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b020e-121">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="b020e-122">id</span><span class="sxs-lookup"><span data-stu-id="b020e-122">id</span></span>                   | <span data-ttu-id="b020e-123">String</span><span class="sxs-lookup"><span data-stu-id="b020e-123">String</span></span>                                   | <span data-ttu-id="b020e-124">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="b020e-124">The participant ID.</span></span>                                          |
| <span data-ttu-id="b020e-125">informações </span><span class="sxs-lookup"><span data-stu-id="b020e-125">info</span></span>                 | [<span data-ttu-id="b020e-126">participantInfo</span><span class="sxs-lookup"><span data-stu-id="b020e-126">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="b020e-127">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="b020e-127">The participant of the participant.</span></span>                          |
| <span data-ttu-id="b020e-128">isInLobby</span><span class="sxs-lookup"><span data-stu-id="b020e-128">isInLobby</span></span>            | <span data-ttu-id="b020e-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="b020e-129">Boolean</span></span>                                  | <span data-ttu-id="b020e-130">`true`Se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="b020e-130">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="b020e-131">IsMuted</span><span class="sxs-lookup"><span data-stu-id="b020e-131">isMuted</span></span>              | <span data-ttu-id="b020e-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="b020e-132">Boolean</span></span>                                  | <span data-ttu-id="b020e-133">`true`Se o participante estiver com mudo ativado (cliente ou servidor sem som).</span><span class="sxs-lookup"><span data-stu-id="b020e-133">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="b020e-134">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="b020e-134">mediaStreams</span></span>         | <span data-ttu-id="b020e-135">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="b020e-135">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="b020e-136">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="b020e-136">The list of media streams.</span></span>                                   |

## <a name="relationships"></a><span data-ttu-id="b020e-137">Relações</span><span class="sxs-lookup"><span data-stu-id="b020e-137">Relationships</span></span>
<span data-ttu-id="b020e-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b020e-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b020e-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b020e-139">JSON representation</span></span>

<span data-ttu-id="b020e-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b020e-140">The following is a JSON representation of the resource.</span></span>

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
