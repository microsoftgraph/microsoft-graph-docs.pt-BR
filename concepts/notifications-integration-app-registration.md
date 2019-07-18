---
title: Gerenciar registro do aplicativo e permissão de API para notificações do Microsoft Graph
description: Para receber notificações enviadas pelo Microsoft Graph, primeiro é necessário registrar seu aplicativo no portal do Microsoft Azure.
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: dc102f451b3f206bbfefe1d3c38c3995041f04fa
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778632"
---
# <a name="manage-app-registration-and-api-permission-for-microsoft-graph-notifications"></a><span data-ttu-id="ea5a5-103">Gerenciar registro do aplicativo e permissão de API para notificações do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ea5a5-103">Manage app registration and API permission for Microsoft Graph notifications</span></span>

<span data-ttu-id="ea5a5-104">Para que o serviço do aplicativo se integre às notificações do Microsoft Graph, é necessário registrar seu aplicativo na Microsoft Identity Platform para suporte às contas corporativas ou de estudante da Microsoft e declarar as permissões de API obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-104">In order for your application service to integrate with Microsoft Graph notifications, you need to register your app with the Microsoft identity platform to support Microsoft accounts or work or school accounts, and declare the API permissions that are required.</span></span>

## <a name="register-your-app-to-support-microsoft-accounts-or-work-or-school-accounts"></a><span data-ttu-id="ea5a5-105">Registre seu aplicativo para suporte às contas corporativas ou de estudante da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ea5a5-105">Register your app to support Microsoft accounts or work or school accounts</span></span>

<span data-ttu-id="ea5a5-106">Registre seu aplicativo no portal do [Microsoft Azure](https://portal.azure.com/#home) para suporte às contas corporativas ou de estudante da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-106">Register your application on the [Microsoft Azure portal](https://portal.azure.com/#home) to support Microsoft accounts or work or school accounts.</span></span> <span data-ttu-id="ea5a5-107">Se já tiver registrado o aplicativo anteriormente no [Portal do aplicativo da Microsoft](https://apps.dev.microsoft.com/), os aplicativos existentes serão exibidos na nova e melhorada experiência do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-107">If you’ve previously registered your application on the [Microsoft Application Portal](https://apps.dev.microsoft.com/), your existing apps will show up in the new and improved Azure portal experience.</span></span>

<span data-ttu-id="ea5a5-108">Para saber como registrar aplicativos, confira [Registrar um aplicativo na Microsoft Identity Platform](auth-register-app-v2.md).</span><span class="sxs-lookup"><span data-stu-id="ea5a5-108">For information about how to register your apps, see [Register an application with the Microsoft identity platform](auth-register-app-v2.md).</span></span> 


> [!NOTE]
> <span data-ttu-id="ea5a5-109">Se ainda não tiver uma conta da Microsoft e quiser usar uma, acesse a página  [conta da Microsoft](https://account.microsoft.com/account).</span><span class="sxs-lookup"><span data-stu-id="ea5a5-109">If you don't already have a Microsoft account and would like to use one, go to the [Microsoft account](https://account.microsoft.com/account) page.</span></span> <span data-ttu-id="ea5a5-110">Se estiver desenvolvendo um aplicativo que usa o Azure AD versão 1.0 como uma estrutura de autenticação e identidade para contas corporativas ou de estudante, confira [Bibliotecas de Autenticação do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span><span class="sxs-lookup"><span data-stu-id="ea5a5-110">If you're writing an app that needs to use Azure AD v1.0 as an authentication and identity framework for work or school accounts, see [Azure Active Directory Authentication Libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span></span> <span data-ttu-id="ea5a5-111">Para saber mais sobre ou se estiver usando a nova Microsoft Identity Platform convergida (versão 2.0), confira [comparação do ponto de extremidade da Microsoft Identity Platform e o ponto de extremidade do Azure AD versão 1.0](https://docs.microsoft.com/pt-BR/azure/active-directory/develop/azure-ad-endpoint-comparison).</span><span class="sxs-lookup"><span data-stu-id="ea5a5-111">If you’re interested in learning about or using the new converged Microsoft identity platform (v2.0), see [Comparing the Microsoft identity platform endpoint and Azure AD v1.0 endpoint](https://docs.microsoft.com/en-us/azure/active-directory/develop/azure-ad-endpoint-comparison).</span></span>

<span data-ttu-id="ea5a5-112">Ao registrar seu aplicativo, mantenha sempre à mão a ID do aplicativo/ID do cliente.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-112">When you register your app, keep the application ID/client ID somewhere handy.</span></span> <span data-ttu-id="ea5a5-113">Essa ID será usada posteriormente ao registrar seu aplicativo para experiências entre dispositivos no [Microsoft Partner Center](https://partner.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="ea5a5-113">You'll need this ID later when you register your application for cross-device experiences in the [Microsoft Partner Center](https://partner.microsoft.com/).</span></span>

## <a name="app-certificates-and-secrets"></a><span data-ttu-id="ea5a5-114">Certificados e segredos do aplicativo </span><span class="sxs-lookup"><span data-stu-id="ea5a5-114">App certificates and secrets</span></span>

<span data-ttu-id="ea5a5-115">Para que o aplicativo se identifique e se autentique ao obter tokens de autenticação, você pode carregar seu próprio certificado ou criar um nova segredo do cliente acessando **certificados e segredos** no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-115">To enable your application to identify and authenticate itself when obtaining auth tokens, you can either upload your own certificate or create a new client secret by going to **Certificates & secrets** in the Azure portal.</span></span>
    
![Captura de tela de certificados e segredos do aplicativo no portal do Azure](images/notifications-app-secrets.png)
    
> [!NOTE]
> <span data-ttu-id="ea5a5-117">Se optar por gerar um novo segredo do cliente, certifique-se de copiá-lo a e guardá-lo em um local seguro.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-117">If you opt to generate a new client secret, be sure to copy and keep it in a safe place.</span></span> <span data-ttu-id="ea5a5-118">Você não poderá acessá-lo novamente após sair do portal.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-118">You won’t be able to access it again after you leave the portal.</span></span>

## <a name="api-permissions"></a><span data-ttu-id="ea5a5-119">Permissões de API</span><span class="sxs-lookup"><span data-stu-id="ea5a5-119">Web API permissions overview</span></span>

<span data-ttu-id="ea5a5-120">É preciso incluir permissões adicionais para usar as notificações do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-120">You'll need to add additional permissions in order to use Microsoft Graph notifications.</span></span> <span data-ttu-id="ea5a5-121">Escolha **Adicionar uma permissão**e, em APIs Microsoft, selecione **Microsoft Graph**e depois **Permissões delegadas**.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-121">Choose **Add a permission**, and under Microsoft APIs, select **Microsoft Graph**, and then select **Delegated permissions**.</span></span>
    
![Captura de tela da página de permissões de API de solicitação do portal do Azure](images/notifications-api-permissions.png)
    
<span data-ttu-id="ea5a5-123">Adicione as seguintes permissões:</span><span class="sxs-lookup"><span data-stu-id="ea5a5-123">Add the following permissions:</span></span>

- <span data-ttu-id="ea5a5-124">User.Read – permite que o aplicativo conecte seu usuário</span><span class="sxs-lookup"><span data-stu-id="ea5a5-124">User.Read - allows your application to sign-in your user</span></span>

- <span data-ttu-id="ea5a5-125">Device.Read – permite a identificação da lista de dispositivos do usuário</span><span class="sxs-lookup"><span data-stu-id="ea5a5-125">Device.Read - allows identification of a user’s list of devices</span></span>

- <span data-ttu-id="ea5a5-126">Device.Command – permite a comunicação do dispositivo do usuário</span><span class="sxs-lookup"><span data-stu-id="ea5a5-126">Device.Command - allows communication to a user’s device</span></span>

- <span data-ttu-id="ea5a5-127">UserActivity.ReadWrite.CreatedByApp – permite a assinatura do aplicativo para recuperação de notificação</span><span class="sxs-lookup"><span data-stu-id="ea5a5-127">UserActivity.ReadWrite.CreatedByApp - allows app subscription for notification retrieval</span></span>

- <span data-ttu-id="ea5a5-128">Notifications.ReadWrite.CreatedByApp – permite o acesso e entrega de notificação</span><span class="sxs-lookup"><span data-stu-id="ea5a5-128">Notifications.ReadWrite.CreatedByApp - allows notification access and delivery</span></span>

- <span data-ttu-id="ea5a5-129">wns.connect – permite conectar ao serviço de notificação do Windows</span><span class="sxs-lookup"><span data-stu-id="ea5a5-129">wns.connect - allows connecting to windows notification service</span></span>

![Captura de tela das permissões delegadas para notificações no portal do Azure](images/notifications-api-permissions-list.png)

## <a name="next-steps"></a><span data-ttu-id="ea5a5-131">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ea5a5-131">Next steps</span></span>

<span data-ttu-id="ea5a5-132">Saiba mais sobre [permissões e consentimento](https://docs.microsoft.com/pt-BR/azure/active-directory/develop/v2-permissions-and-consent) ou consulte a [referência de permissões](https://docs.microsoft.com/pt-BR/graph/permissions-reference) do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-132">Learn more about [permissions and consent](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-permissions-and-consent) or view the Microsoft Graph [permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

<span data-ttu-id="ea5a5-133">Após registrar seu aplicativo, acesse o [Partner Center](https://partner.microsoft.com/) para configurar o aplicativo para experiências entre dispositivos e para direcionar suas plataformas de aplicativo correspondentes para notificações enviadas pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ea5a5-133">Now that you’ve registered your app, go to the [Partner Center](https://partner.microsoft.com/) to set up your application for cross-device experiences and to target your corresponding app platforms for notifications sent via Microsoft Graph.</span></span> <span data-ttu-id="ea5a5-134">Para saber mais, confira a [Integração à experiência entre dispositivos](notifications-integration-cross-device-experiences-onboarding.md).</span><span class="sxs-lookup"><span data-stu-id="ea5a5-134">For details, see [Onboarding to cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md).</span></span> 
