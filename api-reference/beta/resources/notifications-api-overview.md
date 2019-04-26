---
title: Usar as API REST de notificações no Microsoft Graph
description: Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário. Basta informar uma conta de usuário à qual enviar uma notificação e a plataforma entregará a notificação a todos os pontos de extremidade do dispositivo. As solicitações de API de notificações são executadas em nome de um usuário por meio de permissões delegadas e a [permissão de notificação]( /graph/permissions_reference), que pode ser usado com contas Microsoft ou contas corporativas ou de estudante.
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 243f412162ed1427c766272d02d58c57ba47cf42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342097"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="6ad2c-105">Usar as API REST de notificações no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6ad2c-105">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ad2c-106">Você pode usar as API de notificações do Microsoft Graph para enviar notificações por push para um usuário.</span><span class="sxs-lookup"><span data-stu-id="6ad2c-106">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="6ad2c-107">Basta informar uma conta de usuário à qual enviar uma notificação e a plataforma entregará a notificação a todos os pontos de extremidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ad2c-107">Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints.</span></span> <span data-ttu-id="6ad2c-108">As solicitações de API de notificações são executadas em nome de um usuário por meio de [permissões delegadas](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) e da [permissão de notificação]( /graph/permissions_reference), que podem ser usadas com contas Microsoft ou contas corporativas ou de estudante.</span><span class="sxs-lookup"><span data-stu-id="6ad2c-108">Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.</span></span>
<span data-ttu-id="6ad2c-109">Esse tipo de notificação no centro de usuário é representado pelo recurso [notification](../resources/projectrome-notification.md) e armazenado no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6ad2c-109">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="6ad2c-110">Ele pode ser acessado e gerenciado pelo aplicativo de publicação por meio das [APIs de SDK do Projeto Rome ](https://github.com/Microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="6ad2c-110">It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="next-steps"></a><span data-ttu-id="6ad2c-111">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6ad2c-111">Next steps</span></span>
- <span data-ttu-id="6ad2c-112">Confira o [recurso notification](../resources/projectrome-notification.md) e crie notificações para interagir com os usuários.</span><span class="sxs-lookup"><span data-stu-id="6ad2c-112">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="6ad2c-113">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6ad2c-113">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
