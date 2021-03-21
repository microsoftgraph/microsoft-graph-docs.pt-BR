---
title: tipo de recurso de presença
description: Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.
author: jsandoval-msft
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 6de4f4f63302bfa8e1229f60c6aad77b1abe1fd8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962424"
---
# <a name="presence-resource-type"></a><span data-ttu-id="bee7d-103">tipo de recurso de presença</span><span class="sxs-lookup"><span data-stu-id="bee7d-103">presence resource type</span></span>

<span data-ttu-id="bee7d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bee7d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bee7d-105">Contém informações sobre a presença de um usuário, incluindo sua disponibilidade e atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="bee7d-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="bee7d-106">**Observação:** Atualmente, esse recurso só tem suporte para usuários do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bee7d-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="bee7d-107">Esse recurso dá suporte à assinatura para [alterar notificações.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="bee7d-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="bee7d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="bee7d-108">Methods</span></span>

| <span data-ttu-id="bee7d-109">Método</span><span class="sxs-lookup"><span data-stu-id="bee7d-109">Method</span></span>                                                            | <span data-ttu-id="bee7d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bee7d-110">Return Type</span></span>                                       | <span data-ttu-id="bee7d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bee7d-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="bee7d-112">Obter presença</span><span class="sxs-lookup"><span data-stu-id="bee7d-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="bee7d-113">presence</span><span class="sxs-lookup"><span data-stu-id="bee7d-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="bee7d-114">Obter informações de presença de um usuário.</span><span class="sxs-lookup"><span data-stu-id="bee7d-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="bee7d-115">Obter presença de vários usuários</span><span class="sxs-lookup"><span data-stu-id="bee7d-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="bee7d-116">[coleção presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="bee7d-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="bee7d-117">Obter informações de presença para vários usuários.</span><span class="sxs-lookup"><span data-stu-id="bee7d-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="bee7d-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bee7d-118">Properties</span></span>

| <span data-ttu-id="bee7d-119">Relação</span><span class="sxs-lookup"><span data-stu-id="bee7d-119">Relationship</span></span>        | <span data-ttu-id="bee7d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bee7d-120">Type</span></span>                                                 | <span data-ttu-id="bee7d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bee7d-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="bee7d-122">id</span><span class="sxs-lookup"><span data-stu-id="bee7d-122">id</span></span>    |  <span data-ttu-id="bee7d-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bee7d-123">string</span></span>     |  <span data-ttu-id="bee7d-124">A ID do objeto user</span><span class="sxs-lookup"><span data-stu-id="bee7d-124">The user object id</span></span>   |
|<span data-ttu-id="bee7d-125">availability</span><span class="sxs-lookup"><span data-stu-id="bee7d-125">availability</span></span>    |  <span data-ttu-id="bee7d-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bee7d-126">string collection</span></span>   |   <span data-ttu-id="bee7d-127">As informações de presença base para um usuário.</span><span class="sxs-lookup"><span data-stu-id="bee7d-127">The base presence information for a user.</span></span> <span data-ttu-id="bee7d-128">Os valores possíveis `Available` são , , , , , , , `AvailableIdle` ,  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="bee7d-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="bee7d-129">atividade</span><span class="sxs-lookup"><span data-stu-id="bee7d-129">activity</span></span>    |  <span data-ttu-id="bee7d-130">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bee7d-130">string collection</span></span>      |    <span data-ttu-id="bee7d-131">As informações complementares à disponibilidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="bee7d-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="bee7d-132">Os valores `Available` possíveis `Away` são , , , , , , , `BeRightBack` , , , `Busy` , , , `DoNotDisturb` `InACall` , `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="bee7d-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`, `InAMeeting`, `Offline`, `OffWork`, `OutOfOffice`, `PresenceUnknown`, `Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="bee7d-133">**Observação:** Para saber mais sobre os diferentes estados de presença, consulte [Presença do usuário no Teams](/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="bee7d-133">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="bee7d-134">Relações</span><span class="sxs-lookup"><span data-stu-id="bee7d-134">Relationships</span></span>

<span data-ttu-id="bee7d-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bee7d-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bee7d-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bee7d-136">JSON representation</span></span>

<span data-ttu-id="bee7d-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bee7d-137">The following is a JSON representation of the resource.</span></span>

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
