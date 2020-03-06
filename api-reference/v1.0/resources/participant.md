---
title: tipo de recurso participante
description: O tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e6711a771d0c10112850f2d05943f4e8752ebbdf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534086"
---
# <a name="participant-resource-type"></a><span data-ttu-id="e209d-103">tipo de recurso participante</span><span class="sxs-lookup"><span data-stu-id="e209d-103">participant resource type</span></span>

<span data-ttu-id="e209d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e209d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e209d-105">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="e209d-105">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="e209d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e209d-106">Methods</span></span>

| <span data-ttu-id="e209d-107">Método</span><span class="sxs-lookup"><span data-stu-id="e209d-107">Method</span></span>                                                 | <span data-ttu-id="e209d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e209d-108">Return Type</span></span>                                                 | <span data-ttu-id="e209d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e209d-109">Description</span></span>                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [<span data-ttu-id="e209d-110">Obter participante</span><span class="sxs-lookup"><span data-stu-id="e209d-110">Get participant</span></span>](../api/participant-get.md)           | [<span data-ttu-id="e209d-111">participante</span><span class="sxs-lookup"><span data-stu-id="e209d-111">participant</span></span>](participant.md)                               | <span data-ttu-id="e209d-112">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="e209d-112">Read properties of the **participant** object.</span></span> |
| [<span data-ttu-id="e209d-113">Convidar</span><span class="sxs-lookup"><span data-stu-id="e209d-113">Invite</span></span>](../api/participant-invite.md)                 | [<span data-ttu-id="e209d-114">inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="e209d-114">inviteParticipantsOperation</span></span>](../resources/inviteparticipantsoperation.md)                        | <span data-ttu-id="e209d-115">Convidar um participante para a chamada.</span><span class="sxs-lookup"><span data-stu-id="e209d-115">Invite a participant to the call.</span></span>              |
| [<span data-ttu-id="e209d-116">Ativar mudo para participante</span><span class="sxs-lookup"><span data-stu-id="e209d-116">Mute participant</span></span>](../api/participant-mute.md)         | [<span data-ttu-id="e209d-117">muteParticipantOperation</span><span class="sxs-lookup"><span data-stu-id="e209d-117">muteParticipantOperation</span></span>](muteparticipantoperation.md)     | <span data-ttu-id="e209d-118">Tirar o áudio de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="e209d-118">Mute a participant in a call.</span></span>                  |

## <a name="properties"></a><span data-ttu-id="e209d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e209d-119">Properties</span></span>

| <span data-ttu-id="e209d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e209d-120">Property</span></span>             | <span data-ttu-id="e209d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e209d-121">Type</span></span>                                     | <span data-ttu-id="e209d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e209d-122">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="e209d-123">id</span><span class="sxs-lookup"><span data-stu-id="e209d-123">id</span></span>                   | <span data-ttu-id="e209d-124">String</span><span class="sxs-lookup"><span data-stu-id="e209d-124">String</span></span>                                   | <span data-ttu-id="e209d-125">A ID do participante.</span><span class="sxs-lookup"><span data-stu-id="e209d-125">The participant ID.</span></span>                                          |
| <span data-ttu-id="e209d-126">informações </span><span class="sxs-lookup"><span data-stu-id="e209d-126">info</span></span>                 | [<span data-ttu-id="e209d-127">participantInfo</span><span class="sxs-lookup"><span data-stu-id="e209d-127">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="e209d-128">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="e209d-128">The participant of the participant.</span></span>                          |
| <span data-ttu-id="e209d-129">isInLobby</span><span class="sxs-lookup"><span data-stu-id="e209d-129">isInLobby</span></span>            | <span data-ttu-id="e209d-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="e209d-130">Boolean</span></span>                                  | <span data-ttu-id="e209d-131">`true`Se o participante estiver no lobby.</span><span class="sxs-lookup"><span data-stu-id="e209d-131">`true` if the participant is in lobby.</span></span>                          |
| <span data-ttu-id="e209d-132">IsMuted</span><span class="sxs-lookup"><span data-stu-id="e209d-132">isMuted</span></span>              | <span data-ttu-id="e209d-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="e209d-133">Boolean</span></span>                                  | <span data-ttu-id="e209d-134">`true`Se o participante estiver com mudo ativado (cliente ou servidor sem som).</span><span class="sxs-lookup"><span data-stu-id="e209d-134">`true` if the participant is muted (client or server muted).</span></span>    |
| <span data-ttu-id="e209d-135">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="e209d-135">mediaStreams</span></span>         | <span data-ttu-id="e209d-136">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="e209d-136">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="e209d-137">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="e209d-137">The list of media streams.</span></span>                                   |

## <a name="relationships"></a><span data-ttu-id="e209d-138">Relações</span><span class="sxs-lookup"><span data-stu-id="e209d-138">Relationships</span></span>
<span data-ttu-id="e209d-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e209d-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e209d-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e209d-140">JSON representation</span></span>

<span data-ttu-id="e209d-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e209d-141">The following is a JSON representation of the resource.</span></span>

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
