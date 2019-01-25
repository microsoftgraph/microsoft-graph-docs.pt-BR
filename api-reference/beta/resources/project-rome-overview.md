---
title: 'Usar a API do Microsoft Graph para trabalhar com o Project Roma '
description: 'Project Roma é uma iniciativa da Microsoft para criar uma plataforma que permite que os desenvolvedores de aplicativos criar ótimas experiências de referência cruzada de dispositivo. Project Roma habilita recursos diferentes que se conectam a diferentes serviços e pontos de extremidade do cliente quando a usuário se conecta com a Microsoft a mesma conta ou trabalha ou escola conta. Isso permite que você implemente experiências entre dispositivos e plataforma cruzada que são centralizadas em torno de tarefas do usuário, em vez dos dispositivos. '
localization_priority: Normal
ms.openlocfilehash: 57c5189f3caf64ec048d000d5e9108811bd88145
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509690"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="da904-105">Usar a API do Microsoft Graph para trabalhar com o Project Roma</span><span class="sxs-lookup"><span data-stu-id="da904-105">Use the Microsoft Graph API to work with Project Rome</span></span> 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da904-106">[Project Roma](https://developer.microsoft.com/en-us/windows/project-rome) é uma iniciativa da Microsoft para criar uma plataforma que permite que os desenvolvedores de aplicativos criar ótimas experiências de referência cruzada de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da904-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="da904-107">Project Roma habilita recursos diferentes que se conectam a diferentes serviços e pontos de extremidade do cliente quando a usuário se conecta com a Microsoft a mesma conta ou trabalha ou escola conta.</span><span class="sxs-lookup"><span data-stu-id="da904-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="da904-108">Isso permite que você implemente experiências entre dispositivos e plataforma cruzada que são centralizadas em torno de tarefas do usuário, em vez dos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="da904-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span> 

<span data-ttu-id="da904-109">Três principais recursos de projeto Roma são expostos por meio do Microsoft Graph para ajudá-lo a habilitar ótimas experiências de referência cruzada de dispositivo: atividades, dispositivos e notificações.</span><span class="sxs-lookup"><span data-stu-id="da904-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span> 

## <a name="activities"></a><span data-ttu-id="da904-110">Atividades</span><span class="sxs-lookup"><span data-stu-id="da904-110">Activities</span></span>

<span data-ttu-id="da904-111">Atividades no Microsoft Graph habilitar compromisso do usuário de unidade com seus aplicativos em plataformas e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="da904-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="da904-112">Uma atividade é a unidade de compromisso do usuário e consiste em três componentes:</span><span class="sxs-lookup"><span data-stu-id="da904-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="da904-113">Um link profundo</span><span class="sxs-lookup"><span data-stu-id="da904-113">A deep link</span></span>
- <span data-ttu-id="da904-114">Uma representação visual</span><span class="sxs-lookup"><span data-stu-id="da904-114">A visual representation</span></span>
- <span data-ttu-id="da904-115">Metadados do conteúdo que descreve a atividade, usando o [https://schema.org/](https://schema.org/) shared vocabulário</span><span class="sxs-lookup"><span data-stu-id="da904-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="da904-116">Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de participação do usuário.</span><span class="sxs-lookup"><span data-stu-id="da904-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="da904-117">Cada vez que um usuário reengages com uma atividade, um novo item de histórico é adicionado à atividade acumular compromisso do usuário.</span><span class="sxs-lookup"><span data-stu-id="da904-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="da904-118">Quando um aplicativo publica objetos de atividade do usuário, o objeto será mostrada no algumas das novas superfícies de interface do usuário no Windows; Por exemplo, Cortana notificações e linha do tempo.</span><span class="sxs-lookup"><span data-stu-id="da904-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="da904-119">Você pode especificar metadados sofisticados (para permitir atividades a serem apresentados no contexto certo) e o ricas visuais (usando marcação [Cartão adaptável](https://adaptivecards.io/) ) em seus objetos de atividade.</span><span class="sxs-lookup"><span data-stu-id="da904-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="da904-120">Você pode usar as seguintes APIs do Microsoft Graph para criar e recuperar as atividades do usuário:</span><span class="sxs-lookup"><span data-stu-id="da904-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="da904-121">Criar ou substituir atividade</span><span class="sxs-lookup"><span data-stu-id="da904-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="da904-122">Obter atividades</span><span class="sxs-lookup"><span data-stu-id="da904-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="da904-123">Obter atividades recentes</span><span class="sxs-lookup"><span data-stu-id="da904-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="da904-124">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="da904-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="da904-125">Criar ou substituir um item do histórico</span><span class="sxs-lookup"><span data-stu-id="da904-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="da904-126">Excluir um item do histórico</span><span class="sxs-lookup"><span data-stu-id="da904-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="da904-127">Dispositivos</span><span class="sxs-lookup"><span data-stu-id="da904-127">Devices</span></span>

<span data-ttu-id="da904-128">Você pode usar o Project Roma APIs no Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="da904-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="da904-129">Descobrir e se conectar a dispositivos do usuário</span><span class="sxs-lookup"><span data-stu-id="da904-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="da904-130">Início remotamente apps nesses dispositivos</span><span class="sxs-lookup"><span data-stu-id="da904-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="da904-131">Enviar mensagens para seus aplicativos nesses dispositivos</span><span class="sxs-lookup"><span data-stu-id="da904-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="da904-132">Com essas APIs, você pode criar aplicativos que criam experiências fora de um único dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da904-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="da904-133">Por exemplo, você pode estender seu aplicativo de inicialização em uma tela maior.</span><span class="sxs-lookup"><span data-stu-id="da904-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="da904-134">Ou você pode criar uma experiência de complementares para um aplicativo em outro dos dispositivos do usuário.</span><span class="sxs-lookup"><span data-stu-id="da904-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="da904-135">Você pode usar as seguintes APIs do Microsoft Graph para se comunicar com outros dispositivos do Windows:</span><span class="sxs-lookup"><span data-stu-id="da904-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="da904-136">Listar os dispositivos do usuário</span><span class="sxs-lookup"><span data-stu-id="da904-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="da904-137">Enviar um comando para um dispositivo</span><span class="sxs-lookup"><span data-stu-id="da904-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="da904-138">Obter o status de comando</span><span class="sxs-lookup"><span data-stu-id="da904-138">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="notifications"></a><span data-ttu-id="da904-139">Notificações</span><span class="sxs-lookup"><span data-stu-id="da904-139">Notifications</span></span>

<span data-ttu-id="da904-140">Você pode usar as APIs de notificações no Microsoft Graph para fornecer notificações entre vários pontos de extremidade que o mesmo usuário tiver entrado em.</span><span class="sxs-lookup"><span data-stu-id="da904-140">You can use the notifications APIs in Microsoft Graph to deliver notifications across multiple endpoints that the same user is signed in on.</span></span> <span data-ttu-id="da904-141">É possível direcionar um usuário diretamente ao lançar notificações, em vez de se preocupar como endereços/canais de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da904-141">You can target a user directly when posting notifications instead of worrying about device addresses/channels.</span></span> <span data-ttu-id="da904-142">Dessa forma, você pode focalizar Projetando os cenários de notificação direita em uma humanos centrada, em vez de uma maneira centralizada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="da904-142">This way, you can focus on designing the right notification scenarios in a human-centric, rather than a device-centric way.</span></span> 

<span data-ttu-id="da904-143">Você pode publicar uma notificação de dados brutos ou uma notificação visual direta.</span><span class="sxs-lookup"><span data-stu-id="da904-143">You can publish a raw data notification or a direct visual notification.</span></span> <span data-ttu-id="da904-144">Quando uma notificação de dados brutos é entregue para um ponto de extremidade do dispositivo, você pode, em seguida, usar o [SDK do cliente](https://github.com/Microsoft/project-rome) (notificações de Microsoft Graph SDK para Windows, Roma SDK do Project para iOS e Android) para receber e gerenciar notificações.</span><span class="sxs-lookup"><span data-stu-id="da904-144">When a raw data notification is delivered to a device endpoint, you can then use the [client SDK](https://github.com/Microsoft/project-rome) (Microsoft Graph notifications SDK for Windows, Project Rome SDK for iOS and Android) to receive and manage notifications.</span></span> <span data-ttu-id="da904-145">Quando uma notificação visual direta é entregue para um ponto de extremidade do dispositivo, ela mostra específicos de plataforma nativa notificação ao usuário.</span><span class="sxs-lookup"><span data-stu-id="da904-145">When a direct visual notification is delivered to a device endpoint, it shows the platform-specific native notification to the user.</span></span> 

<span data-ttu-id="da904-146">Para obter detalhes, consulte [criar e enviar uma notificação](../api/projectrome-notification-post.md).</span><span class="sxs-lookup"><span data-stu-id="da904-146">For details, see [Create and send a notification](../api/projectrome-notification-post.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/project-rome-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
