---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 531413ee2a9c322af99a98ecf2270faa50ccb0e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534154"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="27722-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="27722-103">onlineMeeting resource type</span></span>

<span data-ttu-id="27722-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27722-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27722-105">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="27722-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="27722-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="27722-106">Methods</span></span>

| <span data-ttu-id="27722-107">Método</span><span class="sxs-lookup"><span data-stu-id="27722-107">Method</span></span>         | <span data-ttu-id="27722-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="27722-108">Return Type</span></span> | <span data-ttu-id="27722-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="27722-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="27722-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="27722-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="27722-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="27722-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="27722-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="27722-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="27722-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="27722-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="27722-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="27722-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="27722-115">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="27722-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="27722-116">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="27722-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="27722-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27722-117">None</span></span> | <span data-ttu-id="27722-118">Excluir uma reunião online</span><span class="sxs-lookup"><span data-stu-id="27722-118">Delete an online meeting</span></span> |

## <a name="properties"></a><span data-ttu-id="27722-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27722-119">Properties</span></span>

| <span data-ttu-id="27722-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27722-120">Property</span></span>                  | <span data-ttu-id="27722-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="27722-121">Type</span></span>                                                   | <span data-ttu-id="27722-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="27722-122">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="27722-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="27722-123">audioConferencing</span></span>         | [<span data-ttu-id="27722-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="27722-124">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="27722-125">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="27722-125">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="27722-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27722-126">Read-only.</span></span> |
| <span data-ttu-id="27722-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="27722-127">chatInfo</span></span>                  | [<span data-ttu-id="27722-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="27722-128">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="27722-129">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="27722-129">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="27722-130">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="27722-130">creationDateTime</span></span>          | <span data-ttu-id="27722-131">DateTime</span><span class="sxs-lookup"><span data-stu-id="27722-131">DateTime</span></span>                                               | <span data-ttu-id="27722-132">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="27722-132">The meeting creation time in UTC.</span></span> <span data-ttu-id="27722-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27722-133">Read-only.</span></span> |
| <span data-ttu-id="27722-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="27722-134">startDateTime</span></span>             | <span data-ttu-id="27722-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="27722-135">DateTime</span></span>                                               | <span data-ttu-id="27722-136">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="27722-136">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="27722-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="27722-137">endDateTime</span></span>               | <span data-ttu-id="27722-138">DateTime</span><span class="sxs-lookup"><span data-stu-id="27722-138">DateTime</span></span>                                               | <span data-ttu-id="27722-139">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="27722-139">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="27722-140">id</span><span class="sxs-lookup"><span data-stu-id="27722-140">id</span></span>                        | <span data-ttu-id="27722-141">String</span><span class="sxs-lookup"><span data-stu-id="27722-141">String</span></span>                                                 | <span data-ttu-id="27722-142">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="27722-142">The default ID associated with the online meeting.</span></span> <span data-ttu-id="27722-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27722-143">Read-only.</span></span> |
| <span data-ttu-id="27722-144">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="27722-144">joinWebUrl</span></span>                | <span data-ttu-id="27722-145">String</span><span class="sxs-lookup"><span data-stu-id="27722-145">String</span></span>                                                 | <span data-ttu-id="27722-146">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="27722-146">The join URL of the online meeting.</span></span> <span data-ttu-id="27722-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27722-147">Read-only.</span></span>|
| <span data-ttu-id="27722-148">participantes</span><span class="sxs-lookup"><span data-stu-id="27722-148">participants</span></span>              | [<span data-ttu-id="27722-149">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="27722-149">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="27722-150">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="27722-150">The participants associated with the online meeting.</span></span>  <span data-ttu-id="27722-151">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="27722-151">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="27722-152">subject</span><span class="sxs-lookup"><span data-stu-id="27722-152">subject</span></span>                   | <span data-ttu-id="27722-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27722-153">String</span></span>                                                 | <span data-ttu-id="27722-154">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="27722-154">The subject of the online meeting.</span></span> |
| <span data-ttu-id="27722-155">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="27722-155">videoTeleconferenceId</span></span>     | <span data-ttu-id="27722-156">String</span><span class="sxs-lookup"><span data-stu-id="27722-156">String</span></span>                                                 | <span data-ttu-id="27722-157">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="27722-157">The video teleconferencing ID.</span></span> <span data-ttu-id="27722-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27722-158">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="27722-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27722-159">JSON representation</span></span>

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
