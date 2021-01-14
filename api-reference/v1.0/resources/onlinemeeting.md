---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 139cd4a20a6097691189d1bd1f843850ba911a21
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866106"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="b56a7-103">Tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b56a7-103">onlineMeeting resource type</span></span>

<span data-ttu-id="b56a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b56a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b56a7-105">Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="b56a7-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="b56a7-106">Methods</span><span class="sxs-lookup"><span data-stu-id="b56a7-106">Methods</span></span>

| <span data-ttu-id="b56a7-107">Método</span><span class="sxs-lookup"><span data-stu-id="b56a7-107">Method</span></span>                                                             | <span data-ttu-id="b56a7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b56a7-108">Return Type</span></span>                       | <span data-ttu-id="b56a7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b56a7-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="b56a7-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="b56a7-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="b56a7-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b56a7-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="b56a7-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="b56a7-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="b56a7-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b56a7-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="b56a7-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b56a7-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="b56a7-115">Leia as propriedades e os relacionamentos de um **objeto onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="b56a7-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="b56a7-116">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b56a7-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="b56a7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b56a7-117">None</span></span>                              | <span data-ttu-id="b56a7-118">Excluir uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="b56a7-118">Delete an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="b56a7-119">Criar ou obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b56a7-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="b56a7-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="b56a7-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="b56a7-121">Crie uma reunião online com uma ID externa personalizada.</span><span class="sxs-lookup"><span data-stu-id="b56a7-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="b56a7-122">Se a reunião já existir, recupere suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b56a7-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="b56a7-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b56a7-123">Properties</span></span>

| <span data-ttu-id="b56a7-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b56a7-124">Property</span></span>              | <span data-ttu-id="b56a7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="b56a7-125">Type</span></span>                                          | <span data-ttu-id="b56a7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b56a7-126">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b56a7-127">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="b56a7-127">audioConferencing</span></span>     | [<span data-ttu-id="b56a7-128">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="b56a7-128">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="b56a7-129">As informações de acesso telefônico (discagem) de uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="b56a7-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="b56a7-130">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="b56a7-130">Read-only.</span></span>                                                   |
| <span data-ttu-id="b56a7-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="b56a7-131">chatInfo</span></span>              | [<span data-ttu-id="b56a7-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="b56a7-132">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="b56a7-133">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="b56a7-133">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="b56a7-134">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="b56a7-134">creationDateTime</span></span>      | <span data-ttu-id="b56a7-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="b56a7-135">DateTime</span></span>                                      | <span data-ttu-id="b56a7-136">A hora de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="b56a7-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="b56a7-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b56a7-137">Read-only.</span></span>                                                                               |
| <span data-ttu-id="b56a7-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b56a7-138">startDateTime</span></span>         | <span data-ttu-id="b56a7-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="b56a7-139">DateTime</span></span>                                      | <span data-ttu-id="b56a7-140">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="b56a7-140">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="b56a7-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b56a7-141">endDateTime</span></span>           | <span data-ttu-id="b56a7-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="b56a7-142">DateTime</span></span>                                      | <span data-ttu-id="b56a7-143">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="b56a7-143">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="b56a7-144">id</span><span class="sxs-lookup"><span data-stu-id="b56a7-144">id</span></span>                    | <span data-ttu-id="b56a7-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b56a7-145">String</span></span>                                        | <span data-ttu-id="b56a7-146">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="b56a7-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="b56a7-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b56a7-147">Read-only.</span></span>                                                              |
| <span data-ttu-id="b56a7-148">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="b56a7-148">joinWebUrl</span></span>            | <span data-ttu-id="b56a7-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b56a7-149">String</span></span>                                        | <span data-ttu-id="b56a7-150">A URL de junção da reunião online.</span><span class="sxs-lookup"><span data-stu-id="b56a7-150">The join URL of the online meeting.</span></span> <span data-ttu-id="b56a7-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b56a7-151">Read-only.</span></span>                                                                             |
| <span data-ttu-id="b56a7-152">participants</span><span class="sxs-lookup"><span data-stu-id="b56a7-152">participants</span></span>          | [<span data-ttu-id="b56a7-153">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="b56a7-153">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="b56a7-154">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="b56a7-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="b56a7-155">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="b56a7-155">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="b56a7-156">assunto</span><span class="sxs-lookup"><span data-stu-id="b56a7-156">subject</span></span>               | <span data-ttu-id="b56a7-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b56a7-157">String</span></span>                                        | <span data-ttu-id="b56a7-158">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="b56a7-158">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="b56a7-159">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="b56a7-159">videoTeleconferenceId</span></span> | <span data-ttu-id="b56a7-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b56a7-160">String</span></span>                                        | <span data-ttu-id="b56a7-161">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="b56a7-161">The video teleconferencing ID.</span></span> <span data-ttu-id="b56a7-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b56a7-162">Read-only.</span></span>                                                                                  |
| <span data-ttu-id="b56a7-163">joinInformation</span><span class="sxs-lookup"><span data-stu-id="b56a7-163">joinInformation</span></span>       | [<span data-ttu-id="b56a7-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="b56a7-164">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="b56a7-165">As informações de junção na variante de idioma e localidade especificadas no cabeçalho `Accept-Language` HTTP da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b56a7-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="b56a7-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b56a7-166">Read-only.</span></span> |
| <span data-ttu-id="b56a7-167">isEntryExitAnentry</span><span class="sxs-lookup"><span data-stu-id="b56a7-167">isEntryExitAnnounced</span></span>  | <span data-ttu-id="b56a7-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b56a7-168">Boolean</span></span>                                       | <span data-ttu-id="b56a7-169">Se será ou não anunciar quando os chamadores ingressarem ou saírem.</span><span class="sxs-lookup"><span data-stu-id="b56a7-169">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="b56a7-170">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="b56a7-170">lobbyBypassSettings</span></span>   | [<span data-ttu-id="b56a7-171">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="b56a7-171">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="b56a7-172">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="b56a7-172">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="b56a7-173">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="b56a7-173">allowedPresenters</span></span>     | <span data-ttu-id="b56a7-174">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="b56a7-174">onlineMeetingPresenters</span></span>                       | <span data-ttu-id="b56a7-175">Especifica quem pode ser um apresentador em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="b56a7-175">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="b56a7-176">Os valores possíveis estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b56a7-176">Possible values are listed in the following table.</span></span>                          |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="b56a7-177">Valores de onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="b56a7-177">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="b56a7-178">Valor</span><span class="sxs-lookup"><span data-stu-id="b56a7-178">Value</span></span>              | <span data-ttu-id="b56a7-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="b56a7-179">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="b56a7-180">everyone</span><span class="sxs-lookup"><span data-stu-id="b56a7-180">everyone</span></span>           | <span data-ttu-id="b56a7-181">Todos são apresentadores (essa é a opção padrão).</span><span class="sxs-lookup"><span data-stu-id="b56a7-181">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="b56a7-182">organization</span><span class="sxs-lookup"><span data-stu-id="b56a7-182">organization</span></span>       | <span data-ttu-id="b56a7-183">Todos na organização do organizador são apresentadores.</span><span class="sxs-lookup"><span data-stu-id="b56a7-183">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="b56a7-184">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="b56a7-184">roleIsPresenter</span></span>    | <span data-ttu-id="b56a7-185">Somente os participantes cuja função é apresentador são apresentadores.</span><span class="sxs-lookup"><span data-stu-id="b56a7-185">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="b56a7-186">organizer</span><span class="sxs-lookup"><span data-stu-id="b56a7-186">organizer</span></span>          | <span data-ttu-id="b56a7-187">Somente o organizador é um apresentador.</span><span class="sxs-lookup"><span data-stu-id="b56a7-187">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="b56a7-188">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="b56a7-188">unknownFutureValue</span></span> | <span data-ttu-id="b56a7-189">Valor futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="b56a7-189">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="b56a7-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b56a7-190">JSON representation</span></span>

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
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String"
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

