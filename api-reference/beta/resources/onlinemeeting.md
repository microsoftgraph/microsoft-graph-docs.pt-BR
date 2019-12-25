---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: e7cae71f220a2a519908e3af890029a2da555577
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866683"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="f0426-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f0426-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0426-104">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="f0426-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="f0426-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f0426-105">Methods</span></span>

| <span data-ttu-id="f0426-106">Método</span><span class="sxs-lookup"><span data-stu-id="f0426-106">Method</span></span>         | <span data-ttu-id="f0426-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f0426-107">Return Type</span></span> | <span data-ttu-id="f0426-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0426-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="f0426-109">Criar onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f0426-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="f0426-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f0426-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f0426-111">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="f0426-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="f0426-112">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f0426-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="f0426-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f0426-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f0426-114">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="f0426-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f0426-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0426-115">Properties</span></span>

| <span data-ttu-id="f0426-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0426-116">Property</span></span>                  | <span data-ttu-id="f0426-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0426-117">Type</span></span>                                                   | <span data-ttu-id="f0426-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0426-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f0426-119">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="f0426-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="f0426-120">String</span><span class="sxs-lookup"><span data-stu-id="f0426-120">String</span></span>                                                 | <span data-ttu-id="f0426-121">A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online.</span><span class="sxs-lookup"><span data-stu-id="f0426-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="f0426-122">Os valores possíveis são: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span><span class="sxs-lookup"><span data-stu-id="f0426-122">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="f0426-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0426-123">Read-only.</span></span>|
| <span data-ttu-id="f0426-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="f0426-124">audioConferencing</span></span>         | [<span data-ttu-id="f0426-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="f0426-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="f0426-126">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="f0426-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="f0426-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0426-127">Read-only.</span></span> |
| <span data-ttu-id="f0426-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f0426-128">chatInfo</span></span>                  | [<span data-ttu-id="f0426-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f0426-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="f0426-130">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="f0426-130">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="f0426-131">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="f0426-131">creationDateTime</span></span>          | <span data-ttu-id="f0426-132">DateTime</span><span class="sxs-lookup"><span data-stu-id="f0426-132">DateTime</span></span>                                               | <span data-ttu-id="f0426-133">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="f0426-133">The meeting creation time in UTC.</span></span> <span data-ttu-id="f0426-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0426-134">Read-only.</span></span> |
| <span data-ttu-id="f0426-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f0426-135">startDateTime</span></span>             | <span data-ttu-id="f0426-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="f0426-136">DateTime</span></span>                                               | <span data-ttu-id="f0426-137">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="f0426-137">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="f0426-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f0426-138">endDateTime</span></span>               | <span data-ttu-id="f0426-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="f0426-139">DateTime</span></span>                                               | <span data-ttu-id="f0426-140">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="f0426-140">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="f0426-141">id</span><span class="sxs-lookup"><span data-stu-id="f0426-141">id</span></span>                        | <span data-ttu-id="f0426-142">String</span><span class="sxs-lookup"><span data-stu-id="f0426-142">String</span></span>                                                 | <span data-ttu-id="f0426-143">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="f0426-143">The default ID associated with the online meeting.</span></span> <span data-ttu-id="f0426-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0426-144">Read-only.</span></span> |
| <span data-ttu-id="f0426-145">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="f0426-145">joinWebUrl</span></span>                   | <span data-ttu-id="f0426-146">String</span><span class="sxs-lookup"><span data-stu-id="f0426-146">String</span></span>                                                 | <span data-ttu-id="f0426-147">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="f0426-147">The join URL of the online meeting.</span></span> <span data-ttu-id="f0426-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0426-148">Read-only.</span></span>|
| <span data-ttu-id="f0426-149">participants</span><span class="sxs-lookup"><span data-stu-id="f0426-149">participants</span></span>              | [<span data-ttu-id="f0426-150">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="f0426-150">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="f0426-151">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="f0426-151">The participants associated with the online meeting.</span></span>  <span data-ttu-id="f0426-152">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="f0426-152">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="f0426-153">subject</span><span class="sxs-lookup"><span data-stu-id="f0426-153">subject</span></span>                   | <span data-ttu-id="f0426-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0426-154">String</span></span>                                                 | <span data-ttu-id="f0426-155">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="f0426-155">The subject of the online meeting.</span></span> |
| <span data-ttu-id="f0426-156">capabilities</span><span class="sxs-lookup"><span data-stu-id="f0426-156">capabilities</span></span>              | <span data-ttu-id="f0426-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0426-157">String collection</span></span>                                      | <span data-ttu-id="f0426-158">A lista de recursos de reunião.</span><span class="sxs-lookup"><span data-stu-id="f0426-158">The list of meeting capabilities.</span></span> <span data-ttu-id="f0426-159">Os valores possíveis são `questionAndAnswer`:.</span><span class="sxs-lookup"><span data-stu-id="f0426-159">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="f0426-160">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="f0426-160">videoTeleconferenceId</span></span>     | <span data-ttu-id="f0426-161">String</span><span class="sxs-lookup"><span data-stu-id="f0426-161">String</span></span>                                                 | <span data-ttu-id="f0426-162">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="f0426-162">The video teleconferencing ID.</span></span> <span data-ttu-id="f0426-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0426-163">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="f0426-164">valores de autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="f0426-164">autoAdmittedUsers values</span></span>
| <span data-ttu-id="f0426-165">Valor</span><span class="sxs-lookup"><span data-stu-id="f0426-165">Value</span></span> | <span data-ttu-id="f0426-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0426-166">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f0426-167">organizer</span><span class="sxs-lookup"><span data-stu-id="f0426-167">organizer</span></span> | <span data-ttu-id="f0426-168">Somente o organizador da reunião é admitido diretamente.</span><span class="sxs-lookup"><span data-stu-id="f0426-168">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="f0426-169">Todos os outros esperam no lobby, até que seja admitido pelo organizador</span><span class="sxs-lookup"><span data-stu-id="f0426-169">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="f0426-170">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="f0426-170">invitedUsersInCompany</span></span> | <span data-ttu-id="f0426-171">O organizador da reunião e os usuários na mesma empresa convidados pelo Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="f0426-171">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="f0426-172">Todos os outros esperam no lobby até que seja admitido.</span><span class="sxs-lookup"><span data-stu-id="f0426-172">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="f0426-173">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="f0426-173">everyoneInCompany</span></span> | <span data-ttu-id="f0426-174">Todos na mesma empresa que o Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="f0426-174">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="f0426-175">Usuários federados e anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="f0426-175">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="f0426-176">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="f0426-176">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="f0426-177">Todos na mesma empresa que o organizador e as empresas federadas ingressam na reunião diretamente.</span><span class="sxs-lookup"><span data-stu-id="f0426-177">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="f0426-178">Usuários anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="f0426-178">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="f0426-179">têm</span><span class="sxs-lookup"><span data-stu-id="f0426-179">everyone</span></span> | <span data-ttu-id="f0426-180">Qualquer usuário é permitido, o que significa que todos (incluindo usuários anônimos) podem participar da reunião diretamente, sem esperar no lobby.</span><span class="sxs-lookup"><span data-stu-id="f0426-180">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="f0426-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0426-181">JSON representation</span></span>

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
