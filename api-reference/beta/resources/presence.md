---
title: tipo de recurso de presença
description: Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: ddbe555df37d232940bb8eadb081be459d0f8562
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796574"
---
# <a name="presence-resource-type"></a><span data-ttu-id="26863-103">tipo de recurso de presença</span><span class="sxs-lookup"><span data-stu-id="26863-103">presence resource type</span></span>

<span data-ttu-id="26863-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26863-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26863-105">Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="26863-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="26863-106">**Observação:** No momento, esse recurso só tem suporte para usuários do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="26863-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

<span data-ttu-id="26863-107">Esse recurso dá suporte à assinatura para [alterar notificações.](/graph/webhooks)</span><span class="sxs-lookup"><span data-stu-id="26863-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="26863-108">Methods</span><span class="sxs-lookup"><span data-stu-id="26863-108">Methods</span></span>

| <span data-ttu-id="26863-109">Método</span><span class="sxs-lookup"><span data-stu-id="26863-109">Method</span></span>                                                            | <span data-ttu-id="26863-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="26863-110">Return Type</span></span>                                       | <span data-ttu-id="26863-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26863-111">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="26863-112">Obter presença</span><span class="sxs-lookup"><span data-stu-id="26863-112">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="26863-113">presença</span><span class="sxs-lookup"><span data-stu-id="26863-113">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="26863-114">Obter informações de presença de um usuário.</span><span class="sxs-lookup"><span data-stu-id="26863-114">Get a user's presence information.</span></span>
| [<span data-ttu-id="26863-115">Obter presença de vários usuários</span><span class="sxs-lookup"><span data-stu-id="26863-115">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="26863-116">[coleção de](../resources/presence.md) presença</span><span class="sxs-lookup"><span data-stu-id="26863-116">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="26863-117">Obter as informações de presença para vários usuários.</span><span class="sxs-lookup"><span data-stu-id="26863-117">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="26863-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26863-118">Properties</span></span>

| <span data-ttu-id="26863-119">Relação</span><span class="sxs-lookup"><span data-stu-id="26863-119">Relationship</span></span>        | <span data-ttu-id="26863-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="26863-120">Type</span></span>                                                 | <span data-ttu-id="26863-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="26863-121">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="26863-122">id</span><span class="sxs-lookup"><span data-stu-id="26863-122">id</span></span>    |  <span data-ttu-id="26863-123">string</span><span class="sxs-lookup"><span data-stu-id="26863-123">string</span></span>     |  <span data-ttu-id="26863-124">A ID de objeto do usuário</span><span class="sxs-lookup"><span data-stu-id="26863-124">The user object id</span></span>   |
|<span data-ttu-id="26863-125">availability</span><span class="sxs-lookup"><span data-stu-id="26863-125">availability</span></span>    |  <span data-ttu-id="26863-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="26863-126">string collection</span></span>   |   <span data-ttu-id="26863-127">As informações de presença base para um usuário.</span><span class="sxs-lookup"><span data-stu-id="26863-127">The base presence information for a user.</span></span> <span data-ttu-id="26863-128">Os valores `Available` possíveis `AvailableIdle` são , , , , , ,  `Away` `BeRightBack` `Busy` `BusyIdle` `DoNotDisturb` `Offline` , `PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="26863-128">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="26863-129">atividade</span><span class="sxs-lookup"><span data-stu-id="26863-129">activity</span></span>    |  <span data-ttu-id="26863-130">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="26863-130">string collection</span></span>      |    <span data-ttu-id="26863-131">As informações complementares para a disponibilidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="26863-131">The supplemental information to a user's availability.</span></span> <span data-ttu-id="26863-132">Os valores `Available` possíveis `Away` são , , , `BeRightBack` , `Busy` , , `DoNotDisturb` , `InACall` `InAConferenceCall` `Inactive` `InAMeeting` `Offline` `OffWork` `OutOfOffice` `PresenceUnknown` `Presenting` `UrgentInterruptionsOnly` .</span><span class="sxs-lookup"><span data-stu-id="26863-132">Possible values are `Available`, `Away`, `BeRightBack`, `Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |
|<span data-ttu-id="26863-133">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="26863-133">outOfOfficeSettings</span></span> | [<span data-ttu-id="26863-134">outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="26863-134">outOfOfficeSettings</span></span>](outOfOfficeSettings.md) | <span data-ttu-id="26863-135">As configurações de fora do escritório para um usuário.</span><span class="sxs-lookup"><span data-stu-id="26863-135">The out of office settings for a user.</span></span> |

><span data-ttu-id="26863-136">**Observação:** Para saber mais sobre os diferentes estados de presença, confira [Presença do usuário no Teams.](/microsoftteams/presence-admins)</span><span class="sxs-lookup"><span data-stu-id="26863-136">**Note:** To learn more about the different presence states, see [User presence in Teams](/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="26863-137">Relações</span><span class="sxs-lookup"><span data-stu-id="26863-137">Relationships</span></span>

<span data-ttu-id="26863-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26863-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26863-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26863-139">JSON representation</span></span>

<span data-ttu-id="26863-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26863-140">The following is a JSON representation of the resource.</span></span>

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
