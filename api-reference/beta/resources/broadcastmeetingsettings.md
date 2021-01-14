---
title: Tipo de recurso broadcastMeetingSettings
description: Configurações relacionadas a um evento ao vivo
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42ac666817b6f259dd888e479939216fc3e39c6c
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866246"
---
# <a name="broadcastmeetingsettings-resource-type"></a><span data-ttu-id="da45d-103">Tipo de recurso broadcastMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="da45d-103">broadcastMeetingSettings resource type</span></span>

<span data-ttu-id="da45d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da45d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da45d-105">Configurações relacionadas a um evento ao vivo.</span><span class="sxs-lookup"><span data-stu-id="da45d-105">Settings related to a live event.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="da45d-106">Essa API não valida configurações de eventos ao vivo gerenciadas por [política.](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="da45d-106">This API does not validate live event settings that are managed by [policy](/microsoftteams/teams-live-events/set-teams-live-events-policies-using-powershell).</span></span>
> <span data-ttu-id="da45d-107">Por exemplo, se um administrador definir uma política de evento ao vivo usando , os usuários serão impedidos de definir permissões de evento ao vivo no cliente do Teams, mas poderão criar um evento ao vivo por meio do Microsoft Graph definindo `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany` `public` **allowedAudience** como `everyone` .</span><span class="sxs-lookup"><span data-stu-id="da45d-107">For example, if an admin sets a live event policy using `Set-CsTeamsMeetingBroadcastPolicy -Identity Global -BroadcastAttendeeVisibility EveryoneInCompany`, users will be prevented from setting live event permissions to `public` in their Teams client, but will be able to create a live event via Microsoft Graph by setting **allowedAudience** to `everyone`.</span></span> 

## <a name="properties"></a><span data-ttu-id="da45d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da45d-108">Properties</span></span>

| <span data-ttu-id="da45d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da45d-109">Property</span></span>                   | <span data-ttu-id="da45d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da45d-110">Type</span></span>                     | <span data-ttu-id="da45d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da45d-111">Description</span></span>                                                                     |
| -------------------------- | ------------------------ | ------------------------------------------------------------------------------- |
| <span data-ttu-id="da45d-112">allowedAudience</span><span class="sxs-lookup"><span data-stu-id="da45d-112">allowedAudience</span></span>            | <span data-ttu-id="da45d-113">broadcastMeetingAudience</span><span class="sxs-lookup"><span data-stu-id="da45d-113">broadcastMeetingAudience</span></span> | <span data-ttu-id="da45d-114">Define quem pode ingressar no evento ao vivo.</span><span class="sxs-lookup"><span data-stu-id="da45d-114">Defines who can join the live event.</span></span> <span data-ttu-id="da45d-115">Os valores possíveis estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="da45d-115">Possible values are listed in the following table.</span></span> |
| <span data-ttu-id="da45d-116">isRecordingEnabled</span><span class="sxs-lookup"><span data-stu-id="da45d-116">isRecordingEnabled</span></span>         | <span data-ttu-id="da45d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="da45d-117">Boolean</span></span>                  | <span data-ttu-id="da45d-118">Indica se a gravação está habilitada para este evento ao vivo.</span><span class="sxs-lookup"><span data-stu-id="da45d-118">Indicates whether recording is enabled for this live event.</span></span> <span data-ttu-id="da45d-119">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="da45d-119">Default value is `false`.</span></span>          |
| <span data-ttu-id="da45d-120">isAttendeeReportEnabled</span><span class="sxs-lookup"><span data-stu-id="da45d-120">isAttendeeReportEnabled</span></span>    | <span data-ttu-id="da45d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="da45d-121">Boolean</span></span>                  | <span data-ttu-id="da45d-122">Indica se o relatório de participantes está habilitado para este evento ao vivo.</span><span class="sxs-lookup"><span data-stu-id="da45d-122">Indicates whether attendee report is enabled for this live event.</span></span> <span data-ttu-id="da45d-123">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="da45d-123">Default value is `false`.</span></span>    |
| <span data-ttu-id="da45d-124">isQuestionAndAnswerEnabled</span><span class="sxs-lookup"><span data-stu-id="da45d-124">isQuestionAndAnswerEnabled</span></span> | <span data-ttu-id="da45d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="da45d-125">Boolean</span></span>                  | <span data-ttu-id="da45d-126">Indica se as&A estão habilitadas para este evento ao vivo.</span><span class="sxs-lookup"><span data-stu-id="da45d-126">Indicates whether Q&A is enabled for this live event.</span></span> <span data-ttu-id="da45d-127">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="da45d-127">Default value is `false`.</span></span>                |
| <span data-ttu-id="da45d-128">isVideoOnDemandEnabled</span><span class="sxs-lookup"><span data-stu-id="da45d-128">isVideoOnDemandEnabled</span></span>     | <span data-ttu-id="da45d-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="da45d-129">Boolean</span></span>                  | <span data-ttu-id="da45d-130">Indica se o vídeo sob demanda está habilitado para este evento ao vivo.</span><span class="sxs-lookup"><span data-stu-id="da45d-130">Indicates whether video on demand is enabled for this live event.</span></span> <span data-ttu-id="da45d-131">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="da45d-131">Default value is `false`.</span></span>    |

### <a name="broadcastmeetingaudience-values"></a><span data-ttu-id="da45d-132">Valores de broadcastMeetingAudience</span><span class="sxs-lookup"><span data-stu-id="da45d-132">broadcastMeetingAudience values</span></span>

| <span data-ttu-id="da45d-133">Valor</span><span class="sxs-lookup"><span data-stu-id="da45d-133">Value</span></span>              | <span data-ttu-id="da45d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="da45d-134">Description</span></span>                                                       |
| ------------------ | ----------------------------------------------------------------- |
| <span data-ttu-id="da45d-135">everyone</span><span class="sxs-lookup"><span data-stu-id="da45d-135">everyone</span></span>           | <span data-ttu-id="da45d-136">O evento ao vivo será aberto para qualquer pessoa.</span><span class="sxs-lookup"><span data-stu-id="da45d-136">The live event will be open to anyone.</span></span> <span data-ttu-id="da45d-137">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="da45d-137">This is the default value.</span></span> |
| <span data-ttu-id="da45d-138">organization</span><span class="sxs-lookup"><span data-stu-id="da45d-138">organization</span></span>       | <span data-ttu-id="da45d-139">Todos em sua organização podem participar do evento ao vivo.</span><span class="sxs-lookup"><span data-stu-id="da45d-139">Everyone in your org can join the live event.</span></span>                     |
| <span data-ttu-id="da45d-140">roleIsAttendee</span><span class="sxs-lookup"><span data-stu-id="da45d-140">roleIsAttendee</span></span>     | <span data-ttu-id="da45d-141">Somente as pessoas especificadas podem participar do evento ao vivo.</span><span class="sxs-lookup"><span data-stu-id="da45d-141">Only the specified people can join the live event.</span></span>                |
| <span data-ttu-id="da45d-142">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="da45d-142">unknownFutureValue</span></span> | <span data-ttu-id="da45d-143">Valor futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="da45d-143">Unknown future value.</span></span>                                             |

## <a name="json-representation"></a><span data-ttu-id="da45d-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da45d-144">JSON representation</span></span>

<span data-ttu-id="da45d-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da45d-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.broadcastMeetingSettings"
}-->
```json
{
  "allowedAudience": "String",
  "isRecordingEnabled": "Boolean",
  "isAttendeeReportEnabled": "Boolean",
  "isQuestionAndAnswerEnabled": "Boolean",
  "isVideoOnDemandEnabled": "Boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "broadcastSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
