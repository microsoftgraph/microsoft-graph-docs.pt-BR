---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 5d86df3bde56e242559e224cc27921d162be7bf4
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913412"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="ae71d-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ae71d-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae71d-104">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="ae71d-104">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="ae71d-105">Methods</span><span class="sxs-lookup"><span data-stu-id="ae71d-105">Methods</span></span>

| <span data-ttu-id="ae71d-106">Método</span><span class="sxs-lookup"><span data-stu-id="ae71d-106">Method</span></span>         | <span data-ttu-id="ae71d-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ae71d-107">Return Type</span></span> | <span data-ttu-id="ae71d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae71d-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="ae71d-109">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="ae71d-109">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="ae71d-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ae71d-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ae71d-111">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae71d-111">Create an online meeting.</span></span> |
| [<span data-ttu-id="ae71d-112">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ae71d-112">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="ae71d-113">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="ae71d-113">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="ae71d-114">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="ae71d-114">Read the properties and relationships of an **onlineMeeting** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae71d-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae71d-115">Properties</span></span>

| <span data-ttu-id="ae71d-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae71d-116">Property</span></span>                  | <span data-ttu-id="ae71d-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae71d-117">Type</span></span>                                                   | <span data-ttu-id="ae71d-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae71d-118">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ae71d-119">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="ae71d-119">autoAdmittedUsers</span></span>         | <span data-ttu-id="ae71d-120">String</span><span class="sxs-lookup"><span data-stu-id="ae71d-120">String</span></span>                                                 | <span data-ttu-id="ae71d-121">A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae71d-121">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="ae71d-122">Os valores possíveis são: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span><span class="sxs-lookup"><span data-stu-id="ae71d-122">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="ae71d-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae71d-123">Read-only.</span></span>|
| <span data-ttu-id="ae71d-124">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="ae71d-124">audioConferencing</span></span>         | [<span data-ttu-id="ae71d-125">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="ae71d-125">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="ae71d-126">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae71d-126">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="ae71d-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae71d-127">Read-only.</span></span> |
| <span data-ttu-id="ae71d-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="ae71d-128">chatInfo</span></span>                  | [<span data-ttu-id="ae71d-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="ae71d-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="ae71d-130">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae71d-130">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="ae71d-131">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="ae71d-131">creationDateTime</span></span>          | <span data-ttu-id="ae71d-132">DateTime</span><span class="sxs-lookup"><span data-stu-id="ae71d-132">DateTime</span></span>                                               | <span data-ttu-id="ae71d-133">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="ae71d-133">The meeting creation time in UTC.</span></span> <span data-ttu-id="ae71d-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae71d-134">Read-only.</span></span> |
| <span data-ttu-id="ae71d-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ae71d-135">startDateTime</span></span>             | <span data-ttu-id="ae71d-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="ae71d-136">DateTime</span></span>                                               | <span data-ttu-id="ae71d-137">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="ae71d-137">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="ae71d-138">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ae71d-138">endDateTime</span></span>               | <span data-ttu-id="ae71d-139">DateTime</span><span class="sxs-lookup"><span data-stu-id="ae71d-139">DateTime</span></span>                                               | <span data-ttu-id="ae71d-140">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="ae71d-140">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="ae71d-141">id</span><span class="sxs-lookup"><span data-stu-id="ae71d-141">id</span></span>                        | <span data-ttu-id="ae71d-142">String</span><span class="sxs-lookup"><span data-stu-id="ae71d-142">String</span></span>                                                 | <span data-ttu-id="ae71d-143">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae71d-143">The default ID associated with the online meeting.</span></span> <span data-ttu-id="ae71d-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae71d-144">Read-only.</span></span> |
| <span data-ttu-id="ae71d-145">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="ae71d-145">joinWebUrl</span></span>                   | <span data-ttu-id="ae71d-146">String</span><span class="sxs-lookup"><span data-stu-id="ae71d-146">String</span></span>                                                 | <span data-ttu-id="ae71d-147">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae71d-147">The join URL of the online meeting.</span></span> <span data-ttu-id="ae71d-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae71d-148">Read-only.</span></span>|
| <span data-ttu-id="ae71d-149">participants</span><span class="sxs-lookup"><span data-stu-id="ae71d-149">participants</span></span>              | [<span data-ttu-id="ae71d-150">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="ae71d-150">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="ae71d-151">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae71d-151">The participants associated with the online meeting.</span></span>  <span data-ttu-id="ae71d-152">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="ae71d-152">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="ae71d-153">assunto</span><span class="sxs-lookup"><span data-stu-id="ae71d-153">subject</span></span>                   | <span data-ttu-id="ae71d-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae71d-154">String</span></span>                                                 | <span data-ttu-id="ae71d-155">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="ae71d-155">The subject of the online meeting.</span></span> |
| <span data-ttu-id="ae71d-156">capabilities</span><span class="sxs-lookup"><span data-stu-id="ae71d-156">capabilities</span></span>              | <span data-ttu-id="ae71d-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae71d-157">String collection</span></span>                                      | <span data-ttu-id="ae71d-158">A lista de recursos de reunião.</span><span class="sxs-lookup"><span data-stu-id="ae71d-158">The list of meeting capabilities.</span></span> <span data-ttu-id="ae71d-159">Os valores possíveis são `questionAndAnswer`:.</span><span class="sxs-lookup"><span data-stu-id="ae71d-159">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="ae71d-160">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="ae71d-160">videoTeleconferenceId</span></span>     | <span data-ttu-id="ae71d-161">String</span><span class="sxs-lookup"><span data-stu-id="ae71d-161">String</span></span>                                                 | <span data-ttu-id="ae71d-162">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="ae71d-162">The video teleconferencing ID.</span></span> <span data-ttu-id="ae71d-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae71d-163">Read-only.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="ae71d-164">valores de autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="ae71d-164">autoAdmittedUsers values</span></span>
| <span data-ttu-id="ae71d-165">Valor</span><span class="sxs-lookup"><span data-stu-id="ae71d-165">Value</span></span> | <span data-ttu-id="ae71d-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae71d-166">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ae71d-167">organizer</span><span class="sxs-lookup"><span data-stu-id="ae71d-167">organizer</span></span> | <span data-ttu-id="ae71d-168">Somente o organizador da reunião é admitido diretamente.</span><span class="sxs-lookup"><span data-stu-id="ae71d-168">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="ae71d-169">Todos os outros esperam no lobby, até que seja admitido pelo organizador</span><span class="sxs-lookup"><span data-stu-id="ae71d-169">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="ae71d-170">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="ae71d-170">invitedUsersInCompany</span></span> | <span data-ttu-id="ae71d-171">O organizador da reunião e os usuários na mesma empresa convidados pelo Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="ae71d-171">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="ae71d-172">Todos os outros esperam no lobby até que seja admitido.</span><span class="sxs-lookup"><span data-stu-id="ae71d-172">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="ae71d-173">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="ae71d-173">everyoneInCompany</span></span> | <span data-ttu-id="ae71d-174">Todos na mesma empresa que o Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="ae71d-174">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="ae71d-175">Usuários federados e anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="ae71d-175">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="ae71d-176">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="ae71d-176">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="ae71d-177">Todos na mesma empresa que o organizador e as empresas federadas ingressam na reunião diretamente.</span><span class="sxs-lookup"><span data-stu-id="ae71d-177">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="ae71d-178">Usuários anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="ae71d-178">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="ae71d-179">têm</span><span class="sxs-lookup"><span data-stu-id="ae71d-179">everyone</span></span> | <span data-ttu-id="ae71d-180">Qualquer usuário é permitido, o que significa que todos (incluindo usuários anônimos) podem participar da reunião diretamente, sem esperar no lobby.</span><span class="sxs-lookup"><span data-stu-id="ae71d-180">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="ae71d-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae71d-181">JSON representation</span></span>

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
