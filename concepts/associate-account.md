---
title: Associar sua conta do Office 365 ao AD do Azure para criar e gerenciar aplicativos
description: 'Para autenticar seus aplicativos usando o Microsoft Azure Active Directory (Azure AD), você precisa registrá-los no Azure AD. É lá que as informações da conta de usuário do Office 365 e do aplicativo estão armazenadas. Para gerenciar o Azure AD no Portal do Azure, você precisará de uma assinatura do Microsoft Azure. Use o portal no Microsoft Azure para gerenciar usuários, funções e aplicativos. '
localization_priority: Normal
ms.openlocfilehash: af77e9bbe87ba3a7c92c91967c8df87a16224d99
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951200"
---
# <a name="associate-your-office-365-account-with-azure-ad-to-create-and-manage-apps"></a><span data-ttu-id="3a1fe-106">Associar sua conta do Office 365 ao Azure AD para criar e gerenciar aplicativos</span><span class="sxs-lookup"><span data-stu-id="3a1fe-106">Associate your Office 365 account with Azure AD to create and manage apps</span></span>

<span data-ttu-id="3a1fe-107">Para autenticar seus aplicativos usando o Microsoft Azure Active Directory (Azure AD), você precisa registrá-los no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-107">To authenticate your applications using Microsoft Azure Active Directory (Azure AD), you need to register them in Azure AD.</span></span> <span data-ttu-id="3a1fe-108">É lá que as informações da conta de usuário do Office 365 e do aplicativo estão armazenadas.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-108">This is where Office 365 user account and application information is stored.</span></span> <span data-ttu-id="3a1fe-109">Para gerenciar o Azure AD no Portal do Azure, você precisará de uma assinatura do Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-109">To manage Azure AD through the Azure portal, you need a Microsoft Azure subscription.</span></span> <span data-ttu-id="3a1fe-110">Use o portal no Microsoft Azure para gerenciar usuários, funções e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-110">You can use the portal in Microsoft Azure to manage users, roles, and apps.</span></span>

<span data-ttu-id="3a1fe-111">Este artigo mostra como associar sua conta do Office 365 ao Azure AD para criar e gerenciar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-111">This article shows you how to associate your Office 365 account with Azure AD to create and manage apps.</span></span>

 ><span data-ttu-id="3a1fe-p103">**Observação:** Este artigo usa o Azure AD como provedor de autenticação para o seu aplicativo. Se você estiver usando o ponto de extremidade do Azure AD v2.0, não precisará executar esta etapa. Para mais informações, confira [Autenticação de aplicativo com o Microsoft Graph](/graph/auth).</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p103">**Note:** This article uses Azure AD as the authentication provider for your app. If you're using the Azure AD v2.0 endpoint, you don't need to perform this step. For more information, see [App authentication with Microsoft Graph](/graph/auth).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a1fe-115">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3a1fe-115">Prerequisites</span></span>

<span data-ttu-id="3a1fe-116">**Conta do Office 365 para empresas**</span><span class="sxs-lookup"><span data-stu-id="3a1fe-116">**Office 365 for business account**</span></span>

<span data-ttu-id="3a1fe-117">Se você não tiver uma conta do Office 365 para empresas, poderá:</span><span class="sxs-lookup"><span data-stu-id="3a1fe-117">If you don't have an existing Office 365 for business account, you can:</span></span>

- <span data-ttu-id="3a1fe-118">Inscreva-se em um dos [planos do Office 365 para empresas](https://products.office.com/en-us/business/compare-office-365-for-business-plans) listados acima ou</span><span class="sxs-lookup"><span data-stu-id="3a1fe-118">Sign up for an [Office 365 for business plans](https://products.office.com/en-us/business/compare-office-365-for-business-plans) listed above, or</span></span>
- <span data-ttu-id="3a1fe-119">[Join the Office 365 Developer Program and get a free 1 year subscription to Office 365](https://aka.ms/devprogramsignup).</span><span class="sxs-lookup"><span data-stu-id="3a1fe-119">[Join the Office 365 Developer Program and get a free 1 year subscription to Office 365](https://aka.ms/devprogramsignup).</span></span>

<span data-ttu-id="3a1fe-120">**Assinatura do Microsoft Azure**</span><span class="sxs-lookup"><span data-stu-id="3a1fe-120">**Microsoft Azure subscription**</span></span>

- <span data-ttu-id="3a1fe-121">Se você tiver uma assinatura existente do Microsoft Azure, poderá associar sua assinatura do Office 365 para empresas a ela.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-121">If you can have an existing Microsoft Azure subscription, you can associate your Office 365 for business subscription with it.</span></span>

- <span data-ttu-id="3a1fe-122">Caso contrário, você precisará criar uma nova assinatura do Azure e associá-la à sua conta do Office 365 para registrar e gerenciar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-122">Otherwise, you'll need to create a new Azure subscription and associate it with your Office 365 account in order to register and manage apps.</span></span>


<!---<a name="bk_AssociateExistingAzureSubscription"> </a>-->

## <a name="to-associate-an-existing-azure-subscription-with-your-office-365-account"></a><span data-ttu-id="3a1fe-123">Para associar uma assinatura existente do Azure à sua conta do Office 365</span><span class="sxs-lookup"><span data-stu-id="3a1fe-123">To associate an existing Azure subscription with your Office 365 account</span></span>


1. <span data-ttu-id="3a1fe-124">Faça logon no [Portal do Microsoft Azure](https://portal.azure.com) com suas credenciais do Azure existentes (por exemplo, sua ID da Microsoft, como user@live.com).</span><span class="sxs-lookup"><span data-stu-id="3a1fe-124">Log on to the  [Microsoft Azure portal](https://portal.azure.com) with your existing Azure credentials (for example, your Microsoft ID such as user@live.com).</span></span>

2. <span data-ttu-id="3a1fe-125">Selecione o nó **Active Directory**, selecione a guia **Diretório** e, na parte inferior da tela, selecione **Novo**.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-125">Select the  **Active Directory** node, then select the **Directory** tab and, at the bottom of the screen, select **New**.</span></span>

4. <span data-ttu-id="3a1fe-126">No menu **Novo**, selecione **Active Directory** > **Diretório** > **Criar Personalizado**.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-126">On the **New** menu, select **Active Directory** > **Directory** > **Custom Create**.</span></span>

5. <span data-ttu-id="3a1fe-p104">Em **Adicionar diretório**, na caixa suspensa **Diretório**, selecione **Usar diretório existente**. Marque **Estou pronto para sair** e escolha a marca de seleção no canto inferior direito.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p104">In **Add directory**, in the **Directory** dropdown box, select  **Use existing directory**. Check **I am ready to be signed out**, and then select the check mark in the lower-right corner.</span></span>

    <span data-ttu-id="3a1fe-129">Isso leva você de volta ao portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-129">This brings you back to the Azure portal.</span></span>

3. <span data-ttu-id="3a1fe-130">Faça logon com suas informações de conta do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-130">Log in with your Office 365 account information.</span></span>

    <span data-ttu-id="3a1fe-131">Você será solicitado a responder se deseja usar seu diretório com o Azure.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-131">You will be prompted whether to use your directory with Azure.</span></span>

    ><span data-ttu-id="3a1fe-132">**Importante:** Para associar sua conta do Office 365 ao Azure AD, você precisará de uma conta do Office 365 para empresas com privilégios de administrador global.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-132">**Important:** To associate your Office 365 account with Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span>


4. <span data-ttu-id="3a1fe-133">Selecione **continuar** e **Sair agora**.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-133">Select  **continue**, and then **Sign out now**.</span></span>

5. <span data-ttu-id="3a1fe-p105">Feche o navegador e reabra o [portal](https://manage.windowsazure.com). Caso contrário, você receberá um erro de acesso negado.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p105">Close the browser and reopen the  [portal](https://manage.windowsazure.com). Otherwise, you will get an access denied error.</span></span>


6. <span data-ttu-id="3a1fe-p106">Faça logon novamente com suas credenciais do Azure existentes (por exemplo, sua ID da Microsoft, como user@live.com). Vá até o nó **Active Directory** e, em **Diretório**, sua conta do Office 365 deverá estar exibida agora.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p106">Log on again with your existing Azure credentials (for example, your Microsoft ID such as user@live.com). Go to the  **Active Directory** node and, under **Directory**, you should now see your Office 365 account listed.</span></span>


<!--<a name="bk_AssociateNewAzureSubscription"> </a>-->

## <a name="to-create-a-new-azure-subscription-and-associate-it-with-your-office-365-account"></a><span data-ttu-id="3a1fe-138">Para criar uma nova assinatura do Azure e associá-la com sua conta do Office 365</span><span class="sxs-lookup"><span data-stu-id="3a1fe-138">To create a new Azure subscription and associate it with your Office 365 account</span></span>


1. <span data-ttu-id="3a1fe-p107">Faça logon no Office 365. Na **Página inicial**, selecione o ícone **Administrador** para abrir o Centro de administração do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p107">Log on to Office 365. From the **Home** page, select the **Admin** icon to open the Office 365 admin center.</span></span>
2. <span data-ttu-id="3a1fe-141">Na página do menu no lado esquerdo, role para baixo até **Administrador** e selecione **Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-141">In the menu page along the left side of the page, scroll down to **Admin** and select **Azure AD**.</span></span>

    ><span data-ttu-id="3a1fe-142">**Importante:** Para abrir o Centro de administração do Office 365 e acessar o Azure AD, você precisará de uma conta do Office 365 para empresas com privilégios de administrador global.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-142">**Important:** To open the Office 365 admin center, and access Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span>

3. <span data-ttu-id="3a1fe-143">Crie uma nova assinatura.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-143">Create a new subscription.</span></span>

    <span data-ttu-id="3a1fe-p108">Se você estiver usando uma versão de avaliação do Office 365, verá uma mensagem informando que o AD do Azure está limitado a clientes com serviços pagos. Você ainda pode criar uma assinatura de avaliação do Azure de 30 dias sem nenhum custo, mas precisará executar algumas etapas adicionais:</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p108">If you're using a trial version of Office 365, you'll see a message telling you that Azure AD is limited to customers with paid services. You can still create a trial 30-day Azure subscription at no charge, but you'll need to perform a few extra steps:</span></span>

    1. <span data-ttu-id="3a1fe-146">Selecione seu país ou região e escolha **Assinatura do Azure**.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-146">Select your country or region, and then choose **Azure subscription**.</span></span>
    2. <span data-ttu-id="3a1fe-p109">Insira suas informações pessoais. Para fins de verificação, insira um número de telefone no qual você possa ser encontrado e especifique se deseja receber uma mensagem de texto ou uma chamada.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p109">Enter your personal information. For verification purposes, enter a telephone number at which you can be reached, and specify whether you want to be sent a text message or called.</span></span>
    3. <span data-ttu-id="3a1fe-149">Depois que você receber seu código de verificação, digite-o e escolha **Verificar código**.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-149">When you receive your verification code, enter it and choose **Verify code**.</span></span>
    4. <span data-ttu-id="3a1fe-150">Insira as informações de pagamento, verifique o contrato e selecione **Inscrever-se**.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-150">Enter payment information, check the agreement, and select **Sign up**.</span></span>

        <span data-ttu-id="3a1fe-151">Your credit card will not be charged.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-151">Your credit card will not be charged.</span></span>

        <span data-ttu-id="3a1fe-152">Não feche ou atualize o navegador enquanto a assinatura do Azure está sendo criada.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-152">Do not close or refresh your browser while your Azure subscription is being created.</span></span>

4. <span data-ttu-id="3a1fe-153">Depois que sua assinatura do Azure for criada, selecione **Portal**.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-153">When your Azure subscription is created, choose  **Portal**.</span></span>

5. <span data-ttu-id="3a1fe-p110">O Tour do Azure é exibido. Você pode exibi-lo ou escolher **X** para fechá-lo.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p110">The Azure Tour appears. You can view it, or choose  **X** to close it.</span></span>

    <span data-ttu-id="3a1fe-p111">Agora, você deve ver todos os itens na sua assinatura do Azure. Ele lista um diretório com o nome do seu locatário do Office 365.</span><span class="sxs-lookup"><span data-stu-id="3a1fe-p111">You should now see all items in your Azure subscription. It lists a directory with the name of your Office 365 tenant.</span></span>

## <a name="see-also"></a><span data-ttu-id="3a1fe-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="3a1fe-158">See also</span></span>
- [<span data-ttu-id="3a1fe-159">Noções básicas de como registrar um aplicativo no Azure AD</span><span class="sxs-lookup"><span data-stu-id="3a1fe-159">Basics of Registering an Application in Azure AD</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)
- [<span data-ttu-id="3a1fe-160">Adicionar, atualizar ou remover um aplicativo no Azure AD</span><span class="sxs-lookup"><span data-stu-id="3a1fe-160">Add, update, or remove an application in Azure AD</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-integrating-applications/)
