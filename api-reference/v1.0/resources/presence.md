---
title: tipo de recurso de presença
description: Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.
author: mkhribech
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: f155db24626420bfb43b225ee67d61ae923b048f
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896715"
---
# <a name="presence-resource-type"></a><span data-ttu-id="2eea4-103">tipo de recurso de presença</span><span class="sxs-lookup"><span data-stu-id="2eea4-103">presence resource type</span></span>

<span data-ttu-id="2eea4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2eea4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2eea4-105">Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="2eea4-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="2eea4-106">**Observação:** Atualmente, esse recurso só tem suporte para Microsoft Teams usuários.</span><span class="sxs-lookup"><span data-stu-id="2eea4-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="2eea4-107">Esse recurso dá suporte à assinatura para [alterar notificações.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="2eea4-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="2eea4-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2eea4-108">Methods</span></span>

| <span data-ttu-id="2eea4-109">Método</span><span class="sxs-lookup"><span data-stu-id="2eea4-109">Method</span></span>                                                            | <span data-ttu-id="2eea4-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2eea4-110">Return Type</span></span>                                       | <span data-ttu-id="2eea4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2eea4-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="2eea4-112">Obter presença</span><span class="sxs-lookup"><span data-stu-id="2eea4-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="2eea4-113">presence</span><span class="sxs-lookup"><span data-stu-id="2eea4-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="2eea4-114">Obter informações de presença de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2eea4-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="2eea4-115">Obter presença de vários usuários</span><span class="sxs-lookup"><span data-stu-id="2eea4-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="2eea4-116">[coleção presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="2eea4-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="2eea4-117">Obter informações de presença para vários usuários.</span><span class="sxs-lookup"><span data-stu-id="2eea4-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="2eea4-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2eea4-118">Properties</span></span>

| <span data-ttu-id="2eea4-119">Relação</span><span class="sxs-lookup"><span data-stu-id="2eea4-119">Relationship</span></span>        | <span data-ttu-id="2eea4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2eea4-120">Type</span></span>                                                 | <span data-ttu-id="2eea4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2eea4-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="2eea4-122">id</span><span class="sxs-lookup"><span data-stu-id="2eea4-122">id</span></span>    |  <span data-ttu-id="2eea4-123">string</span><span class="sxs-lookup"><span data-stu-id="2eea4-123">string</span></span>     |  <span data-ttu-id="2eea4-124">A ID do objeto user</span><span class="sxs-lookup"><span data-stu-id="2eea4-124">The user object id</span></span>   |
|<span data-ttu-id="2eea4-125">availability</span><span class="sxs-lookup"><span data-stu-id="2eea4-125">availability</span></span>    |  <span data-ttu-id="2eea4-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2eea4-126">string collection</span></span>   |   <span data-ttu-id="2eea4-127">As informações de presença base para um usuário.</span><span class="sxs-lookup"><span data-stu-id="2eea4-127">The base presence information for a user.</span></span> <span data-ttu-id="2eea4-128">Os valores possíveis `Available` são , , , , , , , `AvailableIdle` ,  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="2eea4-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="2eea4-129">atividade</span><span class="sxs-lookup"><span data-stu-id="2eea4-129">activity</span></span>    |  <span data-ttu-id="2eea4-130">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2eea4-130">string collection</span></span>      |    <span data-ttu-id="2eea4-131">As informações complementares à disponibilidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="2eea4-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="2eea4-132">Os valores `Available` possíveis `Away` são , , , , , , , `BeRightBack` , , , `Busy` , , , `DoNotDisturb` `InACall` , `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="2eea4-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`, `InAMeeting`, `Offline`, `OffWork`, `OutOfOffice`, `PresenceUnknown`, `Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="2eea4-133">**Observação:** Para saber mais sobre os diferentes estados de presença, consulte [Presença do usuário em Teams](/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="2eea4-133">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="2eea4-134">Relações</span><span class="sxs-lookup"><span data-stu-id="2eea4-134">Relationships</span></span>

<span data-ttu-id="2eea4-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2eea4-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2eea4-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2eea4-136">JSON representation</span></span>

<span data-ttu-id="2eea4-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2eea4-137">The following is a JSON representation of the resource.</span></span>

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
