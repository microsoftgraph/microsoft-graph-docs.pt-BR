---
title: 'Usar a API do Microsoft Graph para trabalhar com o Project Roma '
description: 'O Project Roma é uma iniciativa da Microsoft para criar uma plataforma que permite aos desenvolvedores de aplicativos criar grandes experiências entre dispositivos. O Project Roma permite diferentes recursos que conectam diferentes serviços e pontos de extremidade do cliente quando o usuário entra com a mesma conta da Microsoft ou conta corporativa ou de estudante. Isso permite que você implemente experiências entre dispositivos e várias plataformas centradas em tarefas do usuário, em vez de dispositivos. '
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: ailae
ms.openlocfilehash: 3ebff1e816ee04a9bd6ffdbc0188cbb0b8015895
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029054"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="6709b-105">Usar a API do Microsoft Graph para trabalhar com o Project Roma</span><span class="sxs-lookup"><span data-stu-id="6709b-105">Use the Microsoft Graph API to work with Project Rome</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6709b-106">O [Project Roma](https://developer.microsoft.com/en-us/windows/project-rome) é uma iniciativa da Microsoft para criar uma plataforma que permite aos desenvolvedores de aplicativos criar grandes experiências entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6709b-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a platform that enables app developers to build great cross-device experiences.</span></span> <span data-ttu-id="6709b-107">O Project Roma permite diferentes recursos que conectam diferentes serviços e pontos de extremidade do cliente quando o usuário entra com a mesma conta da Microsoft ou conta corporativa ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="6709b-107">Project Rome enables different capabilities that connect different services and client endpoints when the user signs in with the same Microsoft account or work or school account.</span></span> <span data-ttu-id="6709b-108">Isso permite que você implemente experiências entre dispositivos e várias plataformas centradas em tarefas do usuário, em vez de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6709b-108">This allows you to implement cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="6709b-109">Três principais recursos de Roma do projeto são expostos pelo Microsoft Graph para ajudá-lo a habilitar excelentes experiências entre dispositivos: atividades, dispositivos e notificações.</span><span class="sxs-lookup"><span data-stu-id="6709b-109">Three key Project Rome capabilities are exposed via Microsoft Graph to help you enable great cross-device experiences: activities, devices, and notifications.</span></span>

## <a name="activities"></a><span data-ttu-id="6709b-110">Atividades</span><span class="sxs-lookup"><span data-stu-id="6709b-110">Activities</span></span>

<span data-ttu-id="6709b-111">As atividades no Microsoft Graph permitem que você direcionar o compromisso do usuário com seus aplicativos entre dispositivos e plataformas.</span><span class="sxs-lookup"><span data-stu-id="6709b-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="6709b-112">Uma atividade é a unidade de contrato de usuário e consiste em três componentes:</span><span class="sxs-lookup"><span data-stu-id="6709b-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="6709b-113">Um link profundo</span><span class="sxs-lookup"><span data-stu-id="6709b-113">A deep link</span></span>
- <span data-ttu-id="6709b-114">Uma representação visual</span><span class="sxs-lookup"><span data-stu-id="6709b-114">A visual representation</span></span>
- <span data-ttu-id="6709b-115">Metadados de conteúdo que descrevem a atividade, usando o [https://schema.org/](https://schema.org/) vocabulário compartilhado</span><span class="sxs-lookup"><span data-stu-id="6709b-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="6709b-116">Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de envolvimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="6709b-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="6709b-117">Cada vez que um usuário reparticipa de uma atividade, um novo item de histórico é adicionado à atividade para acumular o envolvimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="6709b-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="6709b-118">Quando um aplicativo publica objetos de atividade do usuário, o objeto aparecerá em algumas das novas superfícies de interface de usuário no Windows; por exemplo, notificações e cronograma da Cortana.</span><span class="sxs-lookup"><span data-stu-id="6709b-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="6709b-119">Você pode especificar tanto metadados avançados (para permitir que as atividades sejam apresentadas no contexto certo) e Visual ricos (usando a marcação de [cartão adaptável](https://adaptivecards.io/) ) em seus objetos de atividade.</span><span class="sxs-lookup"><span data-stu-id="6709b-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="6709b-120">Você pode usar as seguintes APIs do Microsoft Graph para criar e recuperar atividades do usuário:</span><span class="sxs-lookup"><span data-stu-id="6709b-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="6709b-121">Criar ou substituir atividade</span><span class="sxs-lookup"><span data-stu-id="6709b-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="6709b-122">Obter atividades</span><span class="sxs-lookup"><span data-stu-id="6709b-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="6709b-123">Obter atividades recentes</span><span class="sxs-lookup"><span data-stu-id="6709b-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="6709b-124">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="6709b-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="6709b-125">Criar ou substituir um item do histórico</span><span class="sxs-lookup"><span data-stu-id="6709b-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="6709b-126">Excluir um item do histórico</span><span class="sxs-lookup"><span data-stu-id="6709b-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a><span data-ttu-id="6709b-127">Dispositivos</span><span class="sxs-lookup"><span data-stu-id="6709b-127">Devices</span></span>

<span data-ttu-id="6709b-128">Você pode usar as APIs do Project Roma no Microsoft Graph para:</span><span class="sxs-lookup"><span data-stu-id="6709b-128">You can use Project Rome APIs in Microsoft Graph to:</span></span>

- <span data-ttu-id="6709b-129">Descobrir e conectar a dispositivos do usuário</span><span class="sxs-lookup"><span data-stu-id="6709b-129">Discover and connect to user's devices</span></span>
- <span data-ttu-id="6709b-130">Iniciar remotamente aplicativos nesses dispositivos</span><span class="sxs-lookup"><span data-stu-id="6709b-130">Remotely launch apps on those devices</span></span>
- <span data-ttu-id="6709b-131">Enviar mensagens para seus aplicativos nesses dispositivos</span><span class="sxs-lookup"><span data-stu-id="6709b-131">Send messages to your apps on those devices</span></span>

<span data-ttu-id="6709b-132">Com essas APIs, você pode criar aplicativos que criam experiências ricas que transcendem um único dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6709b-132">With these APIs, you can build apps that create rich experiences that transcend a single device.</span></span> <span data-ttu-id="6709b-133">Por exemplo, você pode estender seu aplicativo para iniciar em uma tela maior.</span><span class="sxs-lookup"><span data-stu-id="6709b-133">For example, you can extend your app to launch on a bigger screen.</span></span> <span data-ttu-id="6709b-134">Ou você pode criar uma experiência complementar para um aplicativo em outro dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6709b-134">Or you can create a companion experience for an app on another of the user's devices.</span></span>

<span data-ttu-id="6709b-135">Você pode usar as seguintes APIs do Microsoft Graph para se comunicar com outros dispositivos do Windows:</span><span class="sxs-lookup"><span data-stu-id="6709b-135">You can use the following Microsoft Graph APIs to communicate with other Windows devices:</span></span>

- [<span data-ttu-id="6709b-136">Listar os dispositivos do usuário</span><span class="sxs-lookup"><span data-stu-id="6709b-136">List the user's devices</span></span>](../api/user-list-devices.md)
- [<span data-ttu-id="6709b-137">Enviar um comando para um dispositivo</span><span class="sxs-lookup"><span data-stu-id="6709b-137">Send a command to a device</span></span>](../api/send-device-command.md)
- [<span data-ttu-id="6709b-138">Obter status do comando</span><span class="sxs-lookup"><span data-stu-id="6709b-138">Get command status</span></span>](../api/get-device-command-status.md)

## <a name="whats-new"></a><span data-ttu-id="6709b-139">Novidades</span><span class="sxs-lookup"><span data-stu-id="6709b-139">What's new</span></span>
<span data-ttu-id="6709b-140">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="6709b-140">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

