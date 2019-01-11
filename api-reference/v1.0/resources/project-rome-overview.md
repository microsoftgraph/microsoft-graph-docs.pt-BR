---
title: Usar a API do Microsoft Graph para trabalhar com o Project Roma
description: Project Roma é uma iniciativa da Microsoft para criar uma referência cruzada de dispositivo experiências de plataforma. Project Roma permite que um aplicativo em um cliente local ou serviço interagir com aplicativos e serviços em um host remoto quando o usuário entra com a mesma conta da Microsoft que eles usam para entrar no dispositivo do cliente. Isso permite que você programa entre dispositivos plataforma cruzada experiências e que são centralizadas em torno de tarefas do usuário, em vez dos dispositivos.
localization_priority: Normal
ms.openlocfilehash: d103bb68560a39cc4491460969a36bb81bb6da44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840961"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="ecb66-105">Usar a API do Microsoft Graph para trabalhar com o Project Roma</span><span class="sxs-lookup"><span data-stu-id="ecb66-105">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="ecb66-106">[Project Roma](https://developer.microsoft.com/en-us/windows/project-rome) é uma iniciativa da Microsoft para criar uma referência cruzada de dispositivo experiências de plataforma.</span><span class="sxs-lookup"><span data-stu-id="ecb66-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="ecb66-107">Project Roma permite que um aplicativo em um cliente local ou serviço interagir com aplicativos e serviços em um host remoto quando o usuário entra com a mesma conta da Microsoft que eles usam para entrar no dispositivo do cliente.</span><span class="sxs-lookup"><span data-stu-id="ecb66-107">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="ecb66-108">Isso permite que você programa entre dispositivos plataforma cruzada experiências e que são centralizadas em torno de tarefas do usuário, em vez dos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ecb66-108">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="ecb66-109">Um componente-chave é exposto por meio do Microsoft Graph para habilitar essas experiências: atividades.</span><span class="sxs-lookup"><span data-stu-id="ecb66-109">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="ecb66-110">Atividades</span><span class="sxs-lookup"><span data-stu-id="ecb66-110">Activities</span></span>

<span data-ttu-id="ecb66-111">Atividades no Microsoft Graph habilitar compromisso do usuário de unidade com seus aplicativos em plataformas e dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ecb66-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="ecb66-112">Uma atividade é a unidade de compromisso do usuário e consiste em três componentes:</span><span class="sxs-lookup"><span data-stu-id="ecb66-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="ecb66-113">Um link profundo</span><span class="sxs-lookup"><span data-stu-id="ecb66-113">A deep link</span></span>
- <span data-ttu-id="ecb66-114">Uma representação visual</span><span class="sxs-lookup"><span data-stu-id="ecb66-114">A visual representation</span></span>
- <span data-ttu-id="ecb66-115">Metadados do conteúdo que descreve a atividade, usando o [https://schema.org/](https://schema.org/) shared vocabulário</span><span class="sxs-lookup"><span data-stu-id="ecb66-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="ecb66-116">Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de participação do usuário.</span><span class="sxs-lookup"><span data-stu-id="ecb66-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="ecb66-117">Cada vez que um usuário reengages com uma atividade, um novo item de histórico é adicionado à atividade acumular compromisso do usuário.</span><span class="sxs-lookup"><span data-stu-id="ecb66-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="ecb66-118">Quando um aplicativo publica objetos de atividade do usuário, o objeto será mostrada no algumas das novas superfícies de interface do usuário no Windows; Por exemplo, Cortana notificações e linha do tempo.</span><span class="sxs-lookup"><span data-stu-id="ecb66-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="ecb66-119">Você pode especificar metadados sofisticados (para permitir atividades a serem apresentados no contexto certo) e o ricas visuais (usando marcação [Cartão adaptável](https://adaptivecards.io/) ) em seus objetos de atividade.</span><span class="sxs-lookup"><span data-stu-id="ecb66-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="ecb66-120">Você pode usar as seguintes APIs do Microsoft Graph para criar e recuperar as atividades do usuário:</span><span class="sxs-lookup"><span data-stu-id="ecb66-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="ecb66-121">Criar ou substituir atividade</span><span class="sxs-lookup"><span data-stu-id="ecb66-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="ecb66-122">Obter atividades</span><span class="sxs-lookup"><span data-stu-id="ecb66-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="ecb66-123">Obter atividades recentes</span><span class="sxs-lookup"><span data-stu-id="ecb66-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="ecb66-124">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="ecb66-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="ecb66-125">Criar ou substituir um item do histórico</span><span class="sxs-lookup"><span data-stu-id="ecb66-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="ecb66-126">Excluir um item do histórico</span><span class="sxs-lookup"><span data-stu-id="ecb66-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

