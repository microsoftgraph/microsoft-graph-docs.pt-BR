---
title: tipo de recurso onlineMeeting
description: Captura informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 611731673d932d6c5135c0115d735e4d642b1bfe
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792783"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="f7945-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f7945-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7945-104">Captura informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="f7945-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="f7945-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f7945-105">Methods</span></span>

| <span data-ttu-id="f7945-106">Método</span><span class="sxs-lookup"><span data-stu-id="f7945-106">Method</span></span>         | <span data-ttu-id="f7945-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f7945-107">Return Type</span></span> | <span data-ttu-id="f7945-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7945-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="f7945-109">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f7945-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="f7945-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f7945-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="f7945-111">Leia as propriedades e os relacionamentos do objeto onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="f7945-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7945-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7945-112">Properties</span></span>

| <span data-ttu-id="f7945-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7945-113">Property</span></span>                  | <span data-ttu-id="f7945-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7945-114">Type</span></span>                                                   | <span data-ttu-id="f7945-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7945-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f7945-116">accessLevel</span><span class="sxs-lookup"><span data-stu-id="f7945-116">accessLevel</span></span>               | <span data-ttu-id="f7945-117">String</span><span class="sxs-lookup"><span data-stu-id="f7945-117">String</span></span>                                                 | <span data-ttu-id="f7945-118">O nível de acesso que controla a admissão para a reunião online.</span><span class="sxs-lookup"><span data-stu-id="f7945-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="f7945-119">Os valores possíveis são: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f7945-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="f7945-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="f7945-120">audioConferencing</span></span>         | [<span data-ttu-id="f7945-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="f7945-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="f7945-122">Representa as informações de acesso de telefone de um onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="f7945-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="f7945-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-123">canceledDateTime</span></span>          | <span data-ttu-id="f7945-124">DateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-124">DateTime</span></span>                                               | <span data-ttu-id="f7945-125">A hora em que a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="f7945-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="f7945-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f7945-126">chatInfo</span></span>                  | [<span data-ttu-id="f7945-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="f7945-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="f7945-128">O chat associado a esta reunião.</span><span class="sxs-lookup"><span data-stu-id="f7945-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="f7945-129">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="f7945-129">creationDateTime</span></span>          | <span data-ttu-id="f7945-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-130">DateTime</span></span>                                               | <span data-ttu-id="f7945-131">A hora em que a reunião foi criada.</span><span class="sxs-lookup"><span data-stu-id="f7945-131">The time when the meeting was created.</span></span> <span data-ttu-id="f7945-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7945-132">Read-only.</span></span>
| <span data-ttu-id="f7945-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-133">endDateTime</span></span>               | <span data-ttu-id="f7945-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-134">DateTime</span></span>                                               | <span data-ttu-id="f7945-135">Hora de término da reunião.</span><span class="sxs-lookup"><span data-stu-id="f7945-135">End time of the meeting.</span></span> |
| <span data-ttu-id="f7945-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="f7945-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="f7945-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7945-137">Boolean</span></span>                                                | <span data-ttu-id="f7945-138">O status dos comunicados de presença para a reunião online.</span><span class="sxs-lookup"><span data-stu-id="f7945-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="f7945-139">Quando os comunicados de presença estiverem habilitados, a reunião online anunciará os nomes dos participantes que ingressarem na reunião por meio de áudio.</span><span class="sxs-lookup"><span data-stu-id="f7945-139">When attendance announcements are enabled, the online meeting will announce the names of the participants who join the meeting through audio.</span></span> |
| <span data-ttu-id="f7945-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-140">expirationDateTime</span></span>        | <span data-ttu-id="f7945-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-141">DateTime</span></span>                                               | <span data-ttu-id="f7945-142">A data e a hora UTC (tempo Universal Coordenado) absoluta após a qual a reunião online pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="f7945-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="f7945-143">O dia e a hora devem estar entre um ano antes e dez anos após, a data e a hora atuais no servidor.</span><span class="sxs-lookup"><span data-stu-id="f7945-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="f7945-144">id</span><span class="sxs-lookup"><span data-stu-id="f7945-144">id</span></span>                        | <span data-ttu-id="f7945-145">String</span><span class="sxs-lookup"><span data-stu-id="f7945-145">String</span></span>                                                 | <span data-ttu-id="f7945-146">A ID associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="f7945-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="f7945-147">Usado em uma solicitação HTTP GET como a ID.</span><span class="sxs-lookup"><span data-stu-id="f7945-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="f7945-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7945-148">Read-only.</span></span> <span data-ttu-id="f7945-149">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="f7945-149">Server generated.</span></span> |
| <span data-ttu-id="f7945-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="f7945-150">isCancelled</span></span>               | <span data-ttu-id="f7945-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7945-151">Boolean</span></span>                                                | <span data-ttu-id="f7945-152">Se a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="f7945-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="f7945-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="f7945-153">joinUrl</span></span>                   | <span data-ttu-id="f7945-154">String</span><span class="sxs-lookup"><span data-stu-id="f7945-154">String</span></span>                                                 | <span data-ttu-id="f7945-155">A URL que é usada quando a reunião online é associada da Web.</span><span class="sxs-lookup"><span data-stu-id="f7945-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="f7945-156">meetingtype</span><span class="sxs-lookup"><span data-stu-id="f7945-156">meetingType</span></span>               | <span data-ttu-id="f7945-157">String</span><span class="sxs-lookup"><span data-stu-id="f7945-157">String</span></span>                                                 | <span data-ttu-id="f7945-158">Os valores possíveis são `meetNow`: `scheduled`, `recurring`, `broadcast` , (Observação: a [criação](../api/application-post-onlinemeetings.md) de `meetNow`onlineMeeting só oferece suporte).</span><span class="sxs-lookup"><span data-stu-id="f7945-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast` (Note: [create onlineMeeting](../api/application-post-onlinemeetings.md) only supports `meetNow`).</span></span> |
| <span data-ttu-id="f7945-159">participants</span><span class="sxs-lookup"><span data-stu-id="f7945-159">participants</span></span>              | [<span data-ttu-id="f7945-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="f7945-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="f7945-161">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="f7945-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="f7945-162">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="f7945-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="f7945-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-163">startDateTime</span></span>             | <span data-ttu-id="f7945-164">DateTime</span><span class="sxs-lookup"><span data-stu-id="f7945-164">DateTime</span></span>                                               | <span data-ttu-id="f7945-165">Hora de início da reunião.</span><span class="sxs-lookup"><span data-stu-id="f7945-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="f7945-166">subject</span><span class="sxs-lookup"><span data-stu-id="f7945-166">subject</span></span>                   | <span data-ttu-id="f7945-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7945-167">String</span></span>                                                 | <span data-ttu-id="f7945-168">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="f7945-168">The subject of the online meeting.</span></span> |
| <span data-ttu-id="f7945-169">capabilities</span><span class="sxs-lookup"><span data-stu-id="f7945-169">capabilities</span></span>              | <span data-ttu-id="f7945-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7945-170">String collection</span></span>                                      | <span data-ttu-id="f7945-171">A lista de recursos de reunião.</span><span class="sxs-lookup"><span data-stu-id="f7945-171">The list of meeting capabilities.</span></span> <span data-ttu-id="f7945-172">Os valores possíveis são `questionAndAnswer`:.</span><span class="sxs-lookup"><span data-stu-id="f7945-172">Possible values are: `questionAndAnswer`.</span></span> |
| <span data-ttu-id="f7945-173">videoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="f7945-173">videoTeleconferenceId</span></span>     | <span data-ttu-id="f7945-174">String</span><span class="sxs-lookup"><span data-stu-id="f7945-174">String</span></span>                                                 | <span data-ttu-id="f7945-175">A ID de teleconferência de vídeo.</span><span class="sxs-lookup"><span data-stu-id="f7945-175">The video teleconferencing id.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f7945-176">Relações</span><span class="sxs-lookup"><span data-stu-id="f7945-176">Relationships</span></span>
<span data-ttu-id="f7945-177">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7945-177">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7945-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7945-178">JSON representation</span></span>

<span data-ttu-id="f7945-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7945-179">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
  "videoTeleconferenceId": "String"
}
```