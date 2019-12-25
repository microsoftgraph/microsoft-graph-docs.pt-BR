---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 105c9f3ffa594dd457b40124070aef0dbb96689a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870989"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="fbc59-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="fbc59-103">onlineMeeting resource type</span></span>

<span data-ttu-id="fbc59-104">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="fbc59-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="fbc59-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fbc59-105">Methods</span></span>

| <span data-ttu-id="fbc59-106">Método</span><span class="sxs-lookup"><span data-stu-id="fbc59-106">Method</span></span>         | <span data-ttu-id="fbc59-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fbc59-107">Return Type</span></span> | <span data-ttu-id="fbc59-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc59-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="fbc59-109">Criar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="fbc59-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="fbc59-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="fbc59-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="fbc59-111">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="fbc59-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="fbc59-112">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="fbc59-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="fbc59-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="fbc59-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="fbc59-114">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="fbc59-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="fbc59-115">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="fbc59-115">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="fbc59-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbc59-116">None</span></span> | <span data-ttu-id="fbc59-117">Excluir uma reunião online</span><span class="sxs-lookup"><span data-stu-id="fbc59-117">Delete an online meeting</span></span> |

## <a name="properties"></a><span data-ttu-id="fbc59-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbc59-118">Properties</span></span>

| <span data-ttu-id="fbc59-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbc59-119">Property</span></span>                  | <span data-ttu-id="fbc59-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc59-120">Type</span></span>                                                   | <span data-ttu-id="fbc59-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc59-121">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fbc59-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="fbc59-122">audioConferencing</span></span>         | [<span data-ttu-id="fbc59-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="fbc59-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="fbc59-124">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="fbc59-124">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="fbc59-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc59-125">Read-only.</span></span> |
| <span data-ttu-id="fbc59-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="fbc59-126">chatInfo</span></span>                  | [<span data-ttu-id="fbc59-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="fbc59-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="fbc59-128">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="fbc59-128">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="fbc59-129">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="fbc59-129">creationDateTime</span></span>          | <span data-ttu-id="fbc59-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="fbc59-130">DateTime</span></span>                                               | <span data-ttu-id="fbc59-131">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="fbc59-131">The meeting creation time in UTC.</span></span> <span data-ttu-id="fbc59-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc59-132">Read-only.</span></span> |
| <span data-ttu-id="fbc59-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc59-133">startDateTime</span></span>             | <span data-ttu-id="fbc59-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="fbc59-134">DateTime</span></span>                                               | <span data-ttu-id="fbc59-135">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="fbc59-135">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="fbc59-136">endDateTime</span><span class="sxs-lookup"><span data-stu-id="fbc59-136">endDateTime</span></span>               | <span data-ttu-id="fbc59-137">DateTime</span><span class="sxs-lookup"><span data-stu-id="fbc59-137">DateTime</span></span>                                               | <span data-ttu-id="fbc59-138">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="fbc59-138">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="fbc59-139">id</span><span class="sxs-lookup"><span data-stu-id="fbc59-139">id</span></span>                        | <span data-ttu-id="fbc59-140">String</span><span class="sxs-lookup"><span data-stu-id="fbc59-140">String</span></span>                                                 | <span data-ttu-id="fbc59-141">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="fbc59-141">The default ID associated with the online meeting.</span></span> <span data-ttu-id="fbc59-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc59-142">Read-only.</span></span> |
| <span data-ttu-id="fbc59-143">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="fbc59-143">joinWebUrl</span></span>                | <span data-ttu-id="fbc59-144">String</span><span class="sxs-lookup"><span data-stu-id="fbc59-144">String</span></span>                                                 | <span data-ttu-id="fbc59-145">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="fbc59-145">The join URL of the online meeting.</span></span> <span data-ttu-id="fbc59-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc59-146">Read-only.</span></span>|
| <span data-ttu-id="fbc59-147">participants</span><span class="sxs-lookup"><span data-stu-id="fbc59-147">participants</span></span>              | [<span data-ttu-id="fbc59-148">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="fbc59-148">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="fbc59-149">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="fbc59-149">The participants associated with the online meeting.</span></span>  <span data-ttu-id="fbc59-150">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="fbc59-150">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="fbc59-151">subject</span><span class="sxs-lookup"><span data-stu-id="fbc59-151">subject</span></span>                   | <span data-ttu-id="fbc59-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc59-152">String</span></span>                                                 | <span data-ttu-id="fbc59-153">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="fbc59-153">The subject of the online meeting.</span></span> |
| <span data-ttu-id="fbc59-154">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="fbc59-154">videoTeleconferenceId</span></span>     | <span data-ttu-id="fbc59-155">String</span><span class="sxs-lookup"><span data-stu-id="fbc59-155">String</span></span>                                                 | <span data-ttu-id="fbc59-156">A ID de teleconferência do videio.</span><span class="sxs-lookup"><span data-stu-id="fbc59-156">The videio teleconferencing ID.</span></span> <span data-ttu-id="fbc59-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc59-157">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="fbc59-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbc59-158">JSON representation</span></span>

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
