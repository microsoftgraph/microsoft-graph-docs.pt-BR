---
title: Criar e enviar uma notificação do serviço de aplicativo
description: 'Configure o serviço de aplicativo para enviar notificações centradas no usuário para vários clientes por meio do Microsoft Graph. '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: 1148c554b90fca5aeb56627e47a1d060f53f772e
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063218"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a><span data-ttu-id="db6b5-103">Criar e enviar uma notificação do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="db6b5-103">Create and send a notification from your app service</span></span>

<span data-ttu-id="db6b5-104">Você pode criar e enviar uma notificação para um usuário com as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="db6b5-104">You can create and send a notification to a user by using Microsoft Graph APIs.</span></span> <span data-ttu-id="db6b5-105">A notificação é armazenada no repositório do feed de atividades e enviada para todos os clientes do aplicativo em todos os dispositivos que o usuário alvo estiver conectado. Veja abaixo para saber como autenticar, permissão necessária de escopos, cabeçalho/corpo de solicitação e resposta esperada.</span><span class="sxs-lookup"><span data-stu-id="db6b5-105">The notification is stored in the activity feed store and is sent to all app clients on all devices that the target user is signed in on.See below to learn how to authenticate, required permission scopes, request header/body and expected response.</span></span>

## <a name="authentication"></a><span data-ttu-id="db6b5-106">Autenticação</span><span class="sxs-lookup"><span data-stu-id="db6b5-106">Authentication</span></span>

<span data-ttu-id="db6b5-107">As notificações do Microsoft Graph exige que o serviço de aplicativo use o fluxo On-Behalf-Of (OBO) para postar uma notificação ao usuário.</span><span class="sxs-lookup"><span data-stu-id="db6b5-107">Microsoft Graph notifications requires that your application service uses the On-Behalf-Of (OBO) flow to post a notification to a user.</span></span> <span data-ttu-id="db6b5-108">O fluxo de autenticação é o demonstrado a seguir::</span><span class="sxs-lookup"><span data-stu-id="db6b5-108">The following is a simple and typical authentication flow:</span></span>

1.  <span data-ttu-id="db6b5-109">O usuário entra no aplicativo com a conta corporativa ou de estudante da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="db6b5-109">The user signs in to your application with their Microsoft or their work or school account.</span></span> <span data-ttu-id="db6b5-110">Ao entrar, o serviço de identidade concede um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="db6b5-110">When they sign in, the identity service gives you an access token.</span></span>

2.  <span data-ttu-id="db6b5-111">Você envia o token de acesso ao serviço do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db6b5-111">You send the access token to your app service.</span></span>

3.  <span data-ttu-id="db6b5-112">O serviço do aplicativo autentica no serviço de identidade e solicita um token OBO para as notificações do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="db6b5-112">You app service authenticates against the identity service and requests an OBO token for Microsoft Graph notifications.</span></span>

4.  <span data-ttu-id="db6b5-113">O serviço de identidade retorna um token com base em OBO e um token de atualização.</span><span class="sxs-lookup"><span data-stu-id="db6b5-113">The identity service returns an OBO-based token and a refresh token.</span></span> <span data-ttu-id="db6b5-114">O serviço de aplicativo pode usar o token de acesso para postar notificações ao usuário.</span><span class="sxs-lookup"><span data-stu-id="db6b5-114">Your app service can use this access token to post notifications to this user.</span></span>

<span data-ttu-id="db6b5-115">Para saber mais sobre o fluxo OAuth 2.0 OBO, consulte [Chamadas de serviço a serviço que usam a identidade do usuário delegado no fluxo On-Behalf-Of](https://docs.microsoft.com/pt-BR/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow).</span><span class="sxs-lookup"><span data-stu-id="db6b5-115">To learn more about OAuth 2.0 OBO flow, see [Service-to-service calls that use delegated user identity in the On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow).</span></span> <span data-ttu-id="db6b5-116">Para saber mais sobre como esse fluxo funciona com as notificações do Microsoft Graph, confira o [exemplo de serviço do aplicativo](https://aka.ms/gnsample-appservice).</span><span class="sxs-lookup"><span data-stu-id="db6b5-116">For details about how this flow works with Microsoft Graph notifications, see the [App Service sample](https://aka.ms/gnsample-appservice).</span></span>

> [!NOTE]
> <span data-ttu-id="db6b5-117">As notificações do Microsoft Graph usa atualmente o fluxo de autenticação OBO com planos futuros para simplificar essa autenticação e acabar com a necessidade de manter tokens de acesso e tokens de atualização.</span><span class="sxs-lookup"><span data-stu-id="db6b5-117">Microsoft Graph notifications currently uses OBO authentication flow with future plans to simplify this authentication further and eliminate the need to maintain access tokens and refresh tokens.</span></span>

<span data-ttu-id="db6b5-118">Para obter mais detalhes sobre as APIs de permissão e nos cabeçalhos de solicitação e de resposta, confira [Criar e enviar uma notificação](/graph/api/notifications-post) na seção de referência da API.</span><span class="sxs-lookup"><span data-stu-id="db6b5-118">For more details on the API permissions and on the request and response headers, please see [Create and send a notification](/graph/api/notifications-post) in API reference section.</span></span> 
