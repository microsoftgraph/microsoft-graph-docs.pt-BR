---
title: tipo de recurso de presença
description: Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: d6f88f23a6c08d5aa757163d4956c104a603e87b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515622"
---
# <a name="presence-resource-type"></a><span data-ttu-id="e1cc8-103">tipo de recurso de presença</span><span class="sxs-lookup"><span data-stu-id="e1cc8-103">presence resource type</span></span>

<span data-ttu-id="e1cc8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1cc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1cc8-105">Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1cc8-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="e1cc8-106">**Observação:** Atualmente, esse recurso só tem suporte para usuários do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e1cc8-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="e1cc8-107">Esse recurso dá suporte à assinatura para [alterar notificações.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="e1cc8-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="e1cc8-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e1cc8-108">Methods</span></span>

| <span data-ttu-id="e1cc8-109">Método</span><span class="sxs-lookup"><span data-stu-id="e1cc8-109">Method</span></span>                                                            | <span data-ttu-id="e1cc8-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e1cc8-110">Return Type</span></span>                                       | <span data-ttu-id="e1cc8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1cc8-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="e1cc8-112">Obter presença</span><span class="sxs-lookup"><span data-stu-id="e1cc8-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="e1cc8-113">presence</span><span class="sxs-lookup"><span data-stu-id="e1cc8-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="e1cc8-114">Obter informações de presença de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e1cc8-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="e1cc8-115">Obter presença de vários usuários</span><span class="sxs-lookup"><span data-stu-id="e1cc8-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="e1cc8-116">[coleção presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="e1cc8-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="e1cc8-117">Obter informações de presença para vários usuários.</span><span class="sxs-lookup"><span data-stu-id="e1cc8-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="e1cc8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1cc8-118">Properties</span></span>

| <span data-ttu-id="e1cc8-119">Relação</span><span class="sxs-lookup"><span data-stu-id="e1cc8-119">Relationship</span></span>        | <span data-ttu-id="e1cc8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1cc8-120">Type</span></span>                                                 | <span data-ttu-id="e1cc8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1cc8-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="e1cc8-122">id</span><span class="sxs-lookup"><span data-stu-id="e1cc8-122">id</span></span>    |  <span data-ttu-id="e1cc8-123">string</span><span class="sxs-lookup"><span data-stu-id="e1cc8-123">string</span></span>     |  <span data-ttu-id="e1cc8-124">A ID do objeto user</span><span class="sxs-lookup"><span data-stu-id="e1cc8-124">The user object id</span></span>   |
|<span data-ttu-id="e1cc8-125">availability</span><span class="sxs-lookup"><span data-stu-id="e1cc8-125">availability</span></span>    |  <span data-ttu-id="e1cc8-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1cc8-126">string collection</span></span>   |   <span data-ttu-id="e1cc8-127">As informações de presença base para um usuário.</span><span class="sxs-lookup"><span data-stu-id="e1cc8-127">The base presence information for a user.</span></span> <span data-ttu-id="e1cc8-128">Os valores possíveis `Available` são , , , , , , , `AvailableIdle` ,  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="e1cc8-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="e1cc8-129">atividade</span><span class="sxs-lookup"><span data-stu-id="e1cc8-129">activity</span></span>    |  <span data-ttu-id="e1cc8-130">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1cc8-130">string collection</span></span>      |    <span data-ttu-id="e1cc8-131">As informações complementares à disponibilidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e1cc8-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="e1cc8-132">Os valores `Available` possíveis `Away` são , , , , , , , `BeRightBack` , , , `Busy` , , , `DoNotDisturb` `InACall` , `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="e1cc8-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |
|<span data-ttu-id="e1cc8-133">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="e1cc8-133">outOfOfficeSettings</span></span> | [<span data-ttu-id="e1cc8-134">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="e1cc8-134">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="e1cc8-135">As configurações fora do escritório para um usuário.</span><span class="sxs-lookup"><span data-stu-id="e1cc8-135">The out of office settings for a user.</span></span> |

><span data-ttu-id="e1cc8-136">**Observação:** Para saber mais sobre os diferentes estados de presença, consulte [Presença do usuário no Teams](/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="e1cc8-136">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="e1cc8-137">Relações</span><span class="sxs-lookup"><span data-stu-id="e1cc8-137">Relationships</span></span>

<span data-ttu-id="e1cc8-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1cc8-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1cc8-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1cc8-139">JSON representation</span></span>

<span data-ttu-id="e1cc8-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1cc8-140">The following is a JSON representation of the resource.</span></span>

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
