---
title: tipo de recurso Presence
description: Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 797ddac8bc582cd5e5d4d51e0e1ad94645c3c1e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521569"
---
# <a name="presence-resource-type"></a><span data-ttu-id="7d703-103">tipo de recurso Presence</span><span class="sxs-lookup"><span data-stu-id="7d703-103">presence resource type</span></span>

<span data-ttu-id="7d703-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7d703-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7d703-105">Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="7d703-105">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="7d703-106">**Observação:** No momento, esse recurso só tem suporte para usuários do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7d703-106">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

## <a name="methods"></a><span data-ttu-id="7d703-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7d703-107">Methods</span></span>

| <span data-ttu-id="7d703-108">Método</span><span class="sxs-lookup"><span data-stu-id="7d703-108">Method</span></span>                                                            | <span data-ttu-id="7d703-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7d703-109">Return Type</span></span>                                       | <span data-ttu-id="7d703-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d703-110">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="7d703-111">Obter presença</span><span class="sxs-lookup"><span data-stu-id="7d703-111">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="7d703-112">presença</span><span class="sxs-lookup"><span data-stu-id="7d703-112">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="7d703-113">Obtenha as informações de presença de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7d703-113">Get a user's presence information.</span></span>
| [<span data-ttu-id="7d703-114">Obter presença de vários usuários</span><span class="sxs-lookup"><span data-stu-id="7d703-114">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="7d703-115">coleção [Presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="7d703-115">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="7d703-116">Obtenha as informações de presença de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="7d703-116">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="7d703-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d703-117">Properties</span></span>

| <span data-ttu-id="7d703-118">Relação</span><span class="sxs-lookup"><span data-stu-id="7d703-118">Relationship</span></span>        | <span data-ttu-id="7d703-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d703-119">Type</span></span>                                                 | <span data-ttu-id="7d703-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d703-120">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="7d703-121">id</span><span class="sxs-lookup"><span data-stu-id="7d703-121">id</span></span>    |  <span data-ttu-id="7d703-122">string</span><span class="sxs-lookup"><span data-stu-id="7d703-122">string</span></span>     |  <span data-ttu-id="7d703-123">A ID de objeto de usuário</span><span class="sxs-lookup"><span data-stu-id="7d703-123">The user object id</span></span>   |
|<span data-ttu-id="7d703-124">availability</span><span class="sxs-lookup"><span data-stu-id="7d703-124">availability</span></span>    |  <span data-ttu-id="7d703-125">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d703-125">string collection</span></span>   |   <span data-ttu-id="7d703-126">As informações de presença básicas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7d703-126">The base presence information for a user.</span></span> <span data-ttu-id="7d703-127">Os valores possíveis `Available`são `AvailableIdle`, `Away`, `BeRightBack` `Busy` `BusyIdle`,,, `DoNotDisturb`, `Offline`,,`PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="7d703-127">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="7d703-128">atividade</span><span class="sxs-lookup"><span data-stu-id="7d703-128">activity</span></span>    |  <span data-ttu-id="7d703-129">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d703-129">string collection</span></span>      |    <span data-ttu-id="7d703-130">As informações complementares para a disponibilidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="7d703-130">The supplemental information to a user's availability.</span></span> <span data-ttu-id="7d703-131">Os valores possíveis `Available`são `Away`, `BeRightBack``Busy` `DoNotDisturb` `InACall`,,,, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span><span class="sxs-lookup"><span data-stu-id="7d703-131">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="7d703-132">**Observação:** Para saber mais sobre os diferentes Estados de presença, confira [presença do usuário no Microsoft Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="7d703-132">**Note:** To learn more about the different presence states, see [User presence in Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="7d703-133">Relações</span><span class="sxs-lookup"><span data-stu-id="7d703-133">Relationships</span></span>

<span data-ttu-id="7d703-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d703-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d703-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d703-135">JSON representation</span></span>

<span data-ttu-id="7d703-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d703-136">The following is a JSON representation of the resource.</span></span>

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
