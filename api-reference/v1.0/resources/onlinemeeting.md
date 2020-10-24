---
title: tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 9f986bf0bd7871185673759a6e98e80d5d10b4b7
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741926"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="8e286-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8e286-103">onlineMeeting resource type</span></span>

<span data-ttu-id="8e286-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e286-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e286-105">Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="8e286-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="8e286-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e286-106">Methods</span></span>

| <span data-ttu-id="8e286-107">Método</span><span class="sxs-lookup"><span data-stu-id="8e286-107">Method</span></span>                                                             | <span data-ttu-id="8e286-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e286-108">Return Type</span></span>                       | <span data-ttu-id="8e286-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e286-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="8e286-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="8e286-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="8e286-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8e286-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="8e286-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e286-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="8e286-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8e286-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="8e286-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8e286-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="8e286-115">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="8e286-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="8e286-116">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8e286-116">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="8e286-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e286-117">None</span></span>                              | <span data-ttu-id="8e286-118">Excluir uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e286-118">Delete an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="8e286-119">Criar ou obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8e286-119">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="8e286-120">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8e286-120">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="8e286-121">Criar uma reunião online com uma ID externa personalizada.</span><span class="sxs-lookup"><span data-stu-id="8e286-121">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="8e286-122">Se a reunião já existir, recupere suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="8e286-122">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e286-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e286-123">Properties</span></span>

| <span data-ttu-id="8e286-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e286-124">Property</span></span>              | <span data-ttu-id="8e286-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e286-125">Type</span></span>                                          | <span data-ttu-id="8e286-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e286-126">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8e286-127">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="8e286-127">audioConferencing</span></span>     | [<span data-ttu-id="8e286-128">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="8e286-128">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="8e286-129">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e286-129">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="8e286-130">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="8e286-130">Read-only.</span></span>                                                   |
| <span data-ttu-id="8e286-131">chatInfo</span><span class="sxs-lookup"><span data-stu-id="8e286-131">chatInfo</span></span>              | [<span data-ttu-id="8e286-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="8e286-132">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="8e286-133">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e286-133">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="8e286-134">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="8e286-134">creationDateTime</span></span>      | <span data-ttu-id="8e286-135">DateTime</span><span class="sxs-lookup"><span data-stu-id="8e286-135">DateTime</span></span>                                      | <span data-ttu-id="8e286-136">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="8e286-136">The meeting creation time in UTC.</span></span> <span data-ttu-id="8e286-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e286-137">Read-only.</span></span>                                                                               |
| <span data-ttu-id="8e286-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8e286-138">startDateTime</span></span>         | <span data-ttu-id="8e286-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="8e286-139">DateTime</span></span>                                      | <span data-ttu-id="8e286-140">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="8e286-140">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="8e286-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8e286-141">endDateTime</span></span>           | <span data-ttu-id="8e286-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="8e286-142">DateTime</span></span>                                      | <span data-ttu-id="8e286-143">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="8e286-143">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="8e286-144">id</span><span class="sxs-lookup"><span data-stu-id="8e286-144">id</span></span>                    | <span data-ttu-id="8e286-145">String</span><span class="sxs-lookup"><span data-stu-id="8e286-145">String</span></span>                                        | <span data-ttu-id="8e286-146">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e286-146">The default ID associated with the online meeting.</span></span> <span data-ttu-id="8e286-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e286-147">Read-only.</span></span>                                                              |
| <span data-ttu-id="8e286-148">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="8e286-148">joinWebUrl</span></span>            | <span data-ttu-id="8e286-149">String</span><span class="sxs-lookup"><span data-stu-id="8e286-149">String</span></span>                                        | <span data-ttu-id="8e286-150">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e286-150">The join URL of the online meeting.</span></span> <span data-ttu-id="8e286-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e286-151">Read-only.</span></span>                                                                             |
| <span data-ttu-id="8e286-152">participants</span><span class="sxs-lookup"><span data-stu-id="8e286-152">participants</span></span>          | [<span data-ttu-id="8e286-153">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="8e286-153">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="8e286-154">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e286-154">The participants associated with the online meeting.</span></span>  <span data-ttu-id="8e286-155">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="8e286-155">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="8e286-156">assunto</span><span class="sxs-lookup"><span data-stu-id="8e286-156">subject</span></span>               | <span data-ttu-id="8e286-157">String</span><span class="sxs-lookup"><span data-stu-id="8e286-157">String</span></span>                                        | <span data-ttu-id="8e286-158">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="8e286-158">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="8e286-159">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="8e286-159">videoTeleconferenceId</span></span> | <span data-ttu-id="8e286-160">String</span><span class="sxs-lookup"><span data-stu-id="8e286-160">String</span></span>                                        | <span data-ttu-id="8e286-161">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="8e286-161">The video teleconferencing ID.</span></span> <span data-ttu-id="8e286-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e286-162">Read-only.</span></span>                                                                                  |
| <span data-ttu-id="8e286-163">joinInformation</span><span class="sxs-lookup"><span data-stu-id="8e286-163">joinInformation</span></span>       | [<span data-ttu-id="8e286-164">itemBody</span><span class="sxs-lookup"><span data-stu-id="8e286-164">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="8e286-165">As informações de ingresso no idioma e na variante de localidade especificados no `Accept-Language` cabeçalho HTTP da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e286-165">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="8e286-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e286-166">Read-only.</span></span> |
| <span data-ttu-id="8e286-167">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="8e286-167">isEntryExitAnnounced</span></span>  | <span data-ttu-id="8e286-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e286-168">Boolean</span></span>                                       | <span data-ttu-id="8e286-169">Se deve ou não ser anunciada quando os chamadores ingressarem ou saírem.</span><span class="sxs-lookup"><span data-stu-id="8e286-169">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="8e286-170">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="8e286-170">lobbyBypassSettings</span></span>   | [<span data-ttu-id="8e286-171">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="8e286-171">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="8e286-172">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="8e286-172">Specifies which participants can bypass the meeting   lobby.</span></span>                                                                 |
| <span data-ttu-id="8e286-173">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="8e286-173">allowedPresenters</span></span>     | <span data-ttu-id="8e286-174">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="8e286-174">onlineMeetingPresenters</span></span>                       | <span data-ttu-id="8e286-175">Especifica quem pode ser um apresentador em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="8e286-175">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="8e286-176">Os valores possíveis estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8e286-176">Possible values are listed in the following table.</span></span>                                           |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="8e286-177">valores de onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="8e286-177">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="8e286-178">Valor</span><span class="sxs-lookup"><span data-stu-id="8e286-178">Value</span></span>              | <span data-ttu-id="8e286-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e286-179">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="8e286-180">têm</span><span class="sxs-lookup"><span data-stu-id="8e286-180">everyone</span></span>           | <span data-ttu-id="8e286-181">Todos é um apresentador (esta é a opção padrão).</span><span class="sxs-lookup"><span data-stu-id="8e286-181">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="8e286-182">organization</span><span class="sxs-lookup"><span data-stu-id="8e286-182">organization</span></span>       | <span data-ttu-id="8e286-183">Todos na organização do organizador é um apresentador.</span><span class="sxs-lookup"><span data-stu-id="8e286-183">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="8e286-184">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="8e286-184">roleIsPresenter</span></span>    | <span data-ttu-id="8e286-185">Somente os participantes cuja função é apresentador são apresentadores.</span><span class="sxs-lookup"><span data-stu-id="8e286-185">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="8e286-186">organizer</span><span class="sxs-lookup"><span data-stu-id="8e286-186">organizer</span></span>          | <span data-ttu-id="8e286-187">Somente o organizador é um apresentador.</span><span class="sxs-lookup"><span data-stu-id="8e286-187">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="8e286-188">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="8e286-188">unknownFutureValue</span></span> | <span data-ttu-id="8e286-189">Valor de futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="8e286-189">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="8e286-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e286-190">JSON representation</span></span>

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

