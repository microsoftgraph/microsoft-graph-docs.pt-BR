---
title: Criar um aplicativo no Azure Active Directory
description: Criar um registro Azure Active Directory aplicativo para se comunicar com Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: b68281473d884309c23a72979ae07a8a9c752d2f
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579918"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="70ce1-103">Criar um Azure Active Directory para usar com o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="70ce1-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="70ce1-104">O microsoft Graph, a API que você usa para se conectar ao Microsoft 365, está protegida com o OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="70ce1-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="70ce1-105">Para conectar seu aplicativo ao Microsoft 365, você precisará criar um aplicativo no Azure Active Directory (Azure AD) e conceder a esse aplicativo permissões para acessar recursos específicos em nome da pessoa que está usando seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70ce1-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="70ce1-106">Este tópico descreve como registrar e configurar um aplicativo Web a ser usado com o Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="70ce1-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="70ce1-107">Adicionar novo registro de aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="70ce1-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="70ce1-108">Para criar um aplicativo no Azure Active Directory, você precisa adicionar um novo registro de aplicativo e configurar um nome de aplicativo e um local de URL.</span><span class="sxs-lookup"><span data-stu-id="70ce1-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="70ce1-109">Para criar o aplicativo em Azure Active Directory:</span><span class="sxs-lookup"><span data-stu-id="70ce1-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="70ce1-110">Vá para o portal do Azure em https://portal.azure.com .</span><span class="sxs-lookup"><span data-stu-id="70ce1-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="70ce1-111">No menu, selecione **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="70ce1-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="70ce1-112">No menu Azure Active Directory, selecione **Registros de aplicativos**.</span><span class="sxs-lookup"><span data-stu-id="70ce1-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="70ce1-113">No menu superior, selecione o **botão Novo registro.**</span><span class="sxs-lookup"><span data-stu-id="70ce1-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="70ce1-114">Insira o nome do seu aplicativo; por exemplo, `My M365 app` .</span><span class="sxs-lookup"><span data-stu-id="70ce1-114">Enter the name for your app; for example, `My M365 app`.</span></span>
1. <span data-ttu-id="70ce1-115">Para o tipo de tipos de conta com [suporte,](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)selecione Contas em qualquer diretório organizacional (Qualquer diretório **do Azure AD - Multitenant) e contas pessoais da Microsoft (por exemplo, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="70ce1-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="70ce1-116">No campo **Redirecionar URI,** no menu suspenso, selecione Aplicativo de Página Única **(SPA)** e, no campo URL, insira `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="70ce1-116">In the **Redirect URI** field, in the dropdown, select **Single Page Application (SPA)**, and in the URL field, enter `http://localhost:3000`.</span></span> <span data-ttu-id="70ce1-117">Observação: se você estiver usando o Provedor MSAL e não o Provedor MSAL 2.0, precisará selecionar **Web** em vez de **SPA**.</span><span class="sxs-lookup"><span data-stu-id="70ce1-117">Note: if you are using MSAL Provider and not MSAL 2.0 Provider, you will need to select **Web** instead of **SPA**.</span></span>
1. <span data-ttu-id="70ce1-118">Confirme as alterações selecionando o **botão Registrar.**</span><span class="sxs-lookup"><span data-stu-id="70ce1-118">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow-only-for-msal-10-provider"></a><span data-ttu-id="70ce1-119">Habilitar o fluxo implícito OAuth (somente para provedor MSAL 1.0)</span><span class="sxs-lookup"><span data-stu-id="70ce1-119">Enable OAuth implicit flow (only for MSAL 1.0 provider)</span></span>

<span data-ttu-id="70ce1-120">Na maioria dos casos, você usará o Microsoft Graph Toolkit em aplicativos do lado do cliente que consistem apenas em código do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="70ce1-120">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="70ce1-121">Como os aplicativos do lado do cliente não podem armazenar segredos com segurança, você precisa usar o fluxo implícito [OAuth,](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)que pressu assume a identidade de um aplicativo com base em sua ID e URL.</span><span class="sxs-lookup"><span data-stu-id="70ce1-121">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="70ce1-122">No Portal do Azure, abra seu registro de aplicativo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="70ce1-122">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="70ce1-123">No menu, escolha **Autenticação**.</span><span class="sxs-lookup"><span data-stu-id="70ce1-123">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="70ce1-124">Na seção **Concessão implícita,** habilita as **opções tokens do Access** e **tokens de ID.**</span><span class="sxs-lookup"><span data-stu-id="70ce1-124">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="70ce1-125">Confirme suas alterações escolhendo o **botão Salvar.**</span><span class="sxs-lookup"><span data-stu-id="70ce1-125">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="70ce1-126">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="70ce1-126">Next steps</span></span>

- <span data-ttu-id="70ce1-127">[Criar um aplicativo Web](./build-a-web-app.md) (javaScript de baunilha)</span><span class="sxs-lookup"><span data-stu-id="70ce1-127">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="70ce1-128">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="70ce1-128">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="70ce1-129">Use o Toolkit com React</span><span class="sxs-lookup"><span data-stu-id="70ce1-129">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="70ce1-130">Use o Toolkit com Angular</span><span class="sxs-lookup"><span data-stu-id="70ce1-130">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
