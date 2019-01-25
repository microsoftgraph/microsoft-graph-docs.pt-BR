---
title: tipo de recurso de onlineMeeting
description: Informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição de captura.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519595"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="476f8-103">tipo de recurso de onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="476f8-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="476f8-104">Informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição de captura.</span><span class="sxs-lookup"><span data-stu-id="476f8-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="476f8-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="476f8-105">Methods</span></span>

| <span data-ttu-id="476f8-106">Método</span><span class="sxs-lookup"><span data-stu-id="476f8-106">Method</span></span>         | <span data-ttu-id="476f8-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="476f8-107">Return Type</span></span> | <span data-ttu-id="476f8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="476f8-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="476f8-109">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="476f8-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="476f8-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="476f8-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="476f8-111">Leia as propriedades e os relacionamentos do objeto onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="476f8-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="476f8-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="476f8-112">Properties</span></span>

| <span data-ttu-id="476f8-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="476f8-113">Property</span></span>                  | <span data-ttu-id="476f8-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="476f8-114">Type</span></span>                                                   | <span data-ttu-id="476f8-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="476f8-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="476f8-116">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="476f8-116">accessLevel</span></span>               | <span data-ttu-id="476f8-117">String</span><span class="sxs-lookup"><span data-stu-id="476f8-117">String</span></span>                                                 | <span data-ttu-id="476f8-118">O nível de acesso que controla a admissão na reunião online.</span><span class="sxs-lookup"><span data-stu-id="476f8-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="476f8-119">Os valores possíveis são: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="476f8-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="476f8-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="476f8-120">audioConferencing</span></span>         | [<span data-ttu-id="476f8-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="476f8-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="476f8-122">Representa as informações de acesso telefônicas de um onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="476f8-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="476f8-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-123">canceledDateTime</span></span>          | <span data-ttu-id="476f8-124">DateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-124">DateTime</span></span>                                               | <span data-ttu-id="476f8-125">A hora de quando a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="476f8-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="476f8-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="476f8-126">chatInfo</span></span>                  | [<span data-ttu-id="476f8-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="476f8-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="476f8-128">O chat associado a esta reunião.</span><span class="sxs-lookup"><span data-stu-id="476f8-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="476f8-129">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-129">creationDateTime</span></span>          | <span data-ttu-id="476f8-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-130">DateTime</span></span>                                               | <span data-ttu-id="476f8-131">A hora em que a reunião foi criada.</span><span class="sxs-lookup"><span data-stu-id="476f8-131">The time when the meeting was created.</span></span> <span data-ttu-id="476f8-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="476f8-132">Readonly.</span></span>
| <span data-ttu-id="476f8-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-133">endDateTime</span></span>               | <span data-ttu-id="476f8-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-134">DateTime</span></span>                                               | <span data-ttu-id="476f8-135">Hora de término da reunião.</span><span class="sxs-lookup"><span data-stu-id="476f8-135">End time of the meeting.</span></span> |
| <span data-ttu-id="476f8-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="476f8-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="476f8-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="476f8-137">Boolean</span></span>                                                | <span data-ttu-id="476f8-138">O status de comunicados de participação da reunião online.</span><span class="sxs-lookup"><span data-stu-id="476f8-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="476f8-139">Quando os anúncios de presença estão habilitados, a reunião online lançará os nomes dos participantswho ingressar na reunião através do áudio.</span><span class="sxs-lookup"><span data-stu-id="476f8-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="476f8-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-140">expirationDateTime</span></span>        | <span data-ttu-id="476f8-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-141">DateTime</span></span>                                               | <span data-ttu-id="476f8-142">A data de tempo Universal Coordenado (UTC) e a hora após o qual a absoluto da reunião online pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="476f8-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="476f8-143">O dia e hora devem estar entre um ano antes e dez anos após a data atual e a hora no servidor.</span><span class="sxs-lookup"><span data-stu-id="476f8-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="476f8-144">id</span><span class="sxs-lookup"><span data-stu-id="476f8-144">id</span></span>                        | <span data-ttu-id="476f8-145">String</span><span class="sxs-lookup"><span data-stu-id="476f8-145">String</span></span>                                                 | <span data-ttu-id="476f8-146">A ID associada a reunião online.</span><span class="sxs-lookup"><span data-stu-id="476f8-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="476f8-147">Usado em uma solicitação HTTP GET, como a ID.</span><span class="sxs-lookup"><span data-stu-id="476f8-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="476f8-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="476f8-148">Read-only.</span></span> <span data-ttu-id="476f8-149">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="476f8-149">Server generated.</span></span> |
| <span data-ttu-id="476f8-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="476f8-150">isCancelled</span></span>               | <span data-ttu-id="476f8-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="476f8-151">Boolean</span></span>                                                | <span data-ttu-id="476f8-152">Se a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="476f8-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="476f8-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="476f8-153">joinUrl</span></span>                   | <span data-ttu-id="476f8-154">String</span><span class="sxs-lookup"><span data-stu-id="476f8-154">String</span></span>                                                 | <span data-ttu-id="476f8-155">A URL que é usada durante a reunião online está unida a partir da web.</span><span class="sxs-lookup"><span data-stu-id="476f8-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="476f8-156">meetingType</span><span class="sxs-lookup"><span data-stu-id="476f8-156">meetingType</span></span>               | <span data-ttu-id="476f8-157">String</span><span class="sxs-lookup"><span data-stu-id="476f8-157">String</span></span>                                                 | <span data-ttu-id="476f8-158">Os valores possíveis são: `meetNow`, `scheduled`, `recurring`.</span><span class="sxs-lookup"><span data-stu-id="476f8-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="476f8-159">participantes</span><span class="sxs-lookup"><span data-stu-id="476f8-159">participants</span></span>              | [<span data-ttu-id="476f8-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="476f8-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="476f8-161">Os participantes associados a reunião online.</span><span class="sxs-lookup"><span data-stu-id="476f8-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="476f8-162">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="476f8-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="476f8-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-163">startDateTime</span></span>             | <span data-ttu-id="476f8-164">DateTime</span><span class="sxs-lookup"><span data-stu-id="476f8-164">DateTime</span></span>                                               | <span data-ttu-id="476f8-165">Inicie o horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="476f8-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="476f8-166">subject</span><span class="sxs-lookup"><span data-stu-id="476f8-166">subject</span></span>                   | <span data-ttu-id="476f8-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="476f8-167">String</span></span>                                                 | <span data-ttu-id="476f8-168">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="476f8-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="476f8-169">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="476f8-169">Relationships</span></span>
<span data-ttu-id="476f8-170">Nenhum</span><span class="sxs-lookup"><span data-stu-id="476f8-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="476f8-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="476f8-171">JSON representation</span></span>

<span data-ttu-id="476f8-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="476f8-172">The following is a JSON representation of the resource.</span></span>

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
