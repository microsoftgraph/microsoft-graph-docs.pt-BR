---
title: Criar um aplicativo no Azure Active Directory
description: Criar um registro de aplicativo do Azure Active Directory para se comunicar com o Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 821cd6981ddb24e3917a4c0720f1c8c524081f54
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059564"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="a71d9-103">Criar um aplicativo do Azure Active Directory para usar com o Kit de Ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a71d9-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="a71d9-104">O Microsoft Graph, a API que você usa para se conectar ao Microsoft 365, é protegido com o OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="a71d9-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="a71d9-105">Para conectar seu aplicativo ao Microsoft 365, você precisará criar um aplicativo no Azure Active Directory (Azure AD) e conceder permissões a esse aplicativo para acessar recursos específicos em nome da pessoa que está usando seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a71d9-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="a71d9-106">Este tópico descreve como registrar e configurar um aplicativo Web para usar com o Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="a71d9-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="a71d9-107">Adicionar novo registro de aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a71d9-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="a71d9-108">Para criar um aplicativo no Azure Active Directory, você precisa adicionar um novo registro de aplicativo e configurar um nome de aplicativo e um local de URL.</span><span class="sxs-lookup"><span data-stu-id="a71d9-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="a71d9-109">Para criar o aplicativo no Azure Active Directory:</span><span class="sxs-lookup"><span data-stu-id="a71d9-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="a71d9-110">Vá para o portal do Azure em https://portal.azure.com .</span><span class="sxs-lookup"><span data-stu-id="a71d9-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="a71d9-111">No menu, selecione **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="a71d9-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="a71d9-112">No menu do Azure Active Directory, selecione **Registros de aplicativo.**</span><span class="sxs-lookup"><span data-stu-id="a71d9-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="a71d9-113">No menu superior, selecione o **botão Novo** registro.</span><span class="sxs-lookup"><span data-stu-id="a71d9-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="a71d9-114">Insira o nome do seu aplicativo; por exemplo, `My M365 app` .</span><span class="sxs-lookup"><span data-stu-id="a71d9-114">Enter the name for your app; for example, `My M365 app`.</span></span>
1. <span data-ttu-id="a71d9-115">Para o tipo de conta com [suporte,](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)selecione Contas em qualquer diretório organizacional (qualquer diretório do **Azure AD - Multi-tenant)** e contas pessoais da Microsoft (por exemplo, Skype, Xbox) .</span><span class="sxs-lookup"><span data-stu-id="a71d9-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="a71d9-116">No campo **Redirecionar URI,** na lista suspenso, selecione **Web** e, no campo URL, insira `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="a71d9-116">In the **Redirect URI** field, in the dropdown, select **Web**, and in the URL field, enter `http://localhost:3000`.</span></span>
1. <span data-ttu-id="a71d9-117">Confirme as alterações selecionando o **botão** Registrar.</span><span class="sxs-lookup"><span data-stu-id="a71d9-117">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow"></a><span data-ttu-id="a71d9-118">Habilitar fluxo implícito do OAuth</span><span class="sxs-lookup"><span data-stu-id="a71d9-118">Enable OAuth implicit flow</span></span>

<span data-ttu-id="a71d9-119">Na maioria dos casos, você usará o Microsoft Graph Toolkit em aplicativos do lado do cliente que consistem apenas em código do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="a71d9-119">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="a71d9-120">Como os aplicativos do lado do cliente não podem armazenar segredos com segurança, você precisa usar o fluxo implícito do [OAuth,](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)que pressuou a identidade de um aplicativo com base em sua ID e URL.</span><span class="sxs-lookup"><span data-stu-id="a71d9-120">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="a71d9-121">No Portal do Azure, abra seu registro de aplicativo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="a71d9-121">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="a71d9-122">No menu, escolha **Autenticação.**</span><span class="sxs-lookup"><span data-stu-id="a71d9-122">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="a71d9-123">Na seção **Concessão implícita,** habilitar **tokens do Access** e **opções de tokens de ID.**</span><span class="sxs-lookup"><span data-stu-id="a71d9-123">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="a71d9-124">Confirme suas alterações escolhendo o **botão** Salvar.</span><span class="sxs-lookup"><span data-stu-id="a71d9-124">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a71d9-125">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a71d9-125">Next steps</span></span>

- <span data-ttu-id="a71d9-126">[Criar um aplicativo Web](./build-a-web-app.md) (javascript de java de java)</span><span class="sxs-lookup"><span data-stu-id="a71d9-126">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="a71d9-127">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a71d9-127">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="a71d9-128">Usar o Kit de Ferramentas com o React</span><span class="sxs-lookup"><span data-stu-id="a71d9-128">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="a71d9-129">Usar o Kit de Ferramentas com o Angular</span><span class="sxs-lookup"><span data-stu-id="a71d9-129">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
