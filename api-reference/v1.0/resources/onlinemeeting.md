---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: mkhribech
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 9de25fd3f9f014627b7fcb32e4a16814e82be1e3
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896484"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="1a652-103">Tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a652-103">onlineMeeting resource type</span></span>

<span data-ttu-id="1a652-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a652-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a652-105">Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="1a652-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="1a652-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a652-106">Methods</span></span>

| <span data-ttu-id="1a652-107">Método</span><span class="sxs-lookup"><span data-stu-id="1a652-107">Method</span></span>                                                             | <span data-ttu-id="1a652-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a652-108">Return Type</span></span>                       | <span data-ttu-id="1a652-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a652-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="1a652-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="1a652-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="1a652-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a652-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="1a652-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="1a652-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="1a652-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a652-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="1a652-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a652-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="1a652-115">Leia as propriedades e as relações de um **objeto onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="1a652-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="1a652-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="1a652-116">Update</span></span>](../api/onlinemeeting-update.md)                           | [<span data-ttu-id="1a652-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a652-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="1a652-118">Atualize as propriedades de um **objeto onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="1a652-118">Update the properties of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="1a652-119">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a652-119">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="1a652-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a652-120">None</span></span>                              | <span data-ttu-id="1a652-121">Excluir um **objeto onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="1a652-121">Delete an **onlineMeeting** object.</span></span>                                                                                    |
| [<span data-ttu-id="1a652-122">Criar ou obter OnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a652-122">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="1a652-123">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1a652-123">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="1a652-124">Crie um **objeto onlineMeeting** com uma ID externa personalizada.</span><span class="sxs-lookup"><span data-stu-id="1a652-124">Create an **onlineMeeting** object with a custom, external ID.</span></span> <span data-ttu-id="1a652-125">Se a reunião já existir, recupere suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1a652-125">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a652-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a652-126">Properties</span></span>

| <span data-ttu-id="1a652-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a652-127">Property</span></span>              | <span data-ttu-id="1a652-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a652-128">Type</span></span>                                          | <span data-ttu-id="1a652-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a652-129">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1a652-130">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="1a652-130">allowedPresenters</span></span>     | [<span data-ttu-id="1a652-131">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="1a652-131">onlineMeetingPresenters</span></span>](#onlinemeetingpresenters-values)                       | <span data-ttu-id="1a652-132">Especifica quem pode ser um apresentador em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="1a652-132">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="1a652-133">Os valores possíveis são listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1a652-133">Possible values are listed in the following table.</span></span>                          |
| <span data-ttu-id="1a652-134">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="1a652-134">audioConferencing</span></span>     | [<span data-ttu-id="1a652-135">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="1a652-135">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="1a652-136">As informações de acesso por telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="1a652-136">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="1a652-137">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="1a652-137">Read-only.</span></span>                                                   |
| <span data-ttu-id="1a652-138">chatInfo</span><span class="sxs-lookup"><span data-stu-id="1a652-138">chatInfo</span></span>              | [<span data-ttu-id="1a652-139">chatInfo</span><span class="sxs-lookup"><span data-stu-id="1a652-139">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="1a652-140">As informações de chat associadas a essa reunião online.</span><span class="sxs-lookup"><span data-stu-id="1a652-140">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="1a652-141">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a652-141">creationDateTime</span></span>      | <span data-ttu-id="1a652-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="1a652-142">DateTime</span></span>                                      | <span data-ttu-id="1a652-143">O tempo de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="1a652-143">The meeting creation time in UTC.</span></span> <span data-ttu-id="1a652-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a652-144">Read-only.</span></span>                                                                               |
| <span data-ttu-id="1a652-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1a652-145">endDateTime</span></span>           | <span data-ttu-id="1a652-146">DateTime</span><span class="sxs-lookup"><span data-stu-id="1a652-146">DateTime</span></span>                                      | <span data-ttu-id="1a652-147">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="1a652-147">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="1a652-148">id</span><span class="sxs-lookup"><span data-stu-id="1a652-148">id</span></span>                    | <span data-ttu-id="1a652-149">String</span><span class="sxs-lookup"><span data-stu-id="1a652-149">String</span></span>                                        | <span data-ttu-id="1a652-150">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="1a652-150">The default ID associated with the online meeting.</span></span> <span data-ttu-id="1a652-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a652-151">Read-only.</span></span>                                                              |
| <span data-ttu-id="1a652-152">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="1a652-152">isEntryExitAnnounced</span></span>  | <span data-ttu-id="1a652-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a652-153">Boolean</span></span>                                       | <span data-ttu-id="1a652-154">Se os chamadores ingressarão ou sairão.</span><span class="sxs-lookup"><span data-stu-id="1a652-154">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="1a652-155">joinInformation</span><span class="sxs-lookup"><span data-stu-id="1a652-155">joinInformation</span></span>       | [<span data-ttu-id="1a652-156">itemBody</span><span class="sxs-lookup"><span data-stu-id="1a652-156">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="1a652-157">As informações de junção no idioma e na variante de localidade especificadas no `Accept-Language` cabeçalho HTTP da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a652-157">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="1a652-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a652-158">Read-only.</span></span> |
| <span data-ttu-id="1a652-159">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="1a652-159">joinWebUrl</span></span>            | <span data-ttu-id="1a652-160">String</span><span class="sxs-lookup"><span data-stu-id="1a652-160">String</span></span>                                        | <span data-ttu-id="1a652-161">A URL de junção da reunião online.</span><span class="sxs-lookup"><span data-stu-id="1a652-161">The join URL of the online meeting.</span></span> <span data-ttu-id="1a652-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a652-162">Read-only.</span></span>                                                                             |
| <span data-ttu-id="1a652-163">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="1a652-163">lobbyBypassSettings</span></span>   | [<span data-ttu-id="1a652-164">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="1a652-164">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="1a652-165">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="1a652-165">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="1a652-166">participants</span><span class="sxs-lookup"><span data-stu-id="1a652-166">participants</span></span>          | [<span data-ttu-id="1a652-167">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="1a652-167">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="1a652-168">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="1a652-168">The participants associated with the online meeting.</span></span>  <span data-ttu-id="1a652-169">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="1a652-169">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="1a652-170">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1a652-170">startDateTime</span></span>         | <span data-ttu-id="1a652-171">DateTime</span><span class="sxs-lookup"><span data-stu-id="1a652-171">DateTime</span></span>                                      | <span data-ttu-id="1a652-172">O horário de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="1a652-172">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="1a652-173">Assunto</span><span class="sxs-lookup"><span data-stu-id="1a652-173">subject</span></span>               | <span data-ttu-id="1a652-174">String</span><span class="sxs-lookup"><span data-stu-id="1a652-174">String</span></span>                                        | <span data-ttu-id="1a652-175">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="1a652-175">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="1a652-176">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="1a652-176">videoTeleconferenceId</span></span> | <span data-ttu-id="1a652-177">String</span><span class="sxs-lookup"><span data-stu-id="1a652-177">String</span></span>                                        | <span data-ttu-id="1a652-178">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="1a652-178">The video teleconferencing ID.</span></span> <span data-ttu-id="1a652-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a652-179">Read-only.</span></span>                                                                                  |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="1a652-180">valores onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="1a652-180">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="1a652-181">Valor</span><span class="sxs-lookup"><span data-stu-id="1a652-181">Value</span></span>              | <span data-ttu-id="1a652-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a652-182">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="1a652-183">everyone</span><span class="sxs-lookup"><span data-stu-id="1a652-183">everyone</span></span>           | <span data-ttu-id="1a652-184">Todos são apresentadores (essa é a opção padrão).</span><span class="sxs-lookup"><span data-stu-id="1a652-184">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="1a652-185">organization</span><span class="sxs-lookup"><span data-stu-id="1a652-185">organization</span></span>       | <span data-ttu-id="1a652-186">Todos na organização do organizador são apresentadores.</span><span class="sxs-lookup"><span data-stu-id="1a652-186">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="1a652-187">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="1a652-187">roleIsPresenter</span></span>    | <span data-ttu-id="1a652-188">Somente os participantes cuja função é apresentador são apresentadores.</span><span class="sxs-lookup"><span data-stu-id="1a652-188">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="1a652-189">organizer</span><span class="sxs-lookup"><span data-stu-id="1a652-189">organizer</span></span>          | <span data-ttu-id="1a652-190">Somente o organizador é um apresentador.</span><span class="sxs-lookup"><span data-stu-id="1a652-190">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="1a652-191">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="1a652-191">unknownFutureValue</span></span> | <span data-ttu-id="1a652-192">Valor futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="1a652-192">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="1a652-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a652-193">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "microsoft.graph.lobbyBypassSettings"},
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

