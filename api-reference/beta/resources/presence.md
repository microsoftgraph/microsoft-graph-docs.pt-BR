---
title: tipo de recurso de presença
description: Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 257167fe5b7d417751771650f8e5f03b3dd66296
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107687"
---
# <a name="presence-resource-type"></a><span data-ttu-id="237d5-103">tipo de recurso de presença</span><span class="sxs-lookup"><span data-stu-id="237d5-103">presence resource type</span></span>

<span data-ttu-id="237d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="237d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="237d5-105">Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="237d5-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="237d5-106">**Observação:** Atualmente, esse recurso só tem suporte para Microsoft Teams usuários.</span><span class="sxs-lookup"><span data-stu-id="237d5-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="237d5-107">Esse recurso dá suporte à assinatura para [alterar notificações.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="237d5-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="237d5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="237d5-108">Methods</span></span>

| <span data-ttu-id="237d5-109">Método</span><span class="sxs-lookup"><span data-stu-id="237d5-109">Method</span></span>                                                                               | <span data-ttu-id="237d5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="237d5-110">Return Type</span></span>                                     | <span data-ttu-id="237d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="237d5-111">Description</span></span>                                      |
| :----------------------------------------------------------------------------------- | :---------------------------------------------- | :----------------------------------------------- |
| [<span data-ttu-id="237d5-112">Obter presença</span><span class="sxs-lookup"><span data-stu-id="237d5-112">Get presence</span></span>](../api/presence-get.md)                                               | [<span data-ttu-id="237d5-113">presence</span><span class="sxs-lookup"><span data-stu-id="237d5-113">presence</span></span>](../resources/presence.md)            | <span data-ttu-id="237d5-114">Obter informações de presença de um usuário.</span><span class="sxs-lookup"><span data-stu-id="237d5-114">Get a user's presence information.</span></span>               |
| [<span data-ttu-id="237d5-115">Obter presença de vários usuários</span><span class="sxs-lookup"><span data-stu-id="237d5-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md) | <span data-ttu-id="237d5-116">[coleção presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="237d5-116">[presence](../resources/presence.md) collection</span></span> | <span data-ttu-id="237d5-117">Obter informações de presença para vários usuários.</span><span class="sxs-lookup"><span data-stu-id="237d5-117">Get the presence information for multiple users.</span></span> |
| [<span data-ttu-id="237d5-118">Definir presença</span><span class="sxs-lookup"><span data-stu-id="237d5-118">Set presence</span></span>](../api/presence-setpresence.md)                                               |                                                 | <span data-ttu-id="237d5-119">Definir a sessão de presença de um aplicativo para um usuário.</span><span class="sxs-lookup"><span data-stu-id="237d5-119">Set an application's presence session for a user.</span></span>           |
| [<span data-ttu-id="237d5-120">Presença clara</span><span class="sxs-lookup"><span data-stu-id="237d5-120">Clear presence</span></span>](../api/presence-clearpresence.md)                                           |                                                 | <span data-ttu-id="237d5-121">Desmarcar a sessão de presença de um aplicativo para um usuário.</span><span class="sxs-lookup"><span data-stu-id="237d5-121">Clear an application's presence session for a user.</span></span>         |

## <a name="properties"></a><span data-ttu-id="237d5-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="237d5-122">Properties</span></span>

| <span data-ttu-id="237d5-123">Relação</span><span class="sxs-lookup"><span data-stu-id="237d5-123">Relationship</span></span>        | <span data-ttu-id="237d5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="237d5-124">Type</span></span>                                          | <span data-ttu-id="237d5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="237d5-125">Description</span></span>                                                                                                                                                                                                                                                                                    |
| :------------------ | :-------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="237d5-126">id</span><span class="sxs-lookup"><span data-stu-id="237d5-126">id</span></span>                  | <span data-ttu-id="237d5-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="237d5-127">string</span></span>                                        | <span data-ttu-id="237d5-128">A ID do objeto user</span><span class="sxs-lookup"><span data-stu-id="237d5-128">The user object id</span></span>                                                                                                                                                                                                                                                                             |
| <span data-ttu-id="237d5-129">availability</span><span class="sxs-lookup"><span data-stu-id="237d5-129">availability</span></span>        | <span data-ttu-id="237d5-130">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="237d5-130">string collection</span></span>                             | <span data-ttu-id="237d5-131">As informações de presença base para um usuário.</span><span class="sxs-lookup"><span data-stu-id="237d5-131">The base presence information for a user.</span></span> <span data-ttu-id="237d5-132">Os valores possíveis `Available` são , , , , , , , `AvailableIdle` ,  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="237d5-132">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>                                                                                                           |
| <span data-ttu-id="237d5-133">atividade</span><span class="sxs-lookup"><span data-stu-id="237d5-133">activity</span></span>            | <span data-ttu-id="237d5-134">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="237d5-134">string collection</span></span>                             | <span data-ttu-id="237d5-135">As informações complementares à disponibilidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="237d5-135">The supplemental information to a user's availability.</span></span> <span data-ttu-id="237d5-136">Os valores `Available` possíveis `Away` são , , , , , , , `BeRightBack` , , , `Busy` , , , `DoNotDisturb` `InACall` , `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="237d5-136">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span> |
| <span data-ttu-id="237d5-137">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="237d5-137">outOfOfficeSettings</span></span> | [<span data-ttu-id="237d5-138">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="237d5-138">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="237d5-139">As configurações fora do escritório para um usuário.</span><span class="sxs-lookup"><span data-stu-id="237d5-139">The out of office settings for a user.</span></span>                                                                                                                                                                                                                                                         |

><span data-ttu-id="237d5-140">**Observação:** Para saber mais sobre os diferentes estados de presença, consulte [Presença do usuário em Teams](/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="237d5-140">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="237d5-141">Relações</span><span class="sxs-lookup"><span data-stu-id="237d5-141">Relationships</span></span>

<span data-ttu-id="237d5-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="237d5-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="237d5-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="237d5-143">JSON representation</span></span>

<span data-ttu-id="237d5-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="237d5-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.presence"
}-->
```json
{
   "id":"string",
   "availability":"string",
   "activity":"string",
   "outOfOfficeSettings":{"@odata.type": "#microsoft.graph.outOfOfficeSettings"}
}
```
