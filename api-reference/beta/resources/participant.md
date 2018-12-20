---
title: tipo de recurso de participantes
description: O tipo de participante.
author: VinodRavichandran
ms.openlocfilehash: 3fcc5fc5d95ded3b5424370cd180fde38c1a65be
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380391"
---
# <a name="participant-resource-type"></a><span data-ttu-id="68bd0-103">tipo de recurso de participantes</span><span class="sxs-lookup"><span data-stu-id="68bd0-103">participant resource type</span></span>

> <span data-ttu-id="68bd0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="68bd0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68bd0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="68bd0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68bd0-106">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="68bd0-106">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="68bd0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="68bd0-107">Methods</span></span>

| <span data-ttu-id="68bd0-108">Método		</span><span class="sxs-lookup"><span data-stu-id="68bd0-108">Method</span></span>                                                          | <span data-ttu-id="68bd0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68bd0-109">Return Type</span></span>                              | <span data-ttu-id="68bd0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="68bd0-110">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="68bd0-111">Obtenha um participante</span><span class="sxs-lookup"><span data-stu-id="68bd0-111">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="68bd0-112">participante</span><span class="sxs-lookup"><span data-stu-id="68bd0-112">participant</span></span>](participant.md)            | <span data-ttu-id="68bd0-113">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="68bd0-113">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="68bd0-114">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="68bd0-114">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="68bd0-115">commsOperation</span><span class="sxs-lookup"><span data-stu-id="68bd0-115">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="68bd0-116">Configure o participante mixer de áudio.</span><span class="sxs-lookup"><span data-stu-id="68bd0-116">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="68bd0-117">Convidar</span><span class="sxs-lookup"><span data-stu-id="68bd0-117">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="68bd0-118">commsOperation</span><span class="sxs-lookup"><span data-stu-id="68bd0-118">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="68bd0-119">Convide um participante à chamada.</span><span class="sxs-lookup"><span data-stu-id="68bd0-119">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="68bd0-120">Ativar Mudo participante</span><span class="sxs-lookup"><span data-stu-id="68bd0-120">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="68bd0-121">commsOperation</span><span class="sxs-lookup"><span data-stu-id="68bd0-121">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="68bd0-122">Ativar Mudo de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="68bd0-122">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="68bd0-123">Ativar Mudo de todos os participantes</span><span class="sxs-lookup"><span data-stu-id="68bd0-123">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="68bd0-124">commsOperation</span><span class="sxs-lookup"><span data-stu-id="68bd0-124">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="68bd0-125">Ativar Mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="68bd0-125">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="68bd0-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68bd0-126">Properties</span></span>

| <span data-ttu-id="68bd0-127">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="68bd0-127">Property</span></span>             | <span data-ttu-id="68bd0-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="68bd0-128">Type</span></span>                                     | <span data-ttu-id="68bd0-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="68bd0-129">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="68bd0-130">id</span><span class="sxs-lookup"><span data-stu-id="68bd0-130">id</span></span>                   | <span data-ttu-id="68bd0-131">String</span><span class="sxs-lookup"><span data-stu-id="68bd0-131">String</span></span>                                   | <span data-ttu-id="68bd0-132">A identificação dos participantes.</span><span class="sxs-lookup"><span data-stu-id="68bd0-132">The participant id.</span></span>                                          |
| <span data-ttu-id="68bd0-133">Info</span><span class="sxs-lookup"><span data-stu-id="68bd0-133">info</span></span>                 | [<span data-ttu-id="68bd0-134">participantInfo</span><span class="sxs-lookup"><span data-stu-id="68bd0-134">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="68bd0-135">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="68bd0-135">The participant of the participant.</span></span>                          |
| <span data-ttu-id="68bd0-136">isInLobby</span><span class="sxs-lookup"><span data-stu-id="68bd0-136">isInLobby</span></span>            | <span data-ttu-id="68bd0-137">booliano</span><span class="sxs-lookup"><span data-stu-id="68bd0-137">boolean</span></span>                                  | <span data-ttu-id="68bd0-138">True se o participante estiver no lobby</span><span class="sxs-lookup"><span data-stu-id="68bd0-138">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="68bd0-139">isMuted</span><span class="sxs-lookup"><span data-stu-id="68bd0-139">isMuted</span></span>              | <span data-ttu-id="68bd0-140">booliano</span><span class="sxs-lookup"><span data-stu-id="68bd0-140">boolean</span></span>                                  | <span data-ttu-id="68bd0-141">True se o participante está sem som (cliente ou servidor sem áudio)</span><span class="sxs-lookup"><span data-stu-id="68bd0-141">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="68bd0-142">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="68bd0-142">mediaStreams</span></span>         | <span data-ttu-id="68bd0-143">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="68bd0-143">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="68bd0-144">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="68bd0-144">The list of media streams.</span></span>                                   |
| <span data-ttu-id="68bd0-145">metadados</span><span class="sxs-lookup"><span data-stu-id="68bd0-145">metadata</span></span>             | <span data-ttu-id="68bd0-146">String</span><span class="sxs-lookup"><span data-stu-id="68bd0-146">String</span></span>                                   | <span data-ttu-id="68bd0-147">Um blob de dados fornecidos pelo participante na lista</span><span class="sxs-lookup"><span data-stu-id="68bd0-147">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="68bd0-148">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="68bd0-148">recordingInfo</span></span>        | [<span data-ttu-id="68bd0-149">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="68bd0-149">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="68bd0-150">Informações sobre se o participante tenha o recurso de gravação.</span><span class="sxs-lookup"><span data-stu-id="68bd0-150">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="68bd0-151">Relações</span><span class="sxs-lookup"><span data-stu-id="68bd0-151">Relationships</span></span>
<span data-ttu-id="68bd0-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68bd0-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68bd0-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68bd0-153">JSON representation</span></span>

<span data-ttu-id="68bd0-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68bd0-154">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="68bd0-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68bd0-155">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
