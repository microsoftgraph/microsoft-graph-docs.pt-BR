---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 1b2a87d8494876ada8c45849d2cd93142f1dc570
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056489"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="ccdc5-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ccdc5-103">onlineMeeting resource type</span></span>

<span data-ttu-id="ccdc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccdc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ccdc5-105">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="ccdc5-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ccdc5-106">Methods</span></span>

| <span data-ttu-id="ccdc5-107">Método</span><span class="sxs-lookup"><span data-stu-id="ccdc5-107">Method</span></span>         | <span data-ttu-id="ccdc5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ccdc5-108">Return Type</span></span> | <span data-ttu-id="ccdc5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccdc5-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="ccdc5-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="ccdc5-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="ccdc5-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ccdc5-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ccdc5-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="ccdc5-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ccdc5-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="ccdc5-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ccdc5-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ccdc5-115">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="ccdc5-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="ccdc5-116">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ccdc5-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md) | <span data-ttu-id="ccdc5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ccdc5-117">None</span></span> | <span data-ttu-id="ccdc5-118">Excluir uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-118">Delete an online meeting.</span></span> |
| [<span data-ttu-id="ccdc5-119">Criar ou obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ccdc5-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="ccdc5-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ccdc5-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ccdc5-121">Criar uma reunião online com uma ID externa personalizada.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="ccdc5-122">Se a reunião já existir, recupere suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="ccdc5-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccdc5-123">Properties</span></span>

| <span data-ttu-id="ccdc5-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccdc5-124">Property</span></span>                  | <span data-ttu-id="ccdc5-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccdc5-125">Type</span></span>                                                   | <span data-ttu-id="ccdc5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccdc5-126">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ccdc5-127">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="ccdc5-127">audioConferencing</span></span>         | [<span data-ttu-id="ccdc5-128">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="ccdc5-128">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="ccdc5-129">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="ccdc5-130">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-130">Read-only.</span></span> |
| <span data-ttu-id="ccdc5-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="ccdc5-131">chatInfo</span></span>                  | [<span data-ttu-id="ccdc5-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="ccdc5-132">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="ccdc5-133">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-133">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="ccdc5-134">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="ccdc5-134">creationDateTime</span></span>          | <span data-ttu-id="ccdc5-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="ccdc5-135">DateTime</span></span>                                               | <span data-ttu-id="ccdc5-136">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="ccdc5-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-137">Read-only.</span></span> |
| <span data-ttu-id="ccdc5-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ccdc5-138">startDateTime</span></span>             | <span data-ttu-id="ccdc5-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="ccdc5-139">DateTime</span></span>                                               | <span data-ttu-id="ccdc5-140">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-140">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="ccdc5-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ccdc5-141">endDateTime</span></span>               | <span data-ttu-id="ccdc5-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="ccdc5-142">DateTime</span></span>                                               | <span data-ttu-id="ccdc5-143">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-143">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="ccdc5-144">id</span><span class="sxs-lookup"><span data-stu-id="ccdc5-144">id</span></span>                        | <span data-ttu-id="ccdc5-145">String</span><span class="sxs-lookup"><span data-stu-id="ccdc5-145">String</span></span>                                                 | <span data-ttu-id="ccdc5-146">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="ccdc5-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-147">Read-only.</span></span> |
| <span data-ttu-id="ccdc5-148">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="ccdc5-148">joinWebUrl</span></span>                | <span data-ttu-id="ccdc5-149">String</span><span class="sxs-lookup"><span data-stu-id="ccdc5-149">String</span></span>                                                 | <span data-ttu-id="ccdc5-150">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-150">The join URL of the online meeting.</span></span> <span data-ttu-id="ccdc5-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-151">Read-only.</span></span>|
| <span data-ttu-id="ccdc5-152">participants</span><span class="sxs-lookup"><span data-stu-id="ccdc5-152">participants</span></span>              | [<span data-ttu-id="ccdc5-153">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="ccdc5-153">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="ccdc5-154">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="ccdc5-155">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-155">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="ccdc5-156">assunto</span><span class="sxs-lookup"><span data-stu-id="ccdc5-156">subject</span></span>                   | <span data-ttu-id="ccdc5-157">String</span><span class="sxs-lookup"><span data-stu-id="ccdc5-157">String</span></span>                                                 | <span data-ttu-id="ccdc5-158">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-158">The subject of the online meeting.</span></span> |
| <span data-ttu-id="ccdc5-159">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="ccdc5-159">videoTeleconferenceId</span></span>     | <span data-ttu-id="ccdc5-160">String</span><span class="sxs-lookup"><span data-stu-id="ccdc5-160">String</span></span>                                                 | <span data-ttu-id="ccdc5-161">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-161">The video teleconferencing ID.</span></span> <span data-ttu-id="ccdc5-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-162">Read-only.</span></span> |
| <span data-ttu-id="ccdc5-163">joinInformation</span><span class="sxs-lookup"><span data-stu-id="ccdc5-163">joinInformation</span></span> | [<span data-ttu-id="ccdc5-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="ccdc5-164">itemBody</span></span>](itembody.md) | <span data-ttu-id="ccdc5-165">As informações de ingresso no idioma e na variante de localidade especificados no `Accept-Language` cabeçalho HTTP da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="ccdc5-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ccdc5-166">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ccdc5-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccdc5-167">JSON representation</span></span>

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

