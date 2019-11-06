---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 64b2c1880edafe1241367ac91889440a513964d9
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006610"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="37c9f-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="37c9f-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c9f-104">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="37c9f-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="37c9f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="37c9f-105">Methods</span></span>

| <span data-ttu-id="37c9f-106">Método</span><span class="sxs-lookup"><span data-stu-id="37c9f-106">Method</span></span>         | <span data-ttu-id="37c9f-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37c9f-107">Return Type</span></span> | <span data-ttu-id="37c9f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c9f-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="37c9f-109">Criar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="37c9f-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="37c9f-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="37c9f-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="37c9f-111">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="37c9f-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="37c9f-112">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="37c9f-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="37c9f-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="37c9f-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="37c9f-114">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="37c9f-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="37c9f-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37c9f-115">Properties</span></span>

| <span data-ttu-id="37c9f-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37c9f-116">Property</span></span>                  | <span data-ttu-id="37c9f-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="37c9f-117">Type</span></span>                                                   | <span data-ttu-id="37c9f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c9f-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="37c9f-119">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="37c9f-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="37c9f-120">String</span><span class="sxs-lookup"><span data-stu-id="37c9f-120">String</span></span>                                                 | <span data-ttu-id="37c9f-121">A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online.</span><span class="sxs-lookup"><span data-stu-id="37c9f-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="37c9f-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c9f-122">Read-only.</span></span> <span data-ttu-id="37c9f-123">Os valores possíveis são `everyone`: `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`,,`organizer`</span><span class="sxs-lookup"><span data-stu-id="37c9f-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`</span></span>|
| <span data-ttu-id="37c9f-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="37c9f-124">audioConferencing</span></span>         | [<span data-ttu-id="37c9f-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="37c9f-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="37c9f-126">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="37c9f-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="37c9f-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c9f-127">Read-only.</span></span> |
| <span data-ttu-id="37c9f-128">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="37c9f-128">canceledDateTime</span></span>          | <span data-ttu-id="37c9f-129">DateTime</span><span class="sxs-lookup"><span data-stu-id="37c9f-129">DateTime</span></span>                                               | <span data-ttu-id="37c9f-130">A hora em UTC quando a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="37c9f-130">The time in UTC when the meeting was canceled.</span></span> <span data-ttu-id="37c9f-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c9f-131">Read-only.</span></span> |
| <span data-ttu-id="37c9f-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="37c9f-132">chatInfo</span></span>                  | [<span data-ttu-id="37c9f-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="37c9f-133">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="37c9f-134">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="37c9f-134">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="37c9f-135">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="37c9f-135">creationDateTime</span></span>          | <span data-ttu-id="37c9f-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="37c9f-136">DateTime</span></span>                                               | <span data-ttu-id="37c9f-137">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="37c9f-137">The meeting creation time in UTC.</span></span> <span data-ttu-id="37c9f-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c9f-138">Read-only.</span></span> |
| <span data-ttu-id="37c9f-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="37c9f-139">startDateTime</span></span>             | <span data-ttu-id="37c9f-140">DateTime</span><span class="sxs-lookup"><span data-stu-id="37c9f-140">DateTime</span></span>                                               | <span data-ttu-id="37c9f-141">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="37c9f-141">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="37c9f-142">endDateTime</span><span class="sxs-lookup"><span data-stu-id="37c9f-142">endDateTime</span></span>               | <span data-ttu-id="37c9f-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="37c9f-143">DateTime</span></span>                                               | <span data-ttu-id="37c9f-144">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="37c9f-144">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="37c9f-145">id</span><span class="sxs-lookup"><span data-stu-id="37c9f-145">id</span></span>                        | <span data-ttu-id="37c9f-146">String</span><span class="sxs-lookup"><span data-stu-id="37c9f-146">String</span></span>                                                 | <span data-ttu-id="37c9f-147">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="37c9f-147">The default ID associated with the online meeting.</span></span> <span data-ttu-id="37c9f-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c9f-148">Read-only.</span></span> |
| <span data-ttu-id="37c9f-149">IsCanceled</span><span class="sxs-lookup"><span data-stu-id="37c9f-149">isCanceled</span></span>                | <span data-ttu-id="37c9f-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="37c9f-150">Boolean</span></span>                                                | <span data-ttu-id="37c9f-151">Indica se a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="37c9f-151">Indicates whether the meeting has been canceled.</span></span> <span data-ttu-id="37c9f-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c9f-152">Read-only.</span></span> |
| <span data-ttu-id="37c9f-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="37c9f-153">joinUrl</span></span>                   | <span data-ttu-id="37c9f-154">String</span><span class="sxs-lookup"><span data-stu-id="37c9f-154">String</span></span>                                                 | <span data-ttu-id="37c9f-155">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="37c9f-155">The join URL of the online meeting.</span></span> <span data-ttu-id="37c9f-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c9f-156">Read-only.</span></span>|
| <span data-ttu-id="37c9f-157">isbroadcast</span><span class="sxs-lookup"><span data-stu-id="37c9f-157">isBroadcast</span></span>               | <span data-ttu-id="37c9f-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="37c9f-158">Boolean</span></span>                                                | <span data-ttu-id="37c9f-159">Indica se a reunião é uma reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="37c9f-159">Indicates whether the meeting is a broadcast meeting.</span></span> |
| <span data-ttu-id="37c9f-160">participants</span><span class="sxs-lookup"><span data-stu-id="37c9f-160">participants</span></span>              | [<span data-ttu-id="37c9f-161">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="37c9f-161">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="37c9f-162">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="37c9f-162">The participants associated with the online meeting.</span></span>  <span data-ttu-id="37c9f-163">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="37c9f-163">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="37c9f-164">assunto</span><span class="sxs-lookup"><span data-stu-id="37c9f-164">subject</span></span>                   | <span data-ttu-id="37c9f-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37c9f-165">String</span></span>                                                 | <span data-ttu-id="37c9f-166">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="37c9f-166">The subject of the online meeting.</span></span> |
| <span data-ttu-id="37c9f-167">capabilities</span><span class="sxs-lookup"><span data-stu-id="37c9f-167">capabilities</span></span>              | <span data-ttu-id="37c9f-168">String collection</span><span class="sxs-lookup"><span data-stu-id="37c9f-168">String collection</span></span>                                      | <span data-ttu-id="37c9f-169">A lista de recursos de reunião.</span><span class="sxs-lookup"><span data-stu-id="37c9f-169">The list of meeting capabilities.</span></span> <span data-ttu-id="37c9f-170">Os valores possíveis são `questionAndAnswer`:.</span><span class="sxs-lookup"><span data-stu-id="37c9f-170">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="37c9f-171">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="37c9f-171">videoTeleconferenceId</span></span>     | <span data-ttu-id="37c9f-172">String</span><span class="sxs-lookup"><span data-stu-id="37c9f-172">String</span></span>                                                 | <span data-ttu-id="37c9f-173">A ID de teleconferência do videio.</span><span class="sxs-lookup"><span data-stu-id="37c9f-173">The videio teleconferencing ID.</span></span> <span data-ttu-id="37c9f-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37c9f-174">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="37c9f-175">valores de autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="37c9f-175">autoAdmittedUsers values</span></span>
| <span data-ttu-id="37c9f-176">Valor</span><span class="sxs-lookup"><span data-stu-id="37c9f-176">Value</span></span> | <span data-ttu-id="37c9f-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="37c9f-177">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="37c9f-178">organizer</span><span class="sxs-lookup"><span data-stu-id="37c9f-178">organizer</span></span> | <span data-ttu-id="37c9f-179">Somente o organizador da reunião é admitido diretamente.</span><span class="sxs-lookup"><span data-stu-id="37c9f-179">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="37c9f-180">Todos os outros esperam no lobby, até que seja admitido pelo organizador</span><span class="sxs-lookup"><span data-stu-id="37c9f-180">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="37c9f-181">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="37c9f-181">invitedUsersInCompany</span></span> | <span data-ttu-id="37c9f-182">O organizador da reunião e os usuários na mesma empresa convidados pelo Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="37c9f-182">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="37c9f-183">Todos os outros esperam no lobby até que seja admitido.</span><span class="sxs-lookup"><span data-stu-id="37c9f-183">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="37c9f-184">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="37c9f-184">everyoneInCompany</span></span> | <span data-ttu-id="37c9f-185">Todos na mesma empresa que o Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="37c9f-185">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="37c9f-186">Usuários federados e anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="37c9f-186">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="37c9f-187">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="37c9f-187">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="37c9f-188">Todos na mesma empresa que o organizador e as empresas federadas ingressam na reunião diretamente.</span><span class="sxs-lookup"><span data-stu-id="37c9f-188">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="37c9f-189">Usuários anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="37c9f-189">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="37c9f-190">têm</span><span class="sxs-lookup"><span data-stu-id="37c9f-190">everyone</span></span> | <span data-ttu-id="37c9f-191">Qualquer usuário é permitido, o que significa que todos (incluindo usuários anônimos) podem participar da reunião diretamente, sem esperar no lobby.</span><span class="sxs-lookup"><span data-stu-id="37c9f-191">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="37c9f-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37c9f-192">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "autoAdmittedUsers": "everyone | everyoneInSameAndFederatedCompany | everyoneInCompany | invitedUsersInCompany | organizer",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCanceled": false,
  "joinUrl": "String",
  "isBroadcast": false,
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
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
