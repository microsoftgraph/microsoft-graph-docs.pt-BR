---
title: Usar as API REST de notificações no Microsoft Graph
description: Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. .
localization_priority: Priority
ms.prod: notifications
doc_type: conceptualPageType
author: merzink
ms.openlocfilehash: e48259463377e14a84c3010e229ccd31c29ec6ec
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938895"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="b6509-104">Usar as API REST de notificações no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b6509-104">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6509-105">Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário.</span><span class="sxs-lookup"><span data-stu-id="b6509-105">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="b6509-106">Basta publicar uma notificação para o usuário de destino e a plataforma entregará a notificação a todos os pontos de extremidade de dispositivos registrados para aquele usuário.</span><span class="sxs-lookup"><span data-stu-id="b6509-106">Simply post a notification to your target user, and the platform will deliver the notification to all device endpoints registered to that user.</span></span> <span data-ttu-id="b6509-107">O fluxo de alto nível ocorre da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="b6509-107">The high-level flow is as follows:</span></span>

1. <span data-ttu-id="b6509-108">O usuário entra no aplicativo, o que cria uma assinatura com o serviço de notificação do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b6509-108">User signs in to your application, which creates a subscription with the Microsoft Graph notification service.</span></span> <span data-ttu-id="b6509-109">Uma ID de assinatura de notificação de usuário específica ou UNSID é retornada para o aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="b6509-109">A specific user notification subscription ID or UNSID will be returned to the calling application.</span></span>
2. <span data-ttu-id="b6509-110">O aplicativo envia essa UNSID para o serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6509-110">The application sends this UNSID to your application service.</span></span>
3. <span data-ttu-id="b6509-111">Quando a notificação estiver pronta para envio, o serviço de aplicativo a [autenticará em uma plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) e a publicará por meio do serviço de notificação do Microsoft Graph, fornecendo o token de autenticação, a UNSID do usuário de destino e o conteúdo da notificação.</span><span class="sxs-lookup"><span data-stu-id="b6509-111">When ready to send a notification, your application service [authenticates with the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v1-oauth2-client-creds-grant-flow) and posts a notification via the Microsoft Graph notification service, providing the auth token, target user's UNSID, and notification payload.</span></span>
4. <span data-ttu-id="b6509-112">O serviço de notificação do Microsoft Graph distribui as notificações para todos os pontos de extremidade do usuário que tenham uma assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="b6509-112">The Microsoft Graph notification service fans-out notifications to all endpoints of the user with an active subscription.</span></span>  

<span data-ttu-id="b6509-113">Esse tipo de notificação centrada no usuário é representado pelo recurso [notificação](../resources/projectrome-notification.md) e armazenado no serviço de notificação do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b6509-113">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="b6509-114">Pode ser acessado e gerenciado pelo aplicativo do cliente por meio das [APIs do SDK do lado do cliente](https://aka.ms/GNSDK).</span><span class="sxs-lookup"><span data-stu-id="b6509-114">It can then be accessed and managed by the publishing app via the [client side SDK APIs](https://aka.ms/GNSDK).</span></span> <span data-ttu-id="b6509-115">Se você não conhece o serviço de notificação do Microsoft Graph, confira a seção [visão geral da notificação](https://docs.microsoft.com/graph/notifications-concept-overview) para saber mais.</span><span class="sxs-lookup"><span data-stu-id="b6509-115">If you're new to the Microsoft Graph notification service, check out the [notification overview](https://docs.microsoft.com/graph/notifications-concept-overview) section to learn more.</span></span>    


## <a name="next-steps"></a><span data-ttu-id="b6509-116">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b6509-116">Next steps</span></span>
- <span data-ttu-id="b6509-117">Confira o [recurso notification](../resources/projectrome-notification.md) e crie notificações para interagir com os usuários.</span><span class="sxs-lookup"><span data-stu-id="b6509-117">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="b6509-118">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b6509-118">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="b6509-119">Comece com a integração com o cliente seguindo as etapas descritas no tópico [visão geral da integração](/graph/notifications-integration-e2e-overview).</span><span class="sxs-lookup"><span data-stu-id="b6509-119">Get started with client integration, following the steps outlined in the [integration overview](/graph/notifications-integration-e2e-overview).</span></span>
