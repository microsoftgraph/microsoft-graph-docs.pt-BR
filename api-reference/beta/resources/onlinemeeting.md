---
title: tipo de recurso onlineMeeting
description: Captura informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-cloud communications
doc_type: resourcePageType
ms.openlocfilehash: 5cc62c4caa564aa071ffc6b206d5494814b0cb53
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969798"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="f1364-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f1364-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1364-104">Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="f1364-104">Contains information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="f1364-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f1364-105">Methods</span></span>

| <span data-ttu-id="f1364-106">Método</span><span class="sxs-lookup"><span data-stu-id="f1364-106">Method</span></span>         | <span data-ttu-id="f1364-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f1364-107">Return Type</span></span> | <span data-ttu-id="f1364-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1364-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="f1364-109">Criar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f1364-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="f1364-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f1364-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f1364-111">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1364-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="f1364-112">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f1364-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="f1364-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f1364-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f1364-114">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="f1364-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f1364-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1364-115">Properties</span></span>

| <span data-ttu-id="f1364-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1364-116">Property</span></span>                  | <span data-ttu-id="f1364-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1364-117">Type</span></span>                                                   | <span data-ttu-id="f1364-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1364-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f1364-119">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="f1364-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="f1364-120">String</span><span class="sxs-lookup"><span data-stu-id="f1364-120">String</span></span>                                                 | <span data-ttu-id="f1364-121">A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1364-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="f1364-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1364-122">Read-only.</span></span> <span data-ttu-id="f1364-123">Os valores possíveis são `everyone`: `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`,,`organizer`</span><span class="sxs-lookup"><span data-stu-id="f1364-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`</span></span>|
| <span data-ttu-id="f1364-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="f1364-124">audioConferencing</span></span>         | [<span data-ttu-id="f1364-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="f1364-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="f1364-126">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1364-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="f1364-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1364-127">Read-only.</span></span> |
| <span data-ttu-id="f1364-128">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="f1364-128">canceledDateTime</span></span>          | <span data-ttu-id="f1364-129">DateTime</span><span class="sxs-lookup"><span data-stu-id="f1364-129">DateTime</span></span>                                               | <span data-ttu-id="f1364-130">A hora em UTC quando a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="f1364-130">The time in UTC when the meeting was canceled.</span></span> <span data-ttu-id="f1364-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1364-131">Read-only.</span></span> |
| <span data-ttu-id="f1364-132">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f1364-132">chatInfo</span></span>                  | [<span data-ttu-id="f1364-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f1364-133">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="f1364-134">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1364-134">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="f1364-135">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="f1364-135">creationDateTime</span></span>          | <span data-ttu-id="f1364-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="f1364-136">DateTime</span></span>                                               | <span data-ttu-id="f1364-137">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="f1364-137">The meeting creation time in UTC.</span></span> <span data-ttu-id="f1364-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1364-138">Read-only.</span></span> |
| <span data-ttu-id="f1364-139">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f1364-139">startDateTime</span></span>             | <span data-ttu-id="f1364-140">DateTime</span><span class="sxs-lookup"><span data-stu-id="f1364-140">DateTime</span></span>                                               | <span data-ttu-id="f1364-141">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="f1364-141">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="f1364-142">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f1364-142">endDateTime</span></span>               | <span data-ttu-id="f1364-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="f1364-143">DateTime</span></span>                                               | <span data-ttu-id="f1364-144">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="f1364-144">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="f1364-145">id</span><span class="sxs-lookup"><span data-stu-id="f1364-145">id</span></span>                        | <span data-ttu-id="f1364-146">String</span><span class="sxs-lookup"><span data-stu-id="f1364-146">String</span></span>                                                 | <span data-ttu-id="f1364-147">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1364-147">The default ID associated with the online meeting.</span></span> <span data-ttu-id="f1364-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1364-148">Read-only.</span></span> |
| <span data-ttu-id="f1364-149">IsCanceled</span><span class="sxs-lookup"><span data-stu-id="f1364-149">isCanceled</span></span>                | <span data-ttu-id="f1364-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1364-150">Boolean</span></span>                                                | <span data-ttu-id="f1364-151">Indica se a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="f1364-151">Indicates whether the meeting has been canceled.</span></span> <span data-ttu-id="f1364-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1364-152">Read-only.</span></span> |
| <span data-ttu-id="f1364-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="f1364-153">joinUrl</span></span>                   | <span data-ttu-id="f1364-154">String</span><span class="sxs-lookup"><span data-stu-id="f1364-154">String</span></span>                                                 | <span data-ttu-id="f1364-155">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1364-155">The join URL of the online meeting.</span></span> <span data-ttu-id="f1364-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1364-156">Read-only.</span></span>|
| <span data-ttu-id="f1364-157">isbroadcast</span><span class="sxs-lookup"><span data-stu-id="f1364-157">isBroadcast</span></span>               | <span data-ttu-id="f1364-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1364-158">Boolean</span></span>                                                | <span data-ttu-id="f1364-159">O sinalizador para determinar se é uma reunião de transmissão.</span><span class="sxs-lookup"><span data-stu-id="f1364-159">The flag to determine whether it's a broadcast meeting.</span></span> |
| <span data-ttu-id="f1364-160">participants</span><span class="sxs-lookup"><span data-stu-id="f1364-160">participants</span></span>              | [<span data-ttu-id="f1364-161">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="f1364-161">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="f1364-162">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1364-162">The participants associated with the online meeting.</span></span>  <span data-ttu-id="f1364-163">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="f1364-163">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="f1364-164">assunto</span><span class="sxs-lookup"><span data-stu-id="f1364-164">subject</span></span>                   | <span data-ttu-id="f1364-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1364-165">String</span></span>                                                 | <span data-ttu-id="f1364-166">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="f1364-166">The subject of the online meeting.</span></span> |
| <span data-ttu-id="f1364-167">capabilities</span><span class="sxs-lookup"><span data-stu-id="f1364-167">capabilities</span></span>              | <span data-ttu-id="f1364-168">String collection</span><span class="sxs-lookup"><span data-stu-id="f1364-168">String collection</span></span>                                      | <span data-ttu-id="f1364-169">A lista de recursos de reunião.</span><span class="sxs-lookup"><span data-stu-id="f1364-169">The list of meeting capabilities.</span></span> <span data-ttu-id="f1364-170">Os valores possíveis são `questionAndAnswer`:.</span><span class="sxs-lookup"><span data-stu-id="f1364-170">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="f1364-171">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="f1364-171">videoTeleconferenceId</span></span>     | <span data-ttu-id="f1364-172">String</span><span class="sxs-lookup"><span data-stu-id="f1364-172">String</span></span>                                                 | <span data-ttu-id="f1364-173">A ID de teleconferência do videio.</span><span class="sxs-lookup"><span data-stu-id="f1364-173">The videio teleconferencing ID.</span></span> <span data-ttu-id="f1364-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f1364-174">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="f1364-175">valores de autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="f1364-175">autoAdmittedUsers values</span></span>
| <span data-ttu-id="f1364-176">Valor</span><span class="sxs-lookup"><span data-stu-id="f1364-176">Value</span></span> | <span data-ttu-id="f1364-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1364-177">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f1364-178">organizer</span><span class="sxs-lookup"><span data-stu-id="f1364-178">organizer</span></span> | <span data-ttu-id="f1364-179">Somente o organizador da reunião é admitido diretamente.</span><span class="sxs-lookup"><span data-stu-id="f1364-179">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="f1364-180">Todos os outros esperam no lobby, até que seja admitido pelo organizador.</span><span class="sxs-lookup"><span data-stu-id="f1364-180">Everyone else waits in the lobby, until admitted by the organizer.</span></span>  |
| <span data-ttu-id="f1364-181">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="f1364-181">invitedUsersInCompany</span></span> | <span data-ttu-id="f1364-182">O organizador da reunião e os usuários na mesma empresa convidados pelo Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="f1364-182">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="f1364-183">Todos os outros esperam no lobby até que seja admitido.</span><span class="sxs-lookup"><span data-stu-id="f1364-183">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="f1364-184">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="f1364-184">everyoneInCompany</span></span> | <span data-ttu-id="f1364-185">Todos na mesma empresa que o Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="f1364-185">Everyone in the same company as the organizer join the meeting directly.</span></span> <span data-ttu-id="f1364-186">Usuários federados e anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="f1364-186">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="f1364-187">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="f1364-187">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="f1364-188">Todos na mesma empresa que o organizador e as empresas federadas ingressam na reunião diretamente.</span><span class="sxs-lookup"><span data-stu-id="f1364-188">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="f1364-189">Usuários anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="f1364-189">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="f1364-190">têm</span><span class="sxs-lookup"><span data-stu-id="f1364-190">everyone</span></span> | <span data-ttu-id="f1364-191">Qualquer usuário é permitido.</span><span class="sxs-lookup"><span data-stu-id="f1364-191">Any user is allowed.</span></span> <span data-ttu-id="f1364-192">Todos (incluindo usuários anônimos) podem ingressar na reunião diretamente sem esperar no lobby.</span><span class="sxs-lookup"><span data-stu-id="f1364-192">Everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="f1364-193">Relações</span><span class="sxs-lookup"><span data-stu-id="f1364-193">Relationships</span></span>
<span data-ttu-id="f1364-194">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1364-194">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1364-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1364-195">JSON representation</span></span>

<span data-ttu-id="f1364-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1364-196">The following is a JSON representation of the resource.</span></span>

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
