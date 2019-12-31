---
title: tipo de recurso Presence
description: Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 48574baf0969077add921d6b4c9d52dd2d5d4906
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913566"
---
# <a name="presence-resource-type"></a><span data-ttu-id="c6bb7-103">tipo de recurso Presence</span><span class="sxs-lookup"><span data-stu-id="c6bb7-103">presence resource type</span></span>

<span data-ttu-id="c6bb7-104">Contém informações sobre a presença de um usuário, incluindo a disponibilidade e a atividade do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6bb7-104">Contains information about a user's presence, including their availability and user activity.</span></span>

> <span data-ttu-id="c6bb7-105">**Observação:** No momento, esse recurso só tem suporte para usuários do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c6bb7-105">**Note:** This resource is currently only supported for Microsoft Teams users.</span></span>

## <a name="methods"></a><span data-ttu-id="c6bb7-106">Methods</span><span class="sxs-lookup"><span data-stu-id="c6bb7-106">Methods</span></span>

| <span data-ttu-id="c6bb7-107">Método</span><span class="sxs-lookup"><span data-stu-id="c6bb7-107">Method</span></span>                                                            | <span data-ttu-id="c6bb7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c6bb7-108">Return Type</span></span>                                       | <span data-ttu-id="c6bb7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6bb7-109">Description</span></span>                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="c6bb7-110">Obter presença</span><span class="sxs-lookup"><span data-stu-id="c6bb7-110">Get presence</span></span>](../api/presence-get.md)     | [<span data-ttu-id="c6bb7-111">presença</span><span class="sxs-lookup"><span data-stu-id="c6bb7-111">presence</span></span>](../resources/presence.md)     | <span data-ttu-id="c6bb7-112">Obtenha as informações de presença de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c6bb7-112">Get a user's presence information.</span></span>
| [<span data-ttu-id="c6bb7-113">Obter presença de vários usuários</span><span class="sxs-lookup"><span data-stu-id="c6bb7-113">Get presence of multiple users</span></span>](../api/cloudcommunications-getpresencesbyuserid.md)    |  <span data-ttu-id="c6bb7-114">coleção [Presence](../resources/presence.md)</span><span class="sxs-lookup"><span data-stu-id="c6bb7-114">[presence](../resources/presence.md) collection</span></span>     |  <span data-ttu-id="c6bb7-115">Obtenha as informações de presença de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="c6bb7-115">Get the presence information for multiple users.</span></span>      |


## <a name="properties"></a><span data-ttu-id="c6bb7-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6bb7-116">Properties</span></span>

| <span data-ttu-id="c6bb7-117">Relação</span><span class="sxs-lookup"><span data-stu-id="c6bb7-117">Relationship</span></span>        | <span data-ttu-id="c6bb7-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6bb7-118">Type</span></span>                                                 | <span data-ttu-id="c6bb7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6bb7-119">Description</span></span>                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
|<span data-ttu-id="c6bb7-120">id</span><span class="sxs-lookup"><span data-stu-id="c6bb7-120">id</span></span>    |  <span data-ttu-id="c6bb7-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6bb7-121">string</span></span>     |  <span data-ttu-id="c6bb7-122">A ID de objeto de usuário</span><span class="sxs-lookup"><span data-stu-id="c6bb7-122">The user object id</span></span>   |
|<span data-ttu-id="c6bb7-123">availability</span><span class="sxs-lookup"><span data-stu-id="c6bb7-123">availability</span></span>    |  <span data-ttu-id="c6bb7-124">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6bb7-124">string collection</span></span>   |   <span data-ttu-id="c6bb7-125">As informações de presença básicas de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c6bb7-125">The base presence information for a user.</span></span> <span data-ttu-id="c6bb7-126">Os valores possíveis `Available`são `AvailableIdle`, `Away`, `BeRightBack` `Busy` `BusyIdle`,,, `DoNotDisturb`, `Offline`,,`PresenceUnknown`</span><span class="sxs-lookup"><span data-stu-id="c6bb7-126">Possible values are `Available`, `AvailableIdle`,  `Away`, `BeRightBack`, `Busy`, `BusyIdle`, `DoNotDisturb`, `Offline`, `PresenceUnknown`</span></span>  |
|<span data-ttu-id="c6bb7-127">atividade</span><span class="sxs-lookup"><span data-stu-id="c6bb7-127">activity</span></span>    |  <span data-ttu-id="c6bb7-128">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6bb7-128">string collection</span></span>      |    <span data-ttu-id="c6bb7-129">As informações complementares para a disponibilidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c6bb7-129">The supplemental information to a user's availability.</span></span> <span data-ttu-id="c6bb7-130">Os valores possíveis `Available`são `Away`, `BeRightBack``Busy` `DoNotDisturb` `InACall`,,,, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span><span class="sxs-lookup"><span data-stu-id="c6bb7-130">Possible values are `Available`, `Away`, `BeRightBack`,`Busy`, `DoNotDisturb`, `InACall`, `InAConferenceCall`, `Inactive`,`InAMeeting`, `Offline`, `OffWork`,`OutOfOffice`, `PresenceUnknown`,`Presenting`, `UrgentInterruptionsOnly`.</span></span>       |

><span data-ttu-id="c6bb7-131">**Observação:** Para saber mais sobre os diferentes Estados de presença, confira [presença do usuário no Microsoft Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span><span class="sxs-lookup"><span data-stu-id="c6bb7-131">**Note:** To learn more about the different presence states, see [User presence in Teams](https://docs.microsoft.com/microsoftteams/presence-admins).</span></span> 

## <a name="relationships"></a><span data-ttu-id="c6bb7-132">Relações</span><span class="sxs-lookup"><span data-stu-id="c6bb7-132">Relationships</span></span>

<span data-ttu-id="c6bb7-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6bb7-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6bb7-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6bb7-134">JSON representation</span></span>

<span data-ttu-id="c6bb7-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6bb7-135">The following is a JSON representation of the resource.</span></span>

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
