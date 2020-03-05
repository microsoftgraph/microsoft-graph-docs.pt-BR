---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: b6e0848b88427cf0929030f07b163204842c3cd7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522253"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="1ad65-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1ad65-103">onlineMeeting resource type</span></span>

<span data-ttu-id="1ad65-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1ad65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ad65-105">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="1ad65-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="1ad65-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1ad65-106">Methods</span></span>

| <span data-ttu-id="1ad65-107">Método</span><span class="sxs-lookup"><span data-stu-id="1ad65-107">Method</span></span>         | <span data-ttu-id="1ad65-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1ad65-108">Return Type</span></span> | <span data-ttu-id="1ad65-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ad65-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="1ad65-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="1ad65-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="1ad65-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1ad65-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="1ad65-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="1ad65-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="1ad65-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1ad65-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="1ad65-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1ad65-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="1ad65-115">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="1ad65-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1ad65-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ad65-116">Properties</span></span>

| <span data-ttu-id="1ad65-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ad65-117">Property</span></span>                  | <span data-ttu-id="1ad65-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ad65-118">Type</span></span>                                                   | <span data-ttu-id="1ad65-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ad65-119">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1ad65-120">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="1ad65-120">autoAdmittedUsers</span></span>         | <span data-ttu-id="1ad65-121">String</span><span class="sxs-lookup"><span data-stu-id="1ad65-121">String</span></span>                                                 | <span data-ttu-id="1ad65-122">A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online.</span><span class="sxs-lookup"><span data-stu-id="1ad65-122">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="1ad65-123">Os valores possíveis são: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span><span class="sxs-lookup"><span data-stu-id="1ad65-123">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="1ad65-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ad65-124">Read-only.</span></span>|
| <span data-ttu-id="1ad65-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="1ad65-125">audioConferencing</span></span>         | [<span data-ttu-id="1ad65-126">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="1ad65-126">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="1ad65-127">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="1ad65-127">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="1ad65-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ad65-128">Read-only.</span></span> |
| <span data-ttu-id="1ad65-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="1ad65-129">chatInfo</span></span>                  | [<span data-ttu-id="1ad65-130">chatInfo</span><span class="sxs-lookup"><span data-stu-id="1ad65-130">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="1ad65-131">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="1ad65-131">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="1ad65-132">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="1ad65-132">creationDateTime</span></span>          | <span data-ttu-id="1ad65-133">DateTime</span><span class="sxs-lookup"><span data-stu-id="1ad65-133">DateTime</span></span>                                               | <span data-ttu-id="1ad65-134">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="1ad65-134">The meeting creation time in UTC.</span></span> <span data-ttu-id="1ad65-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ad65-135">Read-only.</span></span> |
| <span data-ttu-id="1ad65-136">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1ad65-136">startDateTime</span></span>             | <span data-ttu-id="1ad65-137">DateTime</span><span class="sxs-lookup"><span data-stu-id="1ad65-137">DateTime</span></span>                                               | <span data-ttu-id="1ad65-138">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="1ad65-138">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="1ad65-139">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1ad65-139">endDateTime</span></span>               | <span data-ttu-id="1ad65-140">DateTime</span><span class="sxs-lookup"><span data-stu-id="1ad65-140">DateTime</span></span>                                               | <span data-ttu-id="1ad65-141">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="1ad65-141">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="1ad65-142">id</span><span class="sxs-lookup"><span data-stu-id="1ad65-142">id</span></span>                        | <span data-ttu-id="1ad65-143">String</span><span class="sxs-lookup"><span data-stu-id="1ad65-143">String</span></span>                                                 | <span data-ttu-id="1ad65-144">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="1ad65-144">The default ID associated with the online meeting.</span></span> <span data-ttu-id="1ad65-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ad65-145">Read-only.</span></span> |
| <span data-ttu-id="1ad65-146">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="1ad65-146">joinWebUrl</span></span>                   | <span data-ttu-id="1ad65-147">String</span><span class="sxs-lookup"><span data-stu-id="1ad65-147">String</span></span>                                                 | <span data-ttu-id="1ad65-148">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="1ad65-148">The join URL of the online meeting.</span></span> <span data-ttu-id="1ad65-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ad65-149">Read-only.</span></span>|
| <span data-ttu-id="1ad65-150">participantes</span><span class="sxs-lookup"><span data-stu-id="1ad65-150">participants</span></span>              | [<span data-ttu-id="1ad65-151">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="1ad65-151">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="1ad65-152">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="1ad65-152">The participants associated with the online meeting.</span></span>  <span data-ttu-id="1ad65-153">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="1ad65-153">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="1ad65-154">assunto</span><span class="sxs-lookup"><span data-stu-id="1ad65-154">subject</span></span>                   | <span data-ttu-id="1ad65-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ad65-155">String</span></span>                                                 | <span data-ttu-id="1ad65-156">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="1ad65-156">The subject of the online meeting.</span></span> |
| <span data-ttu-id="1ad65-157">capabilities</span><span class="sxs-lookup"><span data-stu-id="1ad65-157">capabilities</span></span>              | <span data-ttu-id="1ad65-158">String collection</span><span class="sxs-lookup"><span data-stu-id="1ad65-158">String collection</span></span>                                      | <span data-ttu-id="1ad65-159">A lista de recursos de reunião.</span><span class="sxs-lookup"><span data-stu-id="1ad65-159">The list of meeting capabilities.</span></span> <span data-ttu-id="1ad65-160">Os valores possíveis são `questionAndAnswer`:.</span><span class="sxs-lookup"><span data-stu-id="1ad65-160">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="1ad65-161">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="1ad65-161">videoTeleconferenceId</span></span>     | <span data-ttu-id="1ad65-162">String</span><span class="sxs-lookup"><span data-stu-id="1ad65-162">String</span></span>                                                 | <span data-ttu-id="1ad65-163">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="1ad65-163">The video teleconferencing ID.</span></span> <span data-ttu-id="1ad65-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ad65-164">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="1ad65-165">valores de autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="1ad65-165">autoAdmittedUsers values</span></span>
| <span data-ttu-id="1ad65-166">Valor</span><span class="sxs-lookup"><span data-stu-id="1ad65-166">Value</span></span> | <span data-ttu-id="1ad65-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ad65-167">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1ad65-168">organizer</span><span class="sxs-lookup"><span data-stu-id="1ad65-168">organizer</span></span> | <span data-ttu-id="1ad65-169">Somente o organizador da reunião é admitido diretamente.</span><span class="sxs-lookup"><span data-stu-id="1ad65-169">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="1ad65-170">Todos os outros esperam no lobby, até que seja admitido pelo organizador</span><span class="sxs-lookup"><span data-stu-id="1ad65-170">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="1ad65-171">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="1ad65-171">invitedUsersInCompany</span></span> | <span data-ttu-id="1ad65-172">O organizador da reunião e os usuários na mesma empresa convidados pelo Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="1ad65-172">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="1ad65-173">Todos os outros esperam no lobby até que seja admitido.</span><span class="sxs-lookup"><span data-stu-id="1ad65-173">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="1ad65-174">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="1ad65-174">everyoneInCompany</span></span> | <span data-ttu-id="1ad65-175">Todos na mesma empresa que o Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="1ad65-175">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="1ad65-176">Usuários federados e anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="1ad65-176">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="1ad65-177">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="1ad65-177">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="1ad65-178">Todos na mesma empresa que o organizador e as empresas federadas ingressam na reunião diretamente.</span><span class="sxs-lookup"><span data-stu-id="1ad65-178">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="1ad65-179">Usuários anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="1ad65-179">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="1ad65-180">têm</span><span class="sxs-lookup"><span data-stu-id="1ad65-180">everyone</span></span> | <span data-ttu-id="1ad65-181">Qualquer usuário é permitido, o que significa que todos (incluindo usuários anônimos) podem participar da reunião diretamente, sem esperar no lobby.</span><span class="sxs-lookup"><span data-stu-id="1ad65-181">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="1ad65-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ad65-182">JSON representation</span></span>

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
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
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
