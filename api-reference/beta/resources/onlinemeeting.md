---
title: tipo de recurso de onlineMeeting
description: Informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição de captura.
author: VinodRavichandran
ms.openlocfilehash: 3a2b26ac212bd7a77428dab9f5618db8165de65b
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380475"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="7e7c4-103">tipo de recurso de onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7e7c4-103">onlineMeeting resource type</span></span>

> <span data-ttu-id="7e7c4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e7c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e7c4-106">Informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição de captura.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-106">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="7e7c4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7e7c4-107">Methods</span></span>

| <span data-ttu-id="7e7c4-108">Método		</span><span class="sxs-lookup"><span data-stu-id="7e7c4-108">Method</span></span>         | <span data-ttu-id="7e7c4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7e7c4-109">Return Type</span></span> | <span data-ttu-id="7e7c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e7c4-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="7e7c4-111">Obter onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7e7c4-111">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="7e7c4-112">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7e7c4-112">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="7e7c4-113">Leia as propriedades e os relacionamentos do objeto onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-113">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7e7c4-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e7c4-114">Properties</span></span>

| <span data-ttu-id="7e7c4-115">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="7e7c4-115">Property</span></span>                  | <span data-ttu-id="7e7c4-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e7c4-116">Type</span></span>                                                   | <span data-ttu-id="7e7c4-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e7c4-117">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7e7c4-118">accessLevel</span><span class="sxs-lookup"><span data-stu-id="7e7c4-118">accessLevel</span></span>               | <span data-ttu-id="7e7c4-119">String</span><span class="sxs-lookup"><span data-stu-id="7e7c4-119">String</span></span>                                                 | <span data-ttu-id="7e7c4-120">O nível de acesso que controla a admissão na reunião online.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-120">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="7e7c4-121">Os valores possíveis são: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-121">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="7e7c4-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="7e7c4-122">audioConferencing</span></span>         | [<span data-ttu-id="7e7c4-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="7e7c4-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="7e7c4-124">Representa as informações de acesso telefônicas de um onlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-124">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="7e7c4-125">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-125">canceledDateTime</span></span>          | <span data-ttu-id="7e7c4-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-126">DateTime</span></span>                                               | <span data-ttu-id="7e7c4-127">A hora de quando a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-127">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="7e7c4-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="7e7c4-128">chatInfo</span></span>                  | [<span data-ttu-id="7e7c4-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="7e7c4-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="7e7c4-130">O chat associado a esta reunião.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-130">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="7e7c4-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-131">creationDateTime</span></span>          | <span data-ttu-id="7e7c4-132">DateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-132">DateTime</span></span>                                               | <span data-ttu-id="7e7c4-133">A hora em que a reunião foi criada.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-133">The time when the meeting was created.</span></span> <span data-ttu-id="7e7c4-134">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-134">Readonly.</span></span>
| <span data-ttu-id="7e7c4-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-135">endDateTime</span></span>               | <span data-ttu-id="7e7c4-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-136">DateTime</span></span>                                               | <span data-ttu-id="7e7c4-137">Hora de término da reunião.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-137">End time of the meeting.</span></span> |
| <span data-ttu-id="7e7c4-138">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="7e7c4-138">entryExitAnnouncement</span></span>     | <span data-ttu-id="7e7c4-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e7c4-139">Boolean</span></span>                                                | <span data-ttu-id="7e7c4-140">O status de comunicados de participação da reunião online.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-140">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="7e7c4-141">Quando os anúncios de presença estão habilitados, a reunião online lançará os nomes dos participantswho ingressar na reunião através do áudio.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-141">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="7e7c4-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-142">expirationDateTime</span></span>        | <span data-ttu-id="7e7c4-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-143">DateTime</span></span>                                               | <span data-ttu-id="7e7c4-144">A data de tempo Universal Coordenado (UTC) e a hora após o qual a absoluto da reunião online pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-144">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="7e7c4-145">O dia e hora devem estar entre um ano antes e dez anos após a data atual e a hora no servidor.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-145">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="7e7c4-146">id</span><span class="sxs-lookup"><span data-stu-id="7e7c4-146">id</span></span>                        | <span data-ttu-id="7e7c4-147">String</span><span class="sxs-lookup"><span data-stu-id="7e7c4-147">String</span></span>                                                 | <span data-ttu-id="7e7c4-148">A ID associada a reunião online.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-148">The ID associated with the online meeting.</span></span> <span data-ttu-id="7e7c4-149">Usado em uma solicitação HTTP GET, como a ID.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-149">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="7e7c4-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-150">Read-only.</span></span> <span data-ttu-id="7e7c4-151">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-151">Server generated.</span></span> |
| <span data-ttu-id="7e7c4-152">isCancelled</span><span class="sxs-lookup"><span data-stu-id="7e7c4-152">isCancelled</span></span>               | <span data-ttu-id="7e7c4-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="7e7c4-153">Boolean</span></span>                                                | <span data-ttu-id="7e7c4-154">Se a reunião foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-154">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="7e7c4-155">joinUrl</span><span class="sxs-lookup"><span data-stu-id="7e7c4-155">joinUrl</span></span>                   | <span data-ttu-id="7e7c4-156">String</span><span class="sxs-lookup"><span data-stu-id="7e7c4-156">String</span></span>                                                 | <span data-ttu-id="7e7c4-157">A URL que é usada durante a reunião online está unida a partir da web.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-157">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="7e7c4-158">meetingType</span><span class="sxs-lookup"><span data-stu-id="7e7c4-158">meetingType</span></span>               | <span data-ttu-id="7e7c4-159">String</span><span class="sxs-lookup"><span data-stu-id="7e7c4-159">String</span></span>                                                 | <span data-ttu-id="7e7c4-160">Os valores possíveis são: `meetNow`, `scheduled`, `recurring`,`broadcast`</span><span class="sxs-lookup"><span data-stu-id="7e7c4-160">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="7e7c4-161">participantes</span><span class="sxs-lookup"><span data-stu-id="7e7c4-161">participants</span></span>              | [<span data-ttu-id="7e7c4-162">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="7e7c4-162">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="7e7c4-163">Os participantes associados a reunião online.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-163">The participants associated with the online meeting.</span></span>  <span data-ttu-id="7e7c4-164">Isso inclui o organizador e os participantes.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-164">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="7e7c4-165">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-165">startDateTime</span></span>             | <span data-ttu-id="7e7c4-166">DateTime</span><span class="sxs-lookup"><span data-stu-id="7e7c4-166">DateTime</span></span>                                               | <span data-ttu-id="7e7c4-167">Inicie o horário da reunião.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-167">Start time of the meeting.</span></span> |
| <span data-ttu-id="7e7c4-168">subject</span><span class="sxs-lookup"><span data-stu-id="7e7c4-168">subject</span></span>                   | <span data-ttu-id="7e7c4-169">String</span><span class="sxs-lookup"><span data-stu-id="7e7c4-169">String</span></span>                                                 | <span data-ttu-id="7e7c4-170">O assunto da reunião online.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-170">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7e7c4-171">Relações</span><span class="sxs-lookup"><span data-stu-id="7e7c4-171">Relationships</span></span>
<span data-ttu-id="7e7c4-172">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e7c4-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e7c4-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e7c4-173">JSON representation</span></span>

<span data-ttu-id="7e7c4-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e7c4-174">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
