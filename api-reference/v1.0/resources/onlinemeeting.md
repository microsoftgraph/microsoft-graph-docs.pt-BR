---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 8ded2e79f8a9a2004f2ffa412b6d42e3275556b8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516091"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="73789-103">Tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="73789-103">onlineMeeting resource type</span></span>

<span data-ttu-id="73789-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73789-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73789-105">Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="73789-105">Contains information about a meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="73789-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="73789-106">Methods</span></span>

| <span data-ttu-id="73789-107">Método</span><span class="sxs-lookup"><span data-stu-id="73789-107">Method</span></span>                                                             | <span data-ttu-id="73789-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73789-108">Return Type</span></span>                       | <span data-ttu-id="73789-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73789-109">Description</span></span>                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="73789-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="73789-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md)  | [<span data-ttu-id="73789-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="73789-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="73789-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="73789-112">Create an online meeting.</span></span>                                                                                    |
| [<span data-ttu-id="73789-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="73789-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md)                   | [<span data-ttu-id="73789-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="73789-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="73789-115">Leia as propriedades e as relações de um **objeto onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="73789-115">Read the properties and relationships of an **onlineMeeting** object.</span></span>                                        |
| [<span data-ttu-id="73789-116">Update</span><span class="sxs-lookup"><span data-stu-id="73789-116">Update</span></span>](../api/onlinemeeting-update.md)                           | [<span data-ttu-id="73789-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="73789-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="73789-118">Atualize as propriedades de um **objeto onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="73789-118">Update the properties of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="73789-119">Excluir onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="73789-119">Delete onlineMeeting</span></span>](../api/onlinemeeting-delete.md)             | <span data-ttu-id="73789-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73789-120">None</span></span>                              | <span data-ttu-id="73789-121">Excluir um **objeto onlineMeeting.**</span><span class="sxs-lookup"><span data-stu-id="73789-121">Delete an **onlineMeeting** object.</span></span>                                                                                    |
| [<span data-ttu-id="73789-122">Criar ou obter OnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="73789-122">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="73789-123">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="73789-123">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="73789-124">Crie um **objeto onlineMeeting** com uma ID externa personalizada.</span><span class="sxs-lookup"><span data-stu-id="73789-124">Create an **onlineMeeting** object with a custom, external ID.</span></span> <span data-ttu-id="73789-125">Se a reunião já existir, recupere suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="73789-125">If the meeting already exists, retrieve its properties.</span></span> |

## <a name="properties"></a><span data-ttu-id="73789-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73789-126">Properties</span></span>

| <span data-ttu-id="73789-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73789-127">Property</span></span>              | <span data-ttu-id="73789-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="73789-128">Type</span></span>                                          | <span data-ttu-id="73789-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="73789-129">Description</span></span>                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="73789-130">allowedPresenters</span><span class="sxs-lookup"><span data-stu-id="73789-130">allowedPresenters</span></span>     | <span data-ttu-id="73789-131">onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="73789-131">onlineMeetingPresenters</span></span>                       | <span data-ttu-id="73789-132">Especifica quem pode ser um apresentador em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="73789-132">Specifies who can be a presenter in a meeting.</span></span> <span data-ttu-id="73789-133">Os valores possíveis são listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="73789-133">Possible values are listed in the following table.</span></span>                          |
| <span data-ttu-id="73789-134">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="73789-134">audioConferencing</span></span>     | [<span data-ttu-id="73789-135">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="73789-135">audioConferencing</span></span>](audioconferencing.md)     | <span data-ttu-id="73789-136">As informações de acesso por telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="73789-136">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="73789-137">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="73789-137">Read-only.</span></span>                                                   |
| <span data-ttu-id="73789-138">chatInfo</span><span class="sxs-lookup"><span data-stu-id="73789-138">chatInfo</span></span>              | [<span data-ttu-id="73789-139">chatInfo</span><span class="sxs-lookup"><span data-stu-id="73789-139">chatInfo</span></span>](chatinfo.md)                       | <span data-ttu-id="73789-140">As informações de chat associadas a essa reunião online.</span><span class="sxs-lookup"><span data-stu-id="73789-140">The chat information associated with this online meeting.</span></span>                                                                  |
| <span data-ttu-id="73789-141">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="73789-141">creationDateTime</span></span>      | <span data-ttu-id="73789-142">DateTime</span><span class="sxs-lookup"><span data-stu-id="73789-142">DateTime</span></span>                                      | <span data-ttu-id="73789-143">O tempo de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="73789-143">The meeting creation time in UTC.</span></span> <span data-ttu-id="73789-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73789-144">Read-only.</span></span>                                                                               |
| <span data-ttu-id="73789-145">endDateTime</span><span class="sxs-lookup"><span data-stu-id="73789-145">endDateTime</span></span>           | <span data-ttu-id="73789-146">DateTime</span><span class="sxs-lookup"><span data-stu-id="73789-146">DateTime</span></span>                                      | <span data-ttu-id="73789-147">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="73789-147">The meeting end time in UTC.</span></span>                                                                                               |
| <span data-ttu-id="73789-148">id</span><span class="sxs-lookup"><span data-stu-id="73789-148">id</span></span>                    | <span data-ttu-id="73789-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73789-149">String</span></span>                                        | <span data-ttu-id="73789-150">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="73789-150">The default ID associated with the online meeting.</span></span> <span data-ttu-id="73789-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73789-151">Read-only.</span></span>                                                              |
| <span data-ttu-id="73789-152">isEntryExitAnnounced</span><span class="sxs-lookup"><span data-stu-id="73789-152">isEntryExitAnnounced</span></span>  | <span data-ttu-id="73789-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="73789-153">Boolean</span></span>                                       | <span data-ttu-id="73789-154">Se os chamadores ingressarão ou sairão.</span><span class="sxs-lookup"><span data-stu-id="73789-154">Whether or not to announce when callers join or leave.</span></span>                                                                     |
| <span data-ttu-id="73789-155">joinInformation</span><span class="sxs-lookup"><span data-stu-id="73789-155">joinInformation</span></span>       | [<span data-ttu-id="73789-156">itemBody</span><span class="sxs-lookup"><span data-stu-id="73789-156">itemBody</span></span>](itembody.md)                       | <span data-ttu-id="73789-157">As informações de junção no idioma e na variante de localidade especificadas no `Accept-Language` cabeçalho HTTP da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73789-157">The join information in the language and locale variant specified in the `Accept-Language` request HTTP header.</span></span> <span data-ttu-id="73789-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73789-158">Read-only.</span></span> |
| <span data-ttu-id="73789-159">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="73789-159">joinWebUrl</span></span>            | <span data-ttu-id="73789-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73789-160">String</span></span>                                        | <span data-ttu-id="73789-161">A URL de junção da reunião online.</span><span class="sxs-lookup"><span data-stu-id="73789-161">The join URL of the online meeting.</span></span> <span data-ttu-id="73789-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73789-162">Read-only.</span></span>                                                                             |
| <span data-ttu-id="73789-163">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="73789-163">lobbyBypassSettings</span></span>   | [<span data-ttu-id="73789-164">lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="73789-164">lobbyBypassSettings</span></span>](lobbyBypassSettings.md) | <span data-ttu-id="73789-165">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="73789-165">Specifies which participants can bypass the meeting   lobby.</span></span>                                                               |
| <span data-ttu-id="73789-166">participants</span><span class="sxs-lookup"><span data-stu-id="73789-166">participants</span></span>          | [<span data-ttu-id="73789-167">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="73789-167">meetingParticipants</span></span>](meetingparticipants.md) | <span data-ttu-id="73789-168">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="73789-168">The participants associated with the online meeting.</span></span>  <span data-ttu-id="73789-169">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="73789-169">This includes the organizer and the attendees.</span></span>                       |
| <span data-ttu-id="73789-170">startDateTime</span><span class="sxs-lookup"><span data-stu-id="73789-170">startDateTime</span></span>         | <span data-ttu-id="73789-171">DateTime</span><span class="sxs-lookup"><span data-stu-id="73789-171">DateTime</span></span>                                      | <span data-ttu-id="73789-172">O horário de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="73789-172">The meeting start time in UTC.</span></span>                                                                                             |
| <span data-ttu-id="73789-173">assunto</span><span class="sxs-lookup"><span data-stu-id="73789-173">subject</span></span>               | <span data-ttu-id="73789-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73789-174">String</span></span>                                        | <span data-ttu-id="73789-175">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="73789-175">The subject of the online meeting.</span></span>                                                                                         |
| <span data-ttu-id="73789-176">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="73789-176">videoTeleconferenceId</span></span> | <span data-ttu-id="73789-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73789-177">String</span></span>                                        | <span data-ttu-id="73789-178">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="73789-178">The video teleconferencing ID.</span></span> <span data-ttu-id="73789-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73789-179">Read-only.</span></span>                                                                                  |

### <a name="onlinemeetingpresenters-values"></a><span data-ttu-id="73789-180">valores onlineMeetingPresenters</span><span class="sxs-lookup"><span data-stu-id="73789-180">onlineMeetingPresenters values</span></span>

| <span data-ttu-id="73789-181">Valor</span><span class="sxs-lookup"><span data-stu-id="73789-181">Value</span></span>              | <span data-ttu-id="73789-182">Descrição</span><span class="sxs-lookup"><span data-stu-id="73789-182">Description</span></span>                                                   |
| ------------------ | ------------------------------------------------------------- |
| <span data-ttu-id="73789-183">everyone</span><span class="sxs-lookup"><span data-stu-id="73789-183">everyone</span></span>           | <span data-ttu-id="73789-184">Todos são apresentadores (essa é a opção padrão).</span><span class="sxs-lookup"><span data-stu-id="73789-184">Everyone is a presenter (This is default option).</span></span>             |
| <span data-ttu-id="73789-185">organização</span><span class="sxs-lookup"><span data-stu-id="73789-185">organization</span></span>       | <span data-ttu-id="73789-186">Todos na organização do organizador são apresentadores.</span><span class="sxs-lookup"><span data-stu-id="73789-186">Everyone in organizer’s organization is a presenter.</span></span>          |
| <span data-ttu-id="73789-187">roleIsPresenter</span><span class="sxs-lookup"><span data-stu-id="73789-187">roleIsPresenter</span></span>    | <span data-ttu-id="73789-188">Somente os participantes cuja função é apresentador são apresentadores.</span><span class="sxs-lookup"><span data-stu-id="73789-188">Only the participants whose role is presenter are presenters.</span></span> |
| <span data-ttu-id="73789-189">organizer</span><span class="sxs-lookup"><span data-stu-id="73789-189">organizer</span></span>          | <span data-ttu-id="73789-190">Somente o organizador é um apresentador.</span><span class="sxs-lookup"><span data-stu-id="73789-190">Only the organizer  is a presenter.</span></span>                           |
| <span data-ttu-id="73789-191">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="73789-191">unknownFutureValue</span></span> | <span data-ttu-id="73789-192">Valor futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="73789-192">Unknow future value.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="73789-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73789-193">JSON representation</span></span>

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

