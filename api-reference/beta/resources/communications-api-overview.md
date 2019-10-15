---
title: Trabalhando com a API de comunicações no Microsoft Graph
description: A API de comunicações do Microsoft Graph adiciona uma nova dimensão à maneira como seus aplicativos e serviços podem interagir com os usuários, ativando os recursos de voz e vídeo.
author: VinodRavichandran
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: d5bcd46cb89a5d911c9286ef5c2093460949a3a1
ms.sourcegitcommit: 99cbeac2ca652632d2946c4740133c9b82c8e992
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/12/2019
ms.locfileid: "37477072"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="4c24f-103">Trabalhando com a API de comunicações no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4c24f-103">Working with the calls and online meetings API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c24f-104">A API de comunicações do Microsoft Graph adiciona uma nova dimensão à maneira como você ou sua organização podem interagir com outros usuários, habilitando os principais recursos e funções de comunicação de seus aplicativos e serviços.</span><span class="sxs-lookup"><span data-stu-id="4c24f-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="4c24f-105">Você pode usar esta API para criar e receber chamadas, criar e recuperar coordenadas da reunião e verificar a presença dos usuários.</span><span class="sxs-lookup"><span data-stu-id="4c24f-105">You can use this API to create and receive calls, create and retrieve meeting coordinates, and check users' presence.</span></span>

<span data-ttu-id="4c24f-106">Você pode usar a API de comunicações para criar aplicativos de serviço (bots) que atuam como participantes de uma chamada e que criam e recuperam reuniões em nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="4c24f-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span> <!-- and to check presence availability and activity of users. -->
<span data-ttu-id="4c24f-107">Essa API fornece funcionalidade de chamada, bem como a capacidade de criar e recuperar reuniões online.</span><span class="sxs-lookup"><span data-stu-id="4c24f-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="4c24f-108">Você pode usar aplicativos de serviço (bots) com esta API, onde o bot pode atuar como participante de suas chamadas de VoIP ou reuniões do Microsoft Teams, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="4c24f-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="4c24f-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c24f-109">Authorization</span></span>

<span data-ttu-id="4c24f-110">É necessária uma das seguintes [permissões](https://docs.microsoft.com/pt-BR/graph/permissions-reference#calls-permissions) para acessar a API de comunicações.</span><span class="sxs-lookup"><span data-stu-id="4c24f-110">One of the following [permissions](https://docs.microsoft.com/pt-BR/graph/permissions-reference#calls-permissions) is required to access user operations.</span></span> <span data-ttu-id="4c24f-111">Essas permissões precisam ser concedidas pelo administrador</span><span class="sxs-lookup"><span data-stu-id="4c24f-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="4c24f-112">Cenário</span><span class="sxs-lookup"><span data-stu-id="4c24f-112">Scenario</span></span>                 | <span data-ttu-id="4c24f-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c24f-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="4c24f-114">Chamando</span><span class="sxs-lookup"><span data-stu-id="4c24f-114">Calling Plan</span></span>                 | <span data-ttu-id="4c24f-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="4c24f-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="4c24f-116">Reuniões</span><span class="sxs-lookup"><span data-stu-id="4c24f-116">Meetings</span></span>                 | <span data-ttu-id="4c24f-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c24f-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="4c24f-118">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="4c24f-118">Common use cases</span></span>

<span data-ttu-id="4c24f-119">A tabela a seguir lista alguns dos usos comuns para a API de comunicações.</span><span class="sxs-lookup"><span data-stu-id="4c24f-119">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="4c24f-120">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="4c24f-120">Use cases</span></span>                         | <span data-ttu-id="4c24f-121">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="4c24f-121">REST resources</span></span>                                 | <span data-ttu-id="4c24f-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="4c24f-122">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="4c24f-123">Criando e associando chamadas 1-1 e de grupo</span><span class="sxs-lookup"><span data-stu-id="4c24f-123">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="4c24f-124">Call</span><span class="sxs-lookup"><span data-stu-id="4c24f-124">Call</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta)| [<span data-ttu-id="4c24f-125">Métodos para chamadas</span><span class="sxs-lookup"><span data-stu-id="4c24f-125">Methods for calls</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta#methods)| 
|<span data-ttu-id="4c24f-126">Chamadas IVR</span><span class="sxs-lookup"><span data-stu-id="4c24f-126">IVR calls</span></span>   |     | [<span data-ttu-id="4c24f-127">Métodos para IVR</span><span class="sxs-lookup"><span data-stu-id="4c24f-127">Methods for IVR</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| <span data-ttu-id="4c24f-128">Controles de chamada (participante)</span><span class="sxs-lookup"><span data-stu-id="4c24f-128">Call controls (participant)</span></span> | [<span data-ttu-id="4c24f-129">Participante</span><span class="sxs-lookup"><span data-stu-id="4c24f-129">Participant</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/participant?view=graph-rest-beta)   ||
|<span data-ttu-id="4c24f-130">Reuniões</span><span class="sxs-lookup"><span data-stu-id="4c24f-130">Meetings</span></span>|[<span data-ttu-id="4c24f-131">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4c24f-131">onlineMeeting</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [<span data-ttu-id="4c24f-132">Métodos para reuniões</span><span class="sxs-lookup"><span data-stu-id="4c24f-132">Methods for meetings</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|

## <a name="common-properties"></a><span data-ttu-id="4c24f-133">Propriedades comuns</span><span class="sxs-lookup"><span data-stu-id="4c24f-133">Common properties</span></span>

| <span data-ttu-id="4c24f-134">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c24f-134">Resource</span></span>                | <span data-ttu-id="4c24f-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c24f-135">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="4c24f-136">call</span><span class="sxs-lookup"><span data-stu-id="4c24f-136">call</span></span>                               | [<span data-ttu-id="4c24f-137">propriedades de chamada</span><span class="sxs-lookup"><span data-stu-id="4c24f-137">call properties</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta#properties)  |
| <span data-ttu-id="4c24f-138">participante</span><span class="sxs-lookup"><span data-stu-id="4c24f-138">Participant</span></span>                         | [<span data-ttu-id="4c24f-139">propriedades dos participantes</span><span class="sxs-lookup"><span data-stu-id="4c24f-139">participant properties</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/participant?view=graph-rest-beta#properties) |
| <span data-ttu-id="4c24f-140">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4c24f-140">onlineMeeting</span></span>                            | [<span data-ttu-id="4c24f-141">Propriedades onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4c24f-141">onlineMeeting properties</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |

## <a name="see-also"></a><span data-ttu-id="4c24f-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="4c24f-142">See also</span></span>

- [<span data-ttu-id="4c24f-143">Exemplos da API de comunicações</span><span class="sxs-lookup"><span data-stu-id="4c24f-143">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="4c24f-144">SDK de sinalização de comunicação</span><span class="sxs-lookup"><span data-stu-id="4c24f-144">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [<span data-ttu-id="4c24f-145">SDK de mídia de comunicação</span><span class="sxs-lookup"><span data-stu-id="4c24f-145">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
