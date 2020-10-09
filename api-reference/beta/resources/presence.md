---
title: tipo de recurso Presence
description: Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 286951698255b1a7a7ab3164a82b6fff92cc54ac
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405327"
---
# <a name="presence-resource-type"></a><span data-ttu-id="f61e0-103">tipo de recurso Presence</span><span class="sxs-lookup"><span data-stu-id="f61e0-103">presence resource type</span></span>

<span data-ttu-id="f61e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f61e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f61e0-105">Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="f61e0-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="f61e0-106">**Observação:** No momento, esse recurso só tem suporte para usuários do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f61e0-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="f61e0-107">Esse recurso oferece suporte à assinatura de [alteração de notificações](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="f61e0-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="f61e0-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f61e0-108">Methods</span></span>

| <span data-ttu-id="f61e0-109">Método</span><span class="sxs-lookup"><span data-stu-id="f61e0-109">Method</span></span>                                                            | <span data-ttu-id="f61e0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f61e0-110">Return Type</span></span>                                       | <span data-ttu-id="f61e0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f61e0-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="f61e0-112">Obter presença</span><span class="sxs-lookup"><span data-stu-id="f61e0-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="f61e0-113">presence</span><span class="sxs-lookup"><span data-stu-id="f61e0-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="f61e0-114">Obtenha as informações de presença de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f61e0-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="f61e0-115">Obter presença de vários usuários</span><span class="sxs-lookup"><span data-stu-id="f61e0-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="f61e0-116">coleção [Presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="f61e0-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="f61e0-117">Obtenha as informações de presença de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="f61e0-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="f61e0-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f61e0-118">Properties</span></span>

| <span data-ttu-id="f61e0-119">Relação</span><span class="sxs-lookup"><span data-stu-id="f61e0-119">Relationship</span></span>        | <span data-ttu-id="f61e0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f61e0-120">Type</span></span>                                                 | <span data-ttu-id="f61e0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f61e0-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="f61e0-122">id</span><span class="sxs-lookup"><span data-stu-id="f61e0-122">id</span></span>    |  <span data-ttu-id="f61e0-123">string</span><span class="sxs-lookup"><span data-stu-id="f61e0-123">string</span></span>     |  <span data-ttu-id="f61e0-124">A ID de objeto de usuário</span><span class="sxs-lookup"><span data-stu-id="f61e0-124">The user object id</span></span>   |
|<span data-ttu-id="f61e0-125">availability</span><span class="sxs-lookup"><span data-stu-id="f61e0-125">availability</span></span>    |  <span data-ttu-id="f61e0-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f61e0-126">string collection</span></span>   |   <span data-ttu-id="f61e0-127">As informações de presença básicas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f61e0-127">The base presence information for a user.</span></span> <span data-ttu-id="f61e0-128">Os valores possíveis são,,,,, `Available` `AvailableIdle` ,,  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="f61e0-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="f61e0-129">atividade</span><span class="sxs-lookup"><span data-stu-id="f61e0-129">activity</span></span>    |  <span data-ttu-id="f61e0-130">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f61e0-130">string collection</span></span>      |    <span data-ttu-id="f61e0-131">As informações complementares para a disponibilidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f61e0-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="f61e0-132">Os valores possíveis são,,,,, `Available` `Away` `BeRightBack` `Busy` `DoNotDisturb` `InACall` `InAConferenceCall` , `Inactive` , `InAMeeting` , `Offline` , `OffWork` , `OutOfOffice` , `PresenceUnknown` , `Presenting` , `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="f61e0-132">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="f61e0-133">**Observação:** Para saber mais sobre os diferentes Estados de presença, confira [presença do usuário no Microsoft Teams](/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="f61e0-133">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="f61e0-134">Relações</span><span class="sxs-lookup"><span data-stu-id="f61e0-134">Relationships</span></span>

<span data-ttu-id="f61e0-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f61e0-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f61e0-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f61e0-136">JSON representation</span></span>

<span data-ttu-id="f61e0-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f61e0-137">The following is a JSON representation of the resource.</span></span>

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
   "activity":"string"
}
```