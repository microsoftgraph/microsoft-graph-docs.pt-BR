---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 7b82170b606334c6db8fa07c3f9b2f95f16c0082
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951962"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="9132c-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9132c-103">onlineMeeting resource type</span></span>

<span data-ttu-id="9132c-104">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="9132c-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="9132c-105">Methods</span><span class="sxs-lookup"><span data-stu-id="9132c-105">Methods</span></span>

| <span data-ttu-id="9132c-106">Método</span><span class="sxs-lookup"><span data-stu-id="9132c-106">Method</span></span>         | <span data-ttu-id="9132c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9132c-107">Return Type</span></span> | <span data-ttu-id="9132c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9132c-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="9132c-109">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="9132c-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="9132c-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9132c-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="9132c-111">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="9132c-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="9132c-112">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9132c-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="9132c-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9132c-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="9132c-114">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="9132c-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="9132c-115">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="9132c-115">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="9132c-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9132c-116">None</span></span> | <span data-ttu-id="9132c-117">Excluir uma reunião online</span><span class="sxs-lookup"><span data-stu-id="9132c-117">Delete an online meeting</span></span> |

## <a name="properties"></a><span data-ttu-id="9132c-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9132c-118">Properties</span></span>

| <span data-ttu-id="9132c-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9132c-119">Property</span></span>                  | <span data-ttu-id="9132c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9132c-120">Type</span></span>                                                   | <span data-ttu-id="9132c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9132c-121">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9132c-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="9132c-122">audioConferencing</span></span>         | [<span data-ttu-id="9132c-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="9132c-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="9132c-124">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="9132c-124">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="9132c-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9132c-125">Read-only.</span></span> |
| <span data-ttu-id="9132c-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="9132c-126">chatInfo</span></span>                  | [<span data-ttu-id="9132c-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="9132c-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="9132c-128">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="9132c-128">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="9132c-129">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="9132c-129">creationDateTime</span></span>          | <span data-ttu-id="9132c-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="9132c-130">DateTime</span></span>                                               | <span data-ttu-id="9132c-131">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="9132c-131">The meeting creation time in UTC.</span></span> <span data-ttu-id="9132c-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9132c-132">Read-only.</span></span> |
| <span data-ttu-id="9132c-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9132c-133">startDateTime</span></span>             | <span data-ttu-id="9132c-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="9132c-134">DateTime</span></span>                                               | <span data-ttu-id="9132c-135">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="9132c-135">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="9132c-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9132c-136">endDateTime</span></span>               | <span data-ttu-id="9132c-137">DateTime</span><span class="sxs-lookup"><span data-stu-id="9132c-137">DateTime</span></span>                                               | <span data-ttu-id="9132c-138">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="9132c-138">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="9132c-139">id</span><span class="sxs-lookup"><span data-stu-id="9132c-139">id</span></span>                        | <span data-ttu-id="9132c-140">String</span><span class="sxs-lookup"><span data-stu-id="9132c-140">String</span></span>                                                 | <span data-ttu-id="9132c-141">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="9132c-141">The default ID associated with the online meeting.</span></span> <span data-ttu-id="9132c-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9132c-142">Read-only.</span></span> |
| <span data-ttu-id="9132c-143">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="9132c-143">joinWebUrl</span></span>                | <span data-ttu-id="9132c-144">String</span><span class="sxs-lookup"><span data-stu-id="9132c-144">String</span></span>                                                 | <span data-ttu-id="9132c-145">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="9132c-145">The join URL of the online meeting.</span></span> <span data-ttu-id="9132c-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9132c-146">Read-only.</span></span>|
| <span data-ttu-id="9132c-147">participants</span><span class="sxs-lookup"><span data-stu-id="9132c-147">participants</span></span>              | [<span data-ttu-id="9132c-148">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="9132c-148">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="9132c-149">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="9132c-149">The participants associated with the online meeting.</span></span>  <span data-ttu-id="9132c-150">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="9132c-150">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="9132c-151">assunto</span><span class="sxs-lookup"><span data-stu-id="9132c-151">subject</span></span>                   | <span data-ttu-id="9132c-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9132c-152">String</span></span>                                                 | <span data-ttu-id="9132c-153">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="9132c-153">The subject of the online meeting.</span></span> |
| <span data-ttu-id="9132c-154">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="9132c-154">videoTeleconferenceId</span></span>     | <span data-ttu-id="9132c-155">String</span><span class="sxs-lookup"><span data-stu-id="9132c-155">String</span></span>                                                 | <span data-ttu-id="9132c-156">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="9132c-156">The video teleconferencing ID.</span></span> <span data-ttu-id="9132c-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9132c-157">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9132c-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9132c-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
