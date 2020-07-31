---
title: Usar a API de comunicações em nuvem para criar ou ingressar em reuniões online
description: Você terá a flexibilidade de criar uma reunião que ocorra no futuro ou instantaneamente
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 5e6cf66dbecfe6c8d67354bc615f3f9766feef38
ms.sourcegitcommit: 95c1cf4f70a9322d276dc84726457eeaf98169e2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2020
ms.locfileid: "46531513"
---
# <a name="use-the-cloud-communications-api-to-create-or-join-online-meetings"></a><span data-ttu-id="db144-103">Usar a API de comunicações em nuvem para criar ou ingressar em reuniões online</span><span class="sxs-lookup"><span data-stu-id="db144-103">Use the cloud communications API to create or join online meetings</span></span>

<span data-ttu-id="db144-104">As reuniões online oferecem a capacidade de especificar determinados detalhes, como o assunto da reunião e todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="db144-104">Online meetings provide the ability to specify certain details, such as the subject of the meeting, and who all the attendees are.</span></span> <span data-ttu-id="db144-105">Você também pode definir a data e a hora de início e término da reunião.</span><span class="sxs-lookup"><span data-stu-id="db144-105">You can also set the date and time for when the meeting starts and ends.</span></span>

<span data-ttu-id="db144-106">As reuniões online oferecem a flexibilidade para criar uma reunião que ocorra no futuro ou instantaneamente.</span><span class="sxs-lookup"><span data-stu-id="db144-106">Online meetings provide the flexibility to create a meeting that takes place in the future, or instantaneously.</span></span> <span data-ttu-id="db144-107">A capacidade de configurar uma reunião que inicia imediatamente após sua criação é ideal para problemas inesperados e outros incidentes que exigem a atenção imediata dos participantes.</span><span class="sxs-lookup"><span data-stu-id="db144-107">The ability to set up a meeting that starts immediately after it is created is ideal for unexpected issues and other incidents that require the immediate attention of the attendees.</span></span>

> <span data-ttu-id="db144-108">**Observação** Esse conjunto de APIs permite a flexibilidade e a integração mais rica com o Microsoft Teams ou recursos do Skype; Ele não atualiza ou cria nenhum evento em um calendário.</span><span class="sxs-lookup"><span data-stu-id="db144-108">**Note** This set of APIs allows the flexibility and richer integration with Microsoft Teams or Skype capabilities; it does not update or create any event in a calendar.</span></span> <span data-ttu-id="db144-109">Para obter uma abordagem conveniente para adicionar uma reunião online a um calendário do Outlook, use a API de calendário.</span><span class="sxs-lookup"><span data-stu-id="db144-109">For a convenient approach to add an online meeting to an Outlook calendar, use the calendar API.</span></span> <span data-ttu-id="db144-110">Consulte [escolher uma API no Microsoft Graph para criar e ingressar em reuniões online](choose-online-meeting-api.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="db144-110">See [Choose an API in Microsoft Graph to create and join online meetings](choose-online-meeting-api.md) for more information.</span></span>

## <a name="create-an-online-meeting"></a><span data-ttu-id="db144-111">Criar uma reunião online</span><span class="sxs-lookup"><span data-stu-id="db144-111">Create an online meeting</span></span>

<span data-ttu-id="db144-112">Ao criar uma reunião online, você receberá as [coordenadas](/graph/api/resources/onlinemeeting) da reunião.</span><span class="sxs-lookup"><span data-stu-id="db144-112">When you create an online meeting, you'll receive [coordinates](/graph/api/resources/onlinemeeting) for the meeting.</span></span> <span data-ttu-id="db144-113">Quando os participantes ingressam na reunião usando essas coordenadas de reunião, uma chamada de grupo é criada.</span><span class="sxs-lookup"><span data-stu-id="db144-113">When participants join the meeting using these meeting coordinates, a group call is created.</span></span>

<span data-ttu-id="db144-114">Quando todos os participantes saírem da chamada de grupo, a chamada do grupo será finalizada.</span><span class="sxs-lookup"><span data-stu-id="db144-114">When all the participants leave the group call, the group call will end.</span></span> <span data-ttu-id="db144-115">Os participantes ainda podem reingressar na reunião posteriormente usando as mesmas coordenadas de reunião, mas isso criará outra chamada de grupo.</span><span class="sxs-lookup"><span data-stu-id="db144-115">Participants can still rejoin the meeting afterward using the same meeting coordinates, but this will create another group call.</span></span>

><span data-ttu-id="db144-116">**Observação:** As reuniões criadas não aparecem em calendários.</span><span class="sxs-lookup"><span data-stu-id="db144-116">**Note:** The created meetings do not appear on calendars.</span></span>

## <a name="join-an-online-meeting"></a><span data-ttu-id="db144-117">Ingressar em uma reunião online</span><span class="sxs-lookup"><span data-stu-id="db144-117">Join an online meeting</span></span>
<span data-ttu-id="db144-118">Após a criação de uma reunião online, os usuários podem participar de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="db144-118">After an online meeting is created, users can join in two ways:</span></span>

1. <span data-ttu-id="db144-119">Por meio do navegador, usando o **joinWebURL** que foi retornado como parte das [coordenadas da reunião](/graph/api/resources/onlinemeeting).</span><span class="sxs-lookup"><span data-stu-id="db144-119">Through the browser, using the **joinWebURL** that was returned as part of the [meeting coordinates](/graph/api/resources/onlinemeeting).</span></span>

2. <span data-ttu-id="db144-120">Por meio da [API Create Call](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), que requer que você forneça as [coordenadas da reunião](/graph/api/resources/onlinemeeting), ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo)e [chatInfo](/graph/api/resources/chatinfo)).</span><span class="sxs-lookup"><span data-stu-id="db144-120">Through the [create call API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), which requires that you provide the [meeting coordinates](/graph/api/resources/onlinemeeting), ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo), and [chatInfo](/graph/api/resources/chatinfo)).</span></span>

## <a name="see-also"></a><span data-ttu-id="db144-121">Confira também</span><span class="sxs-lookup"><span data-stu-id="db144-121">See also</span></span>

- [<span data-ttu-id="db144-122">Permissões de reunião online</span><span class="sxs-lookup"><span data-stu-id="db144-122">Online meeting permissions</span></span>](/graph/permissions-reference#online-meetings-permissions)
- [<span data-ttu-id="db144-123">Escolher uma API no Microsoft Graph para criar e ingressar em reuniões online</span><span class="sxs-lookup"><span data-stu-id="db144-123">Choose an API in Microsoft Graph to create and join online meetings</span></span>](choose-online-meeting-api.md)
