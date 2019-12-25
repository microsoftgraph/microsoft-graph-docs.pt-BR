---
title: Visão geral das chamadas
description: Saiba mais sobre os tipos de chamadas compatíveis e como eles são usados para o processo de sinalização.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 8de1f5d890504d9edc63213333f1ea8c4b47282f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871560"
---
# <a name="calls-overview"></a><span data-ttu-id="f8e05-103">Visão geral das chamadas</span><span class="sxs-lookup"><span data-stu-id="f8e05-103">Calls overview</span></span>

<span data-ttu-id="f8e05-104">As APIs de comunicação em nuvem no Microsoft Graph adicionam uma nova dimensão a como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados a comunicações, como chamadas e reuniões online.</span><span class="sxs-lookup"><span data-stu-id="f8e05-104">The cloud communications APIs in Microsoft Graph add a new dimension to how your apps and services interact with users through various communications related features, such as calls and online meetings.</span></span> <span data-ttu-id="f8e05-105">Este artigo descreve os tipos de chamadas compatíveis e como eles são usados para o processo de sinalização.</span><span class="sxs-lookup"><span data-stu-id="f8e05-105">This article describes the supported call types and how they're used for the signaling process.</span></span>

## <a name="peer-to-peer-calls"></a><span data-ttu-id="f8e05-106">Chamadas ponto a ponto</span><span class="sxs-lookup"><span data-stu-id="f8e05-106">Peer-to-peer calls</span></span>
<span data-ttu-id="f8e05-107">Uma chamada é ponto a ponto (P2P) quando um participante está ligando diretamente para outro participante.</span><span class="sxs-lookup"><span data-stu-id="f8e05-107">A call is peer-to-peer (P2P) when one participant is directly calling another participant.</span></span> <span data-ttu-id="f8e05-108">Se um bot chamar um usuário e o usuário for o único destino de chamada especificado, este é um exemplo de uma chamada P2P.</span><span class="sxs-lookup"><span data-stu-id="f8e05-108">If a bot calls a user, and the user is the only calling target specified, this is an example of a P2P call.</span></span>

![Diagrama de chamada P2P](images/communications-p2p-call.PNG)

<span data-ttu-id="f8e05-110">Se um usuário quiser chamar um bot, o bot não precisará de nenhuma permissão adicional para responder à chamada P2P.</span><span class="sxs-lookup"><span data-stu-id="f8e05-110">If a user wants to call a bot, the bot doesn't need any additional permissions in order to respond to the P2P call.</span></span> <span data-ttu-id="f8e05-111">Para que um bot chame um usuário, ele deve ter a permissão calls. initiate. All para uma chamada P2P.</span><span class="sxs-lookup"><span data-stu-id="f8e05-111">In order for a bot to call a user, it must have the Calls.Initiate.All permission for a P2P call.</span></span>

## <a name="group-calls"></a><span data-ttu-id="f8e05-112">Chamadas de grupo</span><span class="sxs-lookup"><span data-stu-id="f8e05-112">Group calls</span></span>

<span data-ttu-id="f8e05-113">Uma chamada de grupo ocorrerá se houver três ou mais participantes na chamada ou se as [coordenadas da reunião](/graph/api/resources/onlinemeeting) foram especificadas quando a chamada foi criada inicialmente.</span><span class="sxs-lookup"><span data-stu-id="f8e05-113">A group call occurs if there are either three or more participants in the call, or if [meeting coordinates](/graph/api/resources/onlinemeeting) were specified when the call was initially created.</span></span> 

<span data-ttu-id="f8e05-114">Você pode criar uma chamada de grupo pelo Microsoft Teams, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="f8e05-114">You can create a group call through Microsoft Teams, for example.</span></span>

![Diagrama de chamada de grupo](images/communications-group-call.PNG)

<span data-ttu-id="f8e05-116">No momento, os bots podem:</span><span class="sxs-lookup"><span data-stu-id="f8e05-116">Currently, bots are able to:</span></span>
- <span data-ttu-id="f8e05-117">Criar chamadas em grupo</span><span class="sxs-lookup"><span data-stu-id="f8e05-117">Create group calls</span></span>
- <span data-ttu-id="f8e05-118">Ingressar em chamadas de grupo existentes</span><span class="sxs-lookup"><span data-stu-id="f8e05-118">Join exisiting group calls</span></span>
- <span data-ttu-id="f8e05-119">Convidar outros participantes para uma chamada de grupo existente</span><span class="sxs-lookup"><span data-stu-id="f8e05-119">Invite other participants into an existing group call</span></span>
- <span data-ttu-id="f8e05-120">Ser convidado para chamadas de grupo existentes</span><span class="sxs-lookup"><span data-stu-id="f8e05-120">Be invited into existing group calls</span></span>

## <a name="see-also"></a><span data-ttu-id="f8e05-121">Confira também</span><span class="sxs-lookup"><span data-stu-id="f8e05-121">See also</span></span>

- [<span data-ttu-id="f8e05-122">Visão geral da API de comunicações em nuvem</span><span class="sxs-lookup"><span data-stu-id="f8e05-122">Cloud communications API overview</span></span>](cloud-communications-concept-overview.md)
- [<span data-ttu-id="f8e05-123">Permissões para chamadas</span><span class="sxs-lookup"><span data-stu-id="f8e05-123">Permissions for calls</span></span>](/graph/permissions-reference#calls-permissions)
