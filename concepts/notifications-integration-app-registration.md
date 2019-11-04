---
title: Gerenciar registro do aplicativo e permissão de API para notificações do Microsoft Graph
description: Para receber notificações enviadas pelo Microsoft Graph, primeiro é necessário registrar seu aplicativo no portal do Microsoft Azure.
localization_priority: Priority
ms.prod: notifications
author: merzink
ms.openlocfilehash: 5c22fb5bc39b5b609eaae958cec9ada55f74b9f0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934355"
---
# <a name="manage-app-registration-and-api-permission-for-microsoft-graph-notifications"></a><span data-ttu-id="fb294-103">Gerenciar registro do aplicativo e permissão de API para notificações do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fb294-103">Manage app registration and API permission for Microsoft Graph notifications</span></span>

<span data-ttu-id="fb294-104">Para que o serviço do aplicativo se integre às notificações do Microsoft Graph, é necessário registrar seu aplicativo na Microsoft Identity Platform para suporte às contas corporativas ou de estudante da Microsoft e declarar as permissões de API obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="fb294-104">In order for your application service to integrate with Microsoft Graph notifications, you need to register your app with the Microsoft identity platform to support Microsoft accounts or work or school accounts, and declare the API permissions that are required.</span></span>

## <a name="register-your-app-to-support-microsoft-accounts-or-work-or-school-accounts"></a><span data-ttu-id="fb294-105">Registre seu aplicativo para suporte às contas corporativas ou de estudante da Microsoft</span><span class="sxs-lookup"><span data-stu-id="fb294-105">Register your app to support Microsoft accounts or work or school accounts</span></span>

<span data-ttu-id="fb294-106">Registre seu aplicativo no portal do [Microsoft Azure](https://portal.azure.com/#home) para suporte às contas corporativas ou de estudante da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fb294-106">Register your application on the [Microsoft Azure portal](https://portal.azure.com/#home) to support Microsoft accounts or work or school accounts.</span></span> <span data-ttu-id="fb294-107">Se já tiver registrado o aplicativo anteriormente no [Portal do aplicativo da Microsoft](https://apps.dev.microsoft.com/), os aplicativos existentes serão exibidos na nova e melhorada experiência do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fb294-107">If you’ve previously registered your application on the [Microsoft Application Portal](https://apps.dev.microsoft.com/), your existing apps will show up in the new and improved Azure portal experience.</span></span>

<span data-ttu-id="fb294-108">Para saber como registrar aplicativos, confira [Registrar um aplicativo na Microsoft Identity Platform](auth-register-app-v2.md).</span><span class="sxs-lookup"><span data-stu-id="fb294-108">For information about how to register your apps, see [Register an application with the Microsoft identity platform](auth-register-app-v2.md).</span></span> <span data-ttu-id="fb294-109">Ao registrar seu aplicativo, certifique-se de manter sempre à mão a ID do aplicativo/ID do cliente.</span><span class="sxs-lookup"><span data-stu-id="fb294-109">When you register your app, keep the application ID/client ID somewhere handy.</span></span> <span data-ttu-id="fb294-110">Essa ID será usada posteriormente ao registrar seu aplicativo para experiências entre dispositivos no [Microsoft Partner Center](https://partner.microsoft.com/) para clientes Windows, Android ou iOS.</span><span class="sxs-lookup"><span data-stu-id="fb294-110">You'll need this ID later when you register your application for cross-device experiences in the [Microsoft Partner Center](https://partner.microsoft.com/).</span></span>

> [!NOTE]
> <span data-ttu-id="fb294-111">Se ainda não tiver uma conta da Microsoft e quiser usar uma, acesse a página  [conta da Microsoft](https://account.microsoft.com/account).</span><span class="sxs-lookup"><span data-stu-id="fb294-111">If you don't already have a Microsoft account and would like to use one, go to the [Microsoft account](https://account.microsoft.com/account) page.</span></span> <span data-ttu-id="fb294-112">Se estiver desenvolvendo um aplicativo que usa o Azure AD versão 1.0 como uma estrutura de autenticação e identidade para contas corporativas ou de estudante, confira [Bibliotecas de Autenticação do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span><span class="sxs-lookup"><span data-stu-id="fb294-112">If you're writing an app that needs to use Azure AD v1.0 as an authentication and identity framework for work or school accounts, see [Azure Active Directory Authentication Libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span></span> <span data-ttu-id="fb294-113">Para saber mais sobre ou se estiver usando a nova Microsoft Identity Platform convergida (versão 2.0), confira [comparação do ponto de extremidade da Microsoft Identity Platform e o ponto de extremidade do Azure AD versão 1.0](https://docs.microsoft.com/azure/active-directory/develop/azure-ad-endpoint-comparison).</span><span class="sxs-lookup"><span data-stu-id="fb294-113">If you’re interested in learning about or using the new converged Microsoft identity platform (v2.0), see [Comparing the Microsoft identity platform endpoint and Azure AD v1.0 endpoint](https://docs.microsoft.com/azure/active-directory/develop/azure-ad-endpoint-comparison).</span></span>


## <a name="app-certificates-and-secrets"></a><span data-ttu-id="fb294-114">Certificados e segredos do aplicativo </span><span class="sxs-lookup"><span data-stu-id="fb294-114">App certificates and secrets</span></span>

<span data-ttu-id="fb294-115">Para que o aplicativo se identifique e se autentique ao obter tokens de autenticação, você pode carregar seu próprio certificado ou criar um nova segredo do cliente acessando **certificados e segredos** no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fb294-115">To enable your application to identify and authenticate itself when obtaining auth tokens, you can either upload your own certificate or create a new client secret by going to **Certificates & secrets** in the Azure portal.</span></span>
    
![Captura de tela de certificados e segredos do aplicativo no portal do Azure](images/notifications-app-secrets.png)
    
> [!NOTE]
> <span data-ttu-id="fb294-117">Se optar por gerar um novo segredo do cliente, certifique-se de copiá-lo a e guardá-lo em um local seguro.</span><span class="sxs-lookup"><span data-stu-id="fb294-117">If you opt to generate a new client secret, be sure to copy and keep it in a safe place.</span></span> <span data-ttu-id="fb294-118">Você não poderá acessá-lo novamente após sair do portal.</span><span class="sxs-lookup"><span data-stu-id="fb294-118">You won’t be able to access it again after you leave the portal.</span></span>

## <a name="api-permissions"></a><span data-ttu-id="fb294-119">Permissões de API</span><span class="sxs-lookup"><span data-stu-id="fb294-119">API permissions</span></span>

<span data-ttu-id="fb294-120">É preciso incluir permissões adicionais para usar as notificações do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb294-120">You'll need to add additional permissions in order to use Microsoft Graph notifications.</span></span> <span data-ttu-id="fb294-121">Escolha **Adicionar uma permissão**e, em APIs Microsoft, selecione **Microsoft Graph**e depois **Permissões delegadas**.</span><span class="sxs-lookup"><span data-stu-id="fb294-121">Choose **Add a permission**, and under Microsoft APIs, select **Microsoft Graph**, and then select **Delegated permissions**.</span></span>
    
![Captura de tela da página de permissões de API de solicitação do portal do Azure](images/notifications-api-permissions.png)
    
<span data-ttu-id="fb294-123">Adicione as seguintes permissões:</span><span class="sxs-lookup"><span data-stu-id="fb294-123">Add the following permissions:</span></span>

- <span data-ttu-id="fb294-124">User.Read – permite que o aplicativo conecte seu usuário</span><span class="sxs-lookup"><span data-stu-id="fb294-124">User.Read - allows your application to sign-in your user</span></span>

- <span data-ttu-id="fb294-125">UserActivity.ReadWrite.CreatedByApp – permite a assinatura do aplicativo para recuperação de notificação</span><span class="sxs-lookup"><span data-stu-id="fb294-125">UserActivity.ReadWrite.CreatedByApp - allows app subscription for notification retrieval</span></span>

![Captura de tela das permissões delegadas para notificações no portal do Azure](images/notifications-api-permissions-list.png)

## <a name="next-steps"></a><span data-ttu-id="fb294-127">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="fb294-127">Next steps</span></span>

<span data-ttu-id="fb294-128">Saiba mais sobre [permissões e consentimento](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) ou consulte a [referência de permissões](https://docs.microsoft.com/graph/permissions-reference) do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb294-128">Learn more about [permissions and consent](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) or see the Microsoft Graph [permissions reference](https://docs.microsoft.com/graph/permissions-reference).</span></span>

<span data-ttu-id="fb294-129">Após registrar seu aplicativo, visite o [Partner Center](https://partner.microsoft.com/) para configurar o aplicativo para direcionar suas plataformas de aplicativo correspondentes (Windows, iOS ou Android) para notificações enviadas pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb294-129">Now that you’ve registered your app, go to the [Partner Center](https://partner.microsoft.com/) to set up your application for cross-device experiences and to target your corresponding app platforms for notifications sent via Microsoft Graph.</span></span> <span data-ttu-id="fb294-130">Para saber mais, confira a [Integração à experiência entre dispositivos](notifications-integration-cross-device-experiences-onboarding.md).</span><span class="sxs-lookup"><span data-stu-id="fb294-130">For details, see [Onboarding to cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md).</span></span> 

>[!NOTE]
><span data-ttu-id="fb294-131">Se você estiver apenas direcionando pontos de extremidade da Web, poderá ignorar o registro do Partner Center e aprender a configurar seu [serviço de aplicativo](notifications-integrating-app-server.md) para enviar notificações.</span><span class="sxs-lookup"><span data-stu-id="fb294-131">If you're only targeting web endpoints, you can skip Partner Center registration and learn how to set up your [app service](notifications-integrating-app-server.md) to send notifications.</span></span>
