---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 812f094667b217d167509be324843227e552e0a5
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556223"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="0d894-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d894-103">onlineMeeting resource type</span></span>

<span data-ttu-id="0d894-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d894-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d894-105">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="0d894-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="0d894-106">Methods</span><span class="sxs-lookup"><span data-stu-id="0d894-106">Methods</span></span>

| <span data-ttu-id="0d894-107">Método</span><span class="sxs-lookup"><span data-stu-id="0d894-107">Method</span></span>         | <span data-ttu-id="0d894-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0d894-108">Return Type</span></span> | <span data-ttu-id="0d894-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d894-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="0d894-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="0d894-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="0d894-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d894-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="0d894-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d894-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="0d894-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d894-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="0d894-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d894-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="0d894-115">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="0d894-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="0d894-116">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d894-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="0d894-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0d894-117">None</span></span> | <span data-ttu-id="0d894-118">Excluir uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d894-118">Delete an online meeting.</span></span> |
| [<span data-ttu-id="0d894-119">Criar ou obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d894-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="0d894-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="0d894-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="0d894-121">Criar uma reunião online com uma ID externa personalizada.</span><span class="sxs-lookup"><span data-stu-id="0d894-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="0d894-122">Se a reunião já existir, recupere suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0d894-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d894-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d894-123">Properties</span></span>

| <span data-ttu-id="0d894-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d894-124">Property</span></span>                  | <span data-ttu-id="0d894-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d894-125">Type</span></span>                                                   | <span data-ttu-id="0d894-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d894-126">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="0d894-127">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="0d894-127">audioConferencing</span></span>         | [<span data-ttu-id="0d894-128">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="0d894-128">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="0d894-129">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d894-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="0d894-130">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="0d894-130">Read-only.</span></span> |
| <span data-ttu-id="0d894-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="0d894-131">chatInfo</span></span>                  | [<span data-ttu-id="0d894-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="0d894-132">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="0d894-133">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d894-133">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="0d894-134">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="0d894-134">creationDateTime</span></span>          | <span data-ttu-id="0d894-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="0d894-135">DateTime</span></span>                                               | <span data-ttu-id="0d894-136">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="0d894-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="0d894-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d894-137">Read-only.</span></span> |
| <span data-ttu-id="0d894-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0d894-138">startDateTime</span></span>             | <span data-ttu-id="0d894-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="0d894-139">DateTime</span></span>                                               | <span data-ttu-id="0d894-140">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="0d894-140">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="0d894-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0d894-141">endDateTime</span></span>               | <span data-ttu-id="0d894-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="0d894-142">DateTime</span></span>                                               | <span data-ttu-id="0d894-143">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="0d894-143">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="0d894-144">id</span><span class="sxs-lookup"><span data-stu-id="0d894-144">id</span></span>                        | <span data-ttu-id="0d894-145">String</span><span class="sxs-lookup"><span data-stu-id="0d894-145">String</span></span>                                                 | <span data-ttu-id="0d894-146">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d894-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="0d894-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d894-147">Read-only.</span></span> |
| <span data-ttu-id="0d894-148">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="0d894-148">joinWebUrl</span></span>                | <span data-ttu-id="0d894-149">String</span><span class="sxs-lookup"><span data-stu-id="0d894-149">String</span></span>                                                 | <span data-ttu-id="0d894-150">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d894-150">The join URL of the online meeting.</span></span> <span data-ttu-id="0d894-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d894-151">Read-only.</span></span>|
| <span data-ttu-id="0d894-152">participants</span><span class="sxs-lookup"><span data-stu-id="0d894-152">participants</span></span>              | [<span data-ttu-id="0d894-153">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="0d894-153">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="0d894-154">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d894-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="0d894-155">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="0d894-155">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="0d894-156">subject</span><span class="sxs-lookup"><span data-stu-id="0d894-156">subject</span></span>                   | <span data-ttu-id="0d894-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d894-157">String</span></span>                                                 | <span data-ttu-id="0d894-158">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d894-158">The subject of the online meeting.</span></span> |
| <span data-ttu-id="0d894-159">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="0d894-159">videoTeleconferenceId</span></span>     | <span data-ttu-id="0d894-160">String</span><span class="sxs-lookup"><span data-stu-id="0d894-160">String</span></span>                                                 | <span data-ttu-id="0d894-161">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="0d894-161">The video teleconferencing ID.</span></span> <span data-ttu-id="0d894-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d894-162">Read-only.</span></span> |
| <span data-ttu-id="0d894-163">joinInformation</span><span class="sxs-lookup"><span data-stu-id="0d894-163">joinInformation</span></span> | [<span data-ttu-id="0d894-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="0d894-164">itemBody</span></span>](itembody.md) | <span data-ttu-id="0d894-165">As informações de ingresso no idioma e na variante de localidade especificados no `Accept-Language` cabeçalho HTTP da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d894-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="0d894-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d894-166">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0d894-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d894-167">JSON representation</span></span>

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
