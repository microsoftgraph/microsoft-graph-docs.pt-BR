---
title: tipo de recurso de participantes
description: O tipo de participante.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c125589506dbd529d2b45df4171e9d54b346cbba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869829"
---
# <a name="participant-resource-type"></a><span data-ttu-id="8ddc5-103">tipo de recurso de participantes</span><span class="sxs-lookup"><span data-stu-id="8ddc5-103">participant resource type</span></span>

> <span data-ttu-id="8ddc5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ddc5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ddc5-106">O tipo de participante.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-106">The participant type.</span></span>

## <a name="methods"></a><span data-ttu-id="8ddc5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ddc5-107">Methods</span></span>

| <span data-ttu-id="8ddc5-108">Método</span><span class="sxs-lookup"><span data-stu-id="8ddc5-108">Method</span></span>                                                          | <span data-ttu-id="8ddc5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ddc5-109">Return Type</span></span>                              | <span data-ttu-id="8ddc5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ddc5-110">Description</span></span>                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [<span data-ttu-id="8ddc5-111">Obtenha um participante</span><span class="sxs-lookup"><span data-stu-id="8ddc5-111">Get participant</span></span>](../api/participant-get.md)                    | [<span data-ttu-id="8ddc5-112">participante</span><span class="sxs-lookup"><span data-stu-id="8ddc5-112">participant</span></span>](participant.md)            | <span data-ttu-id="8ddc5-113">Leia as propriedades do objeto **participante** .</span><span class="sxs-lookup"><span data-stu-id="8ddc5-113">Read properties of the **participant** object.</span></span>    |
| [<span data-ttu-id="8ddc5-114">ConfigureMixer</span><span class="sxs-lookup"><span data-stu-id="8ddc5-114">ConfigureMixer</span></span>](../api/participant-configuremixer.md)          | [<span data-ttu-id="8ddc5-115">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8ddc5-115">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8ddc5-116">Configure o participante mixer de áudio.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-116">Configure the participant audio mixer.</span></span>            |
| [<span data-ttu-id="8ddc5-117">Convidar</span><span class="sxs-lookup"><span data-stu-id="8ddc5-117">Invite</span></span>](../api/participant-invite.md)                          | [<span data-ttu-id="8ddc5-118">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8ddc5-118">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8ddc5-119">Convide um participante à chamada.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-119">Invite a participant to the call.</span></span>                 |
| [<span data-ttu-id="8ddc5-120">Ativar Mudo participante</span><span class="sxs-lookup"><span data-stu-id="8ddc5-120">Mute participant</span></span>](../api/participant-mute.md)                  | [<span data-ttu-id="8ddc5-121">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8ddc5-121">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8ddc5-122">Ativar Mudo de um participante em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-122">Mute a participant in a call.</span></span>                     |
| [<span data-ttu-id="8ddc5-123">Ativar Mudo de todos os participantes</span><span class="sxs-lookup"><span data-stu-id="8ddc5-123">Mute all participants</span></span>](../api/participant-muteall.md)          | [<span data-ttu-id="8ddc5-124">commsOperation</span><span class="sxs-lookup"><span data-stu-id="8ddc5-124">commsOperation</span></span>](commsoperation.md)      | <span data-ttu-id="8ddc5-125">Ativar Mudo de todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-125">Mute all the participants in the meeting.</span></span>         |

## <a name="properties"></a><span data-ttu-id="8ddc5-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ddc5-126">Properties</span></span>

| <span data-ttu-id="8ddc5-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ddc5-127">Property</span></span>             | <span data-ttu-id="8ddc5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ddc5-128">Type</span></span>                                     | <span data-ttu-id="8ddc5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ddc5-129">Description</span></span>                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| <span data-ttu-id="8ddc5-130">id</span><span class="sxs-lookup"><span data-stu-id="8ddc5-130">id</span></span>                   | <span data-ttu-id="8ddc5-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ddc5-131">String</span></span>                                   | <span data-ttu-id="8ddc5-132">A identificação dos participantes.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-132">The participant id.</span></span>                                          |
| <span data-ttu-id="8ddc5-133">Info</span><span class="sxs-lookup"><span data-stu-id="8ddc5-133">info</span></span>                 | [<span data-ttu-id="8ddc5-134">participantInfo</span><span class="sxs-lookup"><span data-stu-id="8ddc5-134">participantInfo</span></span>](participantinfo.md)    | <span data-ttu-id="8ddc5-135">O participante do participante.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-135">The participant of the participant.</span></span>                          |
| <span data-ttu-id="8ddc5-136">isInLobby</span><span class="sxs-lookup"><span data-stu-id="8ddc5-136">isInLobby</span></span>            | <span data-ttu-id="8ddc5-137">booliano</span><span class="sxs-lookup"><span data-stu-id="8ddc5-137">boolean</span></span>                                  | <span data-ttu-id="8ddc5-138">True se o participante estiver no lobby</span><span class="sxs-lookup"><span data-stu-id="8ddc5-138">true if the participant is in lobby</span></span>                          |
| <span data-ttu-id="8ddc5-139">isMuted</span><span class="sxs-lookup"><span data-stu-id="8ddc5-139">isMuted</span></span>              | <span data-ttu-id="8ddc5-140">booliano</span><span class="sxs-lookup"><span data-stu-id="8ddc5-140">boolean</span></span>                                  | <span data-ttu-id="8ddc5-141">True se o participante está sem som (cliente ou servidor sem áudio)</span><span class="sxs-lookup"><span data-stu-id="8ddc5-141">true if the participant is muted (client or server muted)</span></span>    |
| <span data-ttu-id="8ddc5-142">mediaStreams</span><span class="sxs-lookup"><span data-stu-id="8ddc5-142">mediaStreams</span></span>         | <span data-ttu-id="8ddc5-143">coleção [mediaStream](mediastream.md)</span><span class="sxs-lookup"><span data-stu-id="8ddc5-143">[mediaStream](mediastream.md) collection</span></span> | <span data-ttu-id="8ddc5-144">A lista de fluxos de mídia.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-144">The list of media streams.</span></span>                                   |
| <span data-ttu-id="8ddc5-145">metadados</span><span class="sxs-lookup"><span data-stu-id="8ddc5-145">metadata</span></span>             | <span data-ttu-id="8ddc5-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ddc5-146">String</span></span>                                   | <span data-ttu-id="8ddc5-147">Um blob de dados fornecidos pelo participante na lista</span><span class="sxs-lookup"><span data-stu-id="8ddc5-147">A blob of data provided by the participant in the roster</span></span>     |
| <span data-ttu-id="8ddc5-148">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="8ddc5-148">recordingInfo</span></span>        | [<span data-ttu-id="8ddc5-149">recordingInfo</span><span class="sxs-lookup"><span data-stu-id="8ddc5-149">recordingInfo</span></span>](recordinginfo.md)        | <span data-ttu-id="8ddc5-150">Informações sobre se o participante tenha o recurso de gravação.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-150">Information on whether the participant has recording capability.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8ddc5-151">Relações</span><span class="sxs-lookup"><span data-stu-id="8ddc5-151">Relationships</span></span>
<span data-ttu-id="8ddc5-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ddc5-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ddc5-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ddc5-153">JSON representation</span></span>

<span data-ttu-id="8ddc5-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ddc5-154">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="8ddc5-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ddc5-155">Example</span></span>

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
