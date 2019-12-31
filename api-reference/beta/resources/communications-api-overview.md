---
title: Trabalhando com a API de comunicações no Microsoft Graph
description: A API de comunicações do Microsoft Graph adiciona uma nova dimensão à maneira como seus aplicativos e serviços podem interagir com os usuários, ativando os recursos de voz e vídeo.
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 7bbe0ba0387ebbbb6669d463dba7073f571efbf9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913335"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="8553b-103">Trabalhando com a API de comunicações no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8553b-103">Working with the communications API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8553b-104">A API de comunicações do Microsoft Graph adiciona uma nova dimensão à maneira como você ou sua organização podem interagir com outros usuários, habilitando os principais recursos e funções de comunicação de seus aplicativos e serviços.</span><span class="sxs-lookup"><span data-stu-id="8553b-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="8553b-105">Você pode usar esta API para criar e receber chamadas, criar e recuperar coordenadas da reunião e verificar a presença dos usuários.</span><span class="sxs-lookup"><span data-stu-id="8553b-105">You can use this API to create and receive calls, create and retrieve meeting coordinates, and check users' presence.</span></span>

<span data-ttu-id="8553b-106">Você pode usar a API de comunicações para criar aplicativos de serviço (bots) que atuam como participantes de uma chamada e que criam e recuperam reuniões em nome dos usuários e verificar a disponibilidade e a atividade de presença.</span><span class="sxs-lookup"><span data-stu-id="8553b-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users and to check their presence availability and activity.</span></span>
<span data-ttu-id="8553b-107">Essa API fornece funcionalidade de chamada, bem como a capacidade de criar e recuperar reuniões online.</span><span class="sxs-lookup"><span data-stu-id="8553b-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="8553b-108">Você pode usar aplicativos de serviço (bots) com esta API, onde o bot pode atuar como participante de suas chamadas de VoIP ou reuniões do Microsoft Teams, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="8553b-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="8553b-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="8553b-109">Authorization</span></span>

<span data-ttu-id="8553b-110">É necessária uma das seguintes [permissões](/graph/permissions-reference#calls-permissions) para acessar a API de comunicações.</span><span class="sxs-lookup"><span data-stu-id="8553b-110">One of the following [permissions](/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="8553b-111">Essas permissões precisam ser concedidas pelo administrador</span><span class="sxs-lookup"><span data-stu-id="8553b-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="8553b-112">Cenário</span><span class="sxs-lookup"><span data-stu-id="8553b-112">Scenario</span></span>                 | <span data-ttu-id="8553b-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="8553b-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="8553b-114">Chamando</span><span class="sxs-lookup"><span data-stu-id="8553b-114">Calling</span></span>                 | <span data-ttu-id="8553b-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="8553b-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="8553b-116">Reuniões</span><span class="sxs-lookup"><span data-stu-id="8553b-116">Meetings</span></span>                 | <span data-ttu-id="8553b-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8553b-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="8553b-118">Presença</span><span class="sxs-lookup"><span data-stu-id="8553b-118">Presence</span></span>                 | <span data-ttu-id="8553b-119">Presence.Read, Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="8553b-119">Presence.Read, Presence.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="8553b-120">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="8553b-120">Common use cases</span></span>

<span data-ttu-id="8553b-121">A tabela a seguir lista alguns dos usos comuns para a API de comunicações.</span><span class="sxs-lookup"><span data-stu-id="8553b-121">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="8553b-122">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="8553b-122">Use cases</span></span>                         | <span data-ttu-id="8553b-123">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="8553b-123">REST resources</span></span>                                 | <span data-ttu-id="8553b-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="8553b-124">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="8553b-125">Criando e associando chamadas 1-1 e de grupo</span><span class="sxs-lookup"><span data-stu-id="8553b-125">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="8553b-126">Call</span><span class="sxs-lookup"><span data-stu-id="8553b-126">Call</span></span>](/graph/api/resources/call?view=graph-rest-beta)| [<span data-ttu-id="8553b-127">Métodos para chamadas</span><span class="sxs-lookup"><span data-stu-id="8553b-127">Methods for calls</span></span>](/graph/api/resources/call?view=graph-rest-beta#methods)|
|<span data-ttu-id="8553b-128">Chamadas IVR</span><span class="sxs-lookup"><span data-stu-id="8553b-128">IVR calls</span></span>   |     | [<span data-ttu-id="8553b-129">Métodos para IVR</span><span class="sxs-lookup"><span data-stu-id="8553b-129">Methods for IVR</span></span>](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| <span data-ttu-id="8553b-130">Controles de chamada (participante)</span><span class="sxs-lookup"><span data-stu-id="8553b-130">Call controls (participant)</span></span> | [<span data-ttu-id="8553b-131">Participante</span><span class="sxs-lookup"><span data-stu-id="8553b-131">Participant</span></span>](/graph/api/resources/participant?view=graph-rest-beta)   ||
|<span data-ttu-id="8553b-132">Reuniões</span><span class="sxs-lookup"><span data-stu-id="8553b-132">Meetings</span></span>|[<span data-ttu-id="8553b-133">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8553b-133">onlineMeeting</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [<span data-ttu-id="8553b-134">Métodos para reuniões</span><span class="sxs-lookup"><span data-stu-id="8553b-134">Methods for meetings</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|
|<span data-ttu-id="8553b-135">Presença</span><span class="sxs-lookup"><span data-stu-id="8553b-135">Presence</span></span> | [<span data-ttu-id="8553b-136">presença</span><span class="sxs-lookup"><span data-stu-id="8553b-136">presence</span></span>](/graph/api/resources/presence) | [<span data-ttu-id="8553b-137">Métodos para presença</span><span class="sxs-lookup"><span data-stu-id="8553b-137">Methods for presence</span></span>](/graph/api/resources/presence#methods) |

## <a name="common-properties"></a><span data-ttu-id="8553b-138">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="8553b-138">Common properties</span></span>

| <span data-ttu-id="8553b-139">Recurso</span><span class="sxs-lookup"><span data-stu-id="8553b-139">Resource</span></span>                | <span data-ttu-id="8553b-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8553b-140">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="8553b-141">call</span><span class="sxs-lookup"><span data-stu-id="8553b-141">call</span></span>                               | [<span data-ttu-id="8553b-142">propriedades de chamada</span><span class="sxs-lookup"><span data-stu-id="8553b-142">call properties</span></span>](/graph/api/resources/call?view=graph-rest-beta#properties)  |
| <span data-ttu-id="8553b-143">participante</span><span class="sxs-lookup"><span data-stu-id="8553b-143">participant</span></span>                         | [<span data-ttu-id="8553b-144">propriedades dos participantes</span><span class="sxs-lookup"><span data-stu-id="8553b-144">participant properties</span></span>](/graph/api/resources/participant?view=graph-rest-beta#properties) |
| <span data-ttu-id="8553b-145">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8553b-145">onlineMeeting</span></span>                            | [<span data-ttu-id="8553b-146">Propriedades onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8553b-146">onlineMeeting properties</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |
| <span data-ttu-id="8553b-147">presença</span><span class="sxs-lookup"><span data-stu-id="8553b-147">presence</span></span> | [<span data-ttu-id="8553b-148">Propriedades de presença</span><span class="sxs-lookup"><span data-stu-id="8553b-148">presence properties</span></span>](/graph/api/resources/presence#properties) |

## <a name="see-also"></a><span data-ttu-id="8553b-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="8553b-149">See also</span></span>

- [<span data-ttu-id="8553b-150">Exemplos da API de comunicações</span><span class="sxs-lookup"><span data-stu-id="8553b-150">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="8553b-151">SDK de sinalização de comunicação</span><span class="sxs-lookup"><span data-stu-id="8553b-151">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [<span data-ttu-id="8553b-152">SDK de mídia de comunicação</span><span class="sxs-lookup"><span data-stu-id="8553b-152">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
