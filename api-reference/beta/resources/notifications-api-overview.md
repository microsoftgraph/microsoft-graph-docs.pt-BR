---
title: Usar as API REST de notificações no Microsoft Graph
description: Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. .
localization_priority: Priority
ms.prod: notifications
doc_type: conceptualPageType
author: merzink
ms.openlocfilehash: 96b27aa9a57c26666ae9b4fc09c4dadca52b8d6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033654"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="315ee-104">Usar as API REST de notificações no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="315ee-104">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="315ee-105">Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário.</span><span class="sxs-lookup"><span data-stu-id="315ee-105">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="315ee-106">Basta publicar uma notificação para o usuário de destino e a plataforma entregará a notificação a todos os pontos de extremidade de dispositivos registrados para aquele usuário.</span><span class="sxs-lookup"><span data-stu-id="315ee-106">Simply post a notification to your target user, and the platform will deliver the notification to all device endpoints registered to that user.</span></span> <span data-ttu-id="315ee-107">O fluxo de alto nível ocorre da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="315ee-107">The high-level flow is as follows:</span></span>

1. <span data-ttu-id="315ee-108">O usuário entra no aplicativo, o que cria uma assinatura com o serviço de notificação do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="315ee-108">User signs in to your application, which creates a subscription with the Microsoft Graph notification service.</span></span> <span data-ttu-id="315ee-109">Uma ID de assinatura de notificação de usuário específica ou UNSID é retornada para o aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="315ee-109">A specific user notification subscription ID or UNSID will be returned to the calling application.</span></span>
2. <span data-ttu-id="315ee-110">O aplicativo envia essa UNSID para o serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="315ee-110">The application sends this UNSID to your application service.</span></span>
3. <span data-ttu-id="315ee-111">Quando a notificação estiver pronta para envio, o serviço de aplicativo a [autenticará em uma plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) e a publicará por meio do serviço de notificação do Microsoft Graph, fornecendo o token de autenticação, a UNSID do usuário de destino e o conteúdo da notificação.</span><span class="sxs-lookup"><span data-stu-id="315ee-111">When ready to send a notification, your application service [authenticates with the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) and posts a notification via the Microsoft Graph notification service, providing the auth token, target user's UNSID, and notification payload.</span></span>
4. <span data-ttu-id="315ee-112">O serviço de notificação do Microsoft Graph distribui as notificações para todos os pontos de extremidade do usuário que tenham uma assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="315ee-112">The Microsoft Graph notification service fans-out notifications to all endpoints of the user with an active subscription.</span></span>  

<span data-ttu-id="315ee-113">Esse tipo de notificação centrada no usuário é representado pelo recurso [notificação](../resources/projectrome-notification.md) e armazenado no serviço de notificação do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="315ee-113">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored within the Microsoft Graph notification service.</span></span> <span data-ttu-id="315ee-114">Pode ser acessado e gerenciado pelo aplicativo do cliente por meio das [APIs do SDK do lado do cliente](https://aka.ms/GNSDK).</span><span class="sxs-lookup"><span data-stu-id="315ee-114">It can then be accessed and managed by the client application via the [client-side SDK APIs](https://aka.ms/GNSDK).</span></span> <span data-ttu-id="315ee-115">Se você não conhece o serviço de notificação do Microsoft Graph, confira a seção [visão geral da notificação](https://docs.microsoft.com/graph/notifications-concept-overview) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="315ee-115">If you're new to the Microsoft Graph notification service, check out the [notification overview](https://docs.microsoft.com/graph/notifications-concept-overview) section to learn more.</span></span>    

## <a name="whats-new"></a><span data-ttu-id="315ee-116">Novidades</span><span class="sxs-lookup"><span data-stu-id="315ee-116">What's new</span></span>
<span data-ttu-id="315ee-117">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="315ee-117">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="315ee-118">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="315ee-118">Next steps</span></span>
- <span data-ttu-id="315ee-119">Confira o [recurso notification](../resources/projectrome-notification.md) e crie notificações para interagir com os usuários.</span><span class="sxs-lookup"><span data-stu-id="315ee-119">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="315ee-120">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="315ee-120">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="315ee-121">Comece com a integração com o cliente seguindo as etapas descritas no tópico [visão geral da integração](/graph/notifications-integration-e2e-overview).</span><span class="sxs-lookup"><span data-stu-id="315ee-121">Get started with client integration by following the steps in the [integration overview](/graph/notifications-integration-e2e-overview) topic.</span></span>


