---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 888b5d7d60a72ed95cb3e3f6cbb1b6e5407919ab
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962363"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="6edb4-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6edb4-103">onlineMeeting resource type</span></span>

<span data-ttu-id="6edb4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6edb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6edb4-105">Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="6edb4-105">Contains information about the meeting, including the URL used to join a meeting, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="6edb4-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6edb4-106">Methods</span></span>

| <span data-ttu-id="6edb4-107">Método</span><span class="sxs-lookup"><span data-stu-id="6edb4-107">Method</span></span>         | <span data-ttu-id="6edb4-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6edb4-108">Return Type</span></span> | <span data-ttu-id="6edb4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6edb4-109">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="6edb4-110">Criar ReuniãoOnline</span><span class="sxs-lookup"><span data-stu-id="6edb4-110">Create onlineMeeting</span></span>](../api/application-post-onlineMeetings.md) | [<span data-ttu-id="6edb4-111">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6edb4-111">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="6edb4-112">Criar uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="6edb4-112">Create an online meeting.</span></span> |
| [<span data-ttu-id="6edb4-113">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6edb4-113">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="6edb4-114">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6edb4-114">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="6edb4-115">Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** .</span><span class="sxs-lookup"><span data-stu-id="6edb4-115">Read the properties and relationships of an **onlineMeeting** object.</span></span> |
| [<span data-ttu-id="6edb4-116">Criar ou obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6edb4-116">Create or get onlineMeeting</span></span>](../api/onlinemeeting-createorget.md) | [<span data-ttu-id="6edb4-117">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6edb4-117">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="6edb4-118">Criar uma reunião online com uma ID externa personalizada.</span><span class="sxs-lookup"><span data-stu-id="6edb4-118">Create an online meeting with a custom, external ID.</span></span> <span data-ttu-id="6edb4-119">Se a reunião já existir, recupere sua propriedades.</span><span class="sxs-lookup"><span data-stu-id="6edb4-119">If the meeting already exists, retrieve its propertie.</span></span> |

## <a name="properties"></a><span data-ttu-id="6edb4-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6edb4-120">Properties</span></span>

| <span data-ttu-id="6edb4-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6edb4-121">Property</span></span>                  | <span data-ttu-id="6edb4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6edb4-122">Type</span></span>                                                   | <span data-ttu-id="6edb4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6edb4-123">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6edb4-124">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="6edb4-124">autoAdmittedUsers</span></span>         | <span data-ttu-id="6edb4-125">String</span><span class="sxs-lookup"><span data-stu-id="6edb4-125">String</span></span>                                                 | <span data-ttu-id="6edb4-126">A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online.</span><span class="sxs-lookup"><span data-stu-id="6edb4-126">The setting that specifies the type of participants that will automatically be allowed into the online meeting.</span></span> <span data-ttu-id="6edb4-127">Os valores possíveis são: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span><span class="sxs-lookup"><span data-stu-id="6edb4-127">Possible values are: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`.</span></span> <span data-ttu-id="6edb4-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6edb4-128">Read-only.</span></span>|
| <span data-ttu-id="6edb4-129">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="6edb4-129">audioConferencing</span></span>         | [<span data-ttu-id="6edb4-130">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="6edb4-130">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="6edb4-131">As informações de acesso de telefone (discagem) para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="6edb4-131">The phone access (dial-in) information for an online meeting.</span></span> <span data-ttu-id="6edb4-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6edb4-132">Read-only.</span></span> |
| <span data-ttu-id="6edb4-133">chatInfo</span><span class="sxs-lookup"><span data-stu-id="6edb4-133">chatInfo</span></span>                  | [<span data-ttu-id="6edb4-134">chatInfo</span><span class="sxs-lookup"><span data-stu-id="6edb4-134">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="6edb4-135">As informações de chat associadas a esta reunião online.</span><span class="sxs-lookup"><span data-stu-id="6edb4-135">The chat information associated with this online meeting.</span></span> |
| <span data-ttu-id="6edb4-136">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="6edb4-136">creationDateTime</span></span>          | <span data-ttu-id="6edb4-137">DateTime</span><span class="sxs-lookup"><span data-stu-id="6edb4-137">DateTime</span></span>                                               | <span data-ttu-id="6edb4-138">O horário de criação da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="6edb4-138">The meeting creation time in UTC.</span></span> <span data-ttu-id="6edb4-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6edb4-139">Read-only.</span></span> |
| <span data-ttu-id="6edb4-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6edb4-140">startDateTime</span></span>             | <span data-ttu-id="6edb4-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="6edb4-141">DateTime</span></span>                                               | <span data-ttu-id="6edb4-142">A hora de início da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="6edb4-142">The meeting start time in UTC.</span></span> |
| <span data-ttu-id="6edb4-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6edb4-143">endDateTime</span></span>               | <span data-ttu-id="6edb4-144">DateTime</span><span class="sxs-lookup"><span data-stu-id="6edb4-144">DateTime</span></span>                                               | <span data-ttu-id="6edb4-145">A hora de término da reunião em UTC.</span><span class="sxs-lookup"><span data-stu-id="6edb4-145">The meeting end time in UTC.</span></span> |
| <span data-ttu-id="6edb4-146">id</span><span class="sxs-lookup"><span data-stu-id="6edb4-146">id</span></span>                        | <span data-ttu-id="6edb4-147">String</span><span class="sxs-lookup"><span data-stu-id="6edb4-147">String</span></span>                                                 | <span data-ttu-id="6edb4-148">A ID padrão associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="6edb4-148">The default ID associated with the online meeting.</span></span> <span data-ttu-id="6edb4-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6edb4-149">Read-only.</span></span> |
| <span data-ttu-id="6edb4-150">joinWebUrl</span><span class="sxs-lookup"><span data-stu-id="6edb4-150">joinWebUrl</span></span>                   | <span data-ttu-id="6edb4-151">String</span><span class="sxs-lookup"><span data-stu-id="6edb4-151">String</span></span>                                                 | <span data-ttu-id="6edb4-152">A URL de ingresso da reunião online.</span><span class="sxs-lookup"><span data-stu-id="6edb4-152">The join URL of the online meeting.</span></span> <span data-ttu-id="6edb4-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6edb4-153">Read-only.</span></span>|
| <span data-ttu-id="6edb4-154">participantes</span><span class="sxs-lookup"><span data-stu-id="6edb4-154">participants</span></span>              | [<span data-ttu-id="6edb4-155">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="6edb4-155">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="6edb4-156">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="6edb4-156">The participants associated with the online meeting.</span></span>  <span data-ttu-id="6edb4-157">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="6edb4-157">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="6edb4-158">assunto</span><span class="sxs-lookup"><span data-stu-id="6edb4-158">subject</span></span>                   | <span data-ttu-id="6edb4-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6edb4-159">String</span></span>                                                 | <span data-ttu-id="6edb4-160">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="6edb4-160">The subject of the online meeting.</span></span> |
| <span data-ttu-id="6edb4-161">capabilities</span><span class="sxs-lookup"><span data-stu-id="6edb4-161">capabilities</span></span>              | <span data-ttu-id="6edb4-162">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6edb4-162">String collection</span></span>                                      | <span data-ttu-id="6edb4-163">A lista de recursos de reunião.</span><span class="sxs-lookup"><span data-stu-id="6edb4-163">The list of meeting capabilities.</span></span> <span data-ttu-id="6edb4-164">Os valores possíveis são `questionAndAnswer`:.</span><span class="sxs-lookup"><span data-stu-id="6edb4-164">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="6edb4-165">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="6edb4-165">videoTeleconferenceId</span></span>     | <span data-ttu-id="6edb4-166">String</span><span class="sxs-lookup"><span data-stu-id="6edb4-166">String</span></span>                                                 | <span data-ttu-id="6edb4-167">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="6edb4-167">The video teleconferencing ID.</span></span> <span data-ttu-id="6edb4-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6edb4-168">Read-only.</span></span> |
| <span data-ttu-id="6edb4-169">externalId</span><span class="sxs-lookup"><span data-stu-id="6edb4-169">externalId</span></span>                | <span data-ttu-id="6edb4-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6edb4-170">String</span></span>                                                 | <span data-ttu-id="6edb4-171">A ID externa.</span><span class="sxs-lookup"><span data-stu-id="6edb4-171">The external ID.</span></span> <span data-ttu-id="6edb4-172">Uma ID personalizada.</span><span class="sxs-lookup"><span data-stu-id="6edb4-172">A custom ID.</span></span> <span data-ttu-id="6edb4-173">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6edb4-173">Optional.</span></span> |

### <a name="autoadmittedusers-values"></a><span data-ttu-id="6edb4-174">valores de autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="6edb4-174">autoAdmittedUsers values</span></span>
| <span data-ttu-id="6edb4-175">Valor</span><span class="sxs-lookup"><span data-stu-id="6edb4-175">Value</span></span> | <span data-ttu-id="6edb4-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="6edb4-176">Description</span></span>  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6edb4-177">organizer</span><span class="sxs-lookup"><span data-stu-id="6edb4-177">organizer</span></span> | <span data-ttu-id="6edb4-178">Somente o organizador da reunião é admitido diretamente.</span><span class="sxs-lookup"><span data-stu-id="6edb4-178">Only the meeting organizer is admitted directly.</span></span>  <span data-ttu-id="6edb4-179">Todos os outros esperam no lobby, até que seja admitido pelo organizador</span><span class="sxs-lookup"><span data-stu-id="6edb4-179">Everyone else waits in the lobby, until admitted by the organizer</span></span>  |
| <span data-ttu-id="6edb4-180">invitedUsersInCompany</span><span class="sxs-lookup"><span data-stu-id="6edb4-180">invitedUsersInCompany</span></span> | <span data-ttu-id="6edb4-181">O organizador da reunião e os usuários na mesma empresa convidados pelo Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="6edb4-181">The meeting organizer and the users in the same company invited by the organizer join the meeting directly.</span></span>  <span data-ttu-id="6edb4-182">Todos os outros esperam no lobby até que seja admitido.</span><span class="sxs-lookup"><span data-stu-id="6edb4-182">Everyone else waits in lobby until admitted.</span></span>  |
| <span data-ttu-id="6edb4-183">everyoneInCompany</span><span class="sxs-lookup"><span data-stu-id="6edb4-183">everyoneInCompany</span></span> | <span data-ttu-id="6edb4-184">Todos na mesma empresa que o Organizador participam diretamente da reunião.</span><span class="sxs-lookup"><span data-stu-id="6edb4-184">Everyone in the same company as the organizer join the meeting directly.</span></span>  <span data-ttu-id="6edb4-185">Usuários federados e anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="6edb4-185">Federated, anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="6edb4-186">everyoneInSameAndFederatedCompany</span><span class="sxs-lookup"><span data-stu-id="6edb4-186">everyoneInSameAndFederatedCompany</span></span> |  <span data-ttu-id="6edb4-187">Todos na mesma empresa que o organizador e as empresas federadas ingressam na reunião diretamente.</span><span class="sxs-lookup"><span data-stu-id="6edb4-187">Everyone in same company as the organizer and federated companies join the meeting directly.</span></span>  <span data-ttu-id="6edb4-188">Usuários anônimos esperam no lobby até serem admitidos.</span><span class="sxs-lookup"><span data-stu-id="6edb4-188">Anonymous users wait in lobby until admitted.</span></span>  |
| <span data-ttu-id="6edb4-189">têm</span><span class="sxs-lookup"><span data-stu-id="6edb4-189">everyone</span></span> | <span data-ttu-id="6edb4-190">Qualquer usuário é permitido, o que significa que todos (incluindo usuários anônimos) podem participar da reunião diretamente, sem esperar no lobby.</span><span class="sxs-lookup"><span data-stu-id="6edb4-190">Any user is allowed, which means that everyone (including anonymous users) can join the meeting directly without waiting in lobby.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="6edb4-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6edb4-191">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "externalId"
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
