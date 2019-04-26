---
title: tipo de recurso onlineMeeting
description: Captura informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568854"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="38976-103">tipo de recurso onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="38976-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38976-104">Captura informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.</span><span class="sxs-lookup"><span data-stu-id="38976-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="38976-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="38976-105">Methods</span></span>

| <span data-ttu-id="38976-106">Método</span><span class="sxs-lookup"><span data-stu-id="38976-106">Method</span></span>         | <span data-ttu-id="38976-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38976-107">Return Type</span></span> | <span data-ttu-id="38976-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="38976-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="38976-109">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="38976-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="38976-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="38976-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="38976-111">Leia as propriedades e os relacionamentos do objeto onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="38976-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="38976-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38976-112">Properties</span></span>

| <span data-ttu-id="38976-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38976-113">Property</span></span>                  | <span data-ttu-id="38976-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="38976-114">Type</span></span>                                                   | <span data-ttu-id="38976-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="38976-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="38976-116">accessLevel</span><span class="sxs-lookup"><span data-stu-id="38976-116">accessLevel</span></span>               | <span data-ttu-id="38976-117">String</span><span class="sxs-lookup"><span data-stu-id="38976-117">String</span></span>                                                 | <span data-ttu-id="38976-118">O nível de acesso que controla a admissão para a reunião online.</span><span class="sxs-lookup"><span data-stu-id="38976-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="38976-119">Os valores possíveis são: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="38976-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="38976-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="38976-120">audioConferencing</span></span>         | [<span data-ttu-id="38976-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="38976-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="38976-122">Representa as informações de acesso de telefone de um onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="38976-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="38976-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="38976-123">canceledDateTime</span></span>          | <span data-ttu-id="38976-124">DateTime</span><span class="sxs-lookup"><span data-stu-id="38976-124">DateTime</span></span>                                               | <span data-ttu-id="38976-125">A hora em que a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="38976-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="38976-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="38976-126">chatInfo</span></span>                  | [<span data-ttu-id="38976-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="38976-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="38976-128">O chat associado a esta reunião.</span><span class="sxs-lookup"><span data-stu-id="38976-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="38976-129">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="38976-129">creationDateTime</span></span>          | <span data-ttu-id="38976-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="38976-130">DateTime</span></span>                                               | <span data-ttu-id="38976-131">A hora em que a reunião foi criada.</span><span class="sxs-lookup"><span data-stu-id="38976-131">The time when the meeting was created.</span></span> <span data-ttu-id="38976-132">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="38976-132">Readonly.</span></span>
| <span data-ttu-id="38976-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="38976-133">endDateTime</span></span>               | <span data-ttu-id="38976-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="38976-134">DateTime</span></span>                                               | <span data-ttu-id="38976-135">Hora de término da reunião.</span><span class="sxs-lookup"><span data-stu-id="38976-135">End time of the meeting.</span></span> |
| <span data-ttu-id="38976-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="38976-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="38976-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="38976-137">Boolean</span></span>                                                | <span data-ttu-id="38976-138">O status dos comunicados de presença para a reunião online.</span><span class="sxs-lookup"><span data-stu-id="38976-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="38976-139">Quando os comunicados de presença estiverem habilitados, a reunião online anunciará os nomes do participantswho ingressar na reunião por meio de áudio.</span><span class="sxs-lookup"><span data-stu-id="38976-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="38976-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="38976-140">expirationDateTime</span></span>        | <span data-ttu-id="38976-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="38976-141">DateTime</span></span>                                               | <span data-ttu-id="38976-142">A data e a hora UTC (tempo Universal Coordenado) absoluta após a qual a reunião online pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="38976-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="38976-143">O dia e a hora devem estar entre um ano antes e dez anos após, a data e a hora atuais no servidor.</span><span class="sxs-lookup"><span data-stu-id="38976-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="38976-144">id</span><span class="sxs-lookup"><span data-stu-id="38976-144">id</span></span>                        | <span data-ttu-id="38976-145">String</span><span class="sxs-lookup"><span data-stu-id="38976-145">String</span></span>                                                 | <span data-ttu-id="38976-146">A ID associada à reunião online.</span><span class="sxs-lookup"><span data-stu-id="38976-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="38976-147">Usado em uma solicitação HTTP GET como a ID.</span><span class="sxs-lookup"><span data-stu-id="38976-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="38976-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38976-148">Read-only.</span></span> <span data-ttu-id="38976-149">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="38976-149">Server generated.</span></span> |
| <span data-ttu-id="38976-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="38976-150">isCancelled</span></span>               | <span data-ttu-id="38976-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="38976-151">Boolean</span></span>                                                | <span data-ttu-id="38976-152">Se a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="38976-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="38976-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="38976-153">joinUrl</span></span>                   | <span data-ttu-id="38976-154">String</span><span class="sxs-lookup"><span data-stu-id="38976-154">String</span></span>                                                 | <span data-ttu-id="38976-155">A URL que é usada quando a reunião online é associada da Web.</span><span class="sxs-lookup"><span data-stu-id="38976-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="38976-156">meetingtype</span><span class="sxs-lookup"><span data-stu-id="38976-156">meetingType</span></span>               | <span data-ttu-id="38976-157">String</span><span class="sxs-lookup"><span data-stu-id="38976-157">String</span></span>                                                 | <span data-ttu-id="38976-158">Os valores possíveis são `meetNow`: `scheduled`, `recurring`,,`broadcast`</span><span class="sxs-lookup"><span data-stu-id="38976-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="38976-159">participantes</span><span class="sxs-lookup"><span data-stu-id="38976-159">participants</span></span>              | [<span data-ttu-id="38976-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="38976-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="38976-161">Os participantes associados à reunião online.</span><span class="sxs-lookup"><span data-stu-id="38976-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="38976-162">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="38976-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="38976-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="38976-163">startDateTime</span></span>             | <span data-ttu-id="38976-164">DateTime</span><span class="sxs-lookup"><span data-stu-id="38976-164">DateTime</span></span>                                               | <span data-ttu-id="38976-165">Hora de início da reunião.</span><span class="sxs-lookup"><span data-stu-id="38976-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="38976-166">subject</span><span class="sxs-lookup"><span data-stu-id="38976-166">subject</span></span>                   | <span data-ttu-id="38976-167">String</span><span class="sxs-lookup"><span data-stu-id="38976-167">String</span></span>                                                 | <span data-ttu-id="38976-168">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="38976-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="38976-169">Relações</span><span class="sxs-lookup"><span data-stu-id="38976-169">Relationships</span></span>
<span data-ttu-id="38976-170">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38976-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38976-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38976-171">JSON representation</span></span>

<span data-ttu-id="38976-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38976-172">The following is a JSON representation of the resource.</span></span>

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
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
