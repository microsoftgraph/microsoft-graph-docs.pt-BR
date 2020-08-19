---
title: Usar a API do Microsoft Graph para trabalhar com o Project Roma
description: O Project Roma é uma iniciativa da Microsoft para criar uma plataforma de experiências entre dispositivos. O Project Roma permite que um aplicativo em um cliente ou serviço local interaja com aplicativos e serviços em um host remoto quando o usuário entrar com a mesma conta da Microsoft que eles usam para entrar no dispositivo cliente. Isso permite programar experiências entre dispositivos e várias plataformas centradas em tarefas do usuário, em vez de dispositivos.
localization_priority: Normal
author: ailae
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: f7e68c50e6e58c4f9f7a2b04bf2f26361fef6063
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806972"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a><span data-ttu-id="8b32e-105">Usar a API do Microsoft Graph para trabalhar com o Project Roma</span><span class="sxs-lookup"><span data-stu-id="8b32e-105">Use the Microsoft Graph API to work with Project Rome</span></span>

<span data-ttu-id="8b32e-106">O [Project Roma](https://developer.microsoft.com/en-us/windows/project-rome) é uma iniciativa da Microsoft para criar uma plataforma de experiências entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8b32e-106">[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) is a Microsoft initiative to build a cross-device experiences platform.</span></span> <span data-ttu-id="8b32e-107">O Project Roma permite que um aplicativo em um cliente ou serviço local interaja com aplicativos e serviços em um host remoto quando o usuário entrar com a mesma conta da Microsoft que eles usam para entrar no dispositivo cliente.</span><span class="sxs-lookup"><span data-stu-id="8b32e-107">Project Rome enables an app on a local client or service to interact with apps and services on a remote host when the user signs in with the same Microsoft account that they use to sign in on the client device.</span></span> <span data-ttu-id="8b32e-108">Isso permite programar experiências entre dispositivos e várias plataformas centradas em tarefas do usuário, em vez de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8b32e-108">This allows you to program cross-device and cross-platform experiences that are centered around user tasks rather than devices.</span></span>

<span data-ttu-id="8b32e-109">Um componente importante é exposto pelo Microsoft Graph para habilitar essas experiências: atividades.</span><span class="sxs-lookup"><span data-stu-id="8b32e-109">A key component is exposed via Microsoft Graph to enable these experiences: activities.</span></span>

## <a name="activities"></a><span data-ttu-id="8b32e-110">Atividades</span><span class="sxs-lookup"><span data-stu-id="8b32e-110">Activities</span></span>

<span data-ttu-id="8b32e-111">As atividades no Microsoft Graph permitem que você direcionar o compromisso do usuário com seus aplicativos entre dispositivos e plataformas.</span><span class="sxs-lookup"><span data-stu-id="8b32e-111">Activities in Microsoft Graph enable you to drive user engagement with your apps across devices and platforms.</span></span> <span data-ttu-id="8b32e-112">Uma atividade é a unidade de contrato de usuário e consiste em três componentes:</span><span class="sxs-lookup"><span data-stu-id="8b32e-112">An activity is the unit of user engagement, and consists of three components:</span></span>

- <span data-ttu-id="8b32e-113">Um link profundo</span><span class="sxs-lookup"><span data-stu-id="8b32e-113">A deep link</span></span>
- <span data-ttu-id="8b32e-114">Uma representação visual</span><span class="sxs-lookup"><span data-stu-id="8b32e-114">A visual representation</span></span>
- <span data-ttu-id="8b32e-115">Metadados de conteúdo que descrevem a atividade, usando o [https://schema.org/](https://schema.org/) vocabulário compartilhado</span><span class="sxs-lookup"><span data-stu-id="8b32e-115">Content metadata that describes the activity, using the [https://schema.org/](https://schema.org/) shared vocabulary</span></span>

<span data-ttu-id="8b32e-116">Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de envolvimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b32e-116">When a session is created by an application, a history item is added to the activity to reflect the period of user engagement.</span></span> <span data-ttu-id="8b32e-117">Cada vez que um usuário reparticipa de uma atividade, um novo item de histórico é adicionado à atividade para acumular o envolvimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b32e-117">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

<span data-ttu-id="8b32e-118">Quando um aplicativo publica objetos de atividade do usuário, o objeto aparecerá em algumas das novas superfícies de interface de usuário no Windows; por exemplo, notificações e cronograma da Cortana.</span><span class="sxs-lookup"><span data-stu-id="8b32e-118">When an application publishes user activity objects, the object will show up in some of the new UI surfaces in Windows; for example, Cortana Notifications and Timeline.</span></span> <span data-ttu-id="8b32e-119">Você pode especificar tanto metadados avançados (para permitir que as atividades sejam apresentadas no contexto certo) e Visual ricos (usando a marcação de [cartão adaptável](https://adaptivecards.io/) ) em seus objetos de atividade.</span><span class="sxs-lookup"><span data-stu-id="8b32e-119">You can specify both rich metadata (to allow activities to be presented in just the right context) and rich visuals (using [Adaptive Card](https://adaptivecards.io/) markup) in your activity objects.</span></span>

<span data-ttu-id="8b32e-120">Você pode usar as seguintes APIs do Microsoft Graph para criar e recuperar atividades do usuário:</span><span class="sxs-lookup"><span data-stu-id="8b32e-120">You can use the following Microsoft Graph APIs to create and retrieve user activities:</span></span>

- [<span data-ttu-id="8b32e-121">Criar ou substituir atividade</span><span class="sxs-lookup"><span data-stu-id="8b32e-121">Create or replace activity</span></span>](../api/projectrome-put-activity.md)
- [<span data-ttu-id="8b32e-122">Obter atividades</span><span class="sxs-lookup"><span data-stu-id="8b32e-122">Get activities</span></span>](../api/projectrome-get-activities.md)
- [<span data-ttu-id="8b32e-123">Obter atividades recentes</span><span class="sxs-lookup"><span data-stu-id="8b32e-123">Get recent activities</span></span>](../api/projectrome-get-recent-activities.md)
- [<span data-ttu-id="8b32e-124">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="8b32e-124">Delete an activity</span></span>](../api/projectrome-delete-activity.md)
- [<span data-ttu-id="8b32e-125">Criar ou substituir um item do histórico</span><span class="sxs-lookup"><span data-stu-id="8b32e-125">Create or replace a history item</span></span>](../api/projectrome-put-historyitem.md)
- [<span data-ttu-id="8b32e-126">Excluir um item do histórico</span><span class="sxs-lookup"><span data-stu-id="8b32e-126">Delete a history item</span></span>](../api/projectrome-delete-historyitem.md)

## <a name="whats-new"></a><span data-ttu-id="8b32e-127">Novidades</span><span class="sxs-lookup"><span data-stu-id="8b32e-127">What's new</span></span>
<span data-ttu-id="8b32e-128">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="8b32e-128">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>