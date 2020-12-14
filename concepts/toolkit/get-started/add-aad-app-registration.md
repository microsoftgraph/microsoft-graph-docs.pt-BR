---
title: Criar um aplicativo no Azure Active Directory
description: Criar um registro de aplicativo do Azure Active Directory para se comunicar com o Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 7534d0d15b9ff1b2e1d94fe8d5e8e9e8f771ca91
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659160"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="ccc38-103">Criar um aplicativo do Azure Active Directory para uso com o kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ccc38-103">Create an Azure Active Directory app to use with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ccc38-104">O Microsoft Graph, a API que você usa para se conectar ao Microsoft 365, é protegido com o OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="ccc38-104">Microsoft Graph, the API that you use to connect to Microsoft 365, is secured with OAuth 2.0.</span></span> <span data-ttu-id="ccc38-105">Para conectar seu aplicativo ao Microsoft 365, você precisará criar um aplicativo no Azure Active Directory (Azure AD) e conceder a este aplicativo permissões para acessar recursos específicos em nome da pessoa que está usando seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ccc38-105">In order to connect your app to Microsoft 365, you will need to create an app in Azure Active Directory (Azure AD) and grant this app permissions to access specific resources on behalf of the person using your app.</span></span> <span data-ttu-id="ccc38-106">Este tópico descreve como registrar e configurar um aplicativo Web para usar com o Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="ccc38-106">This topic describes how to register and configure a web application to use with Microsoft Graph Toolkit.</span></span>

## <a name="add-new-application-registration-in-azure-active-directory"></a><span data-ttu-id="ccc38-107">Adicionar novo registro de aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="ccc38-107">Add new application registration in Azure Active Directory</span></span>

<span data-ttu-id="ccc38-108">Para criar um aplicativo no Azure Active Directory, você precisa adicionar um novo registro de aplicativo e, em seguida, configurar o nome do aplicativo e o local da URL.</span><span class="sxs-lookup"><span data-stu-id="ccc38-108">To create an application in Azure Active Directory, you need to add a new application registration, and then configure an app name and URL location.</span></span>

<span data-ttu-id="ccc38-109">Para criar o aplicativo no Azure Active Directory:</span><span class="sxs-lookup"><span data-stu-id="ccc38-109">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="ccc38-110">Vá para o portal do Azure em https://portal.azure.com .</span><span class="sxs-lookup"><span data-stu-id="ccc38-110">Go to the Azure portal at https://portal.azure.com.</span></span>
1. <span data-ttu-id="ccc38-111">No menu, selecione **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="ccc38-111">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="ccc38-112">No menu do Azure Active Directory, selecione **registros de aplicativos**.</span><span class="sxs-lookup"><span data-stu-id="ccc38-112">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="ccc38-113">No menu superior, selecione o botão **novo registro** .</span><span class="sxs-lookup"><span data-stu-id="ccc38-113">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="ccc38-114">Insira o nome do seu aplicativo; para exampe, `My M365 app` .</span><span class="sxs-lookup"><span data-stu-id="ccc38-114">Enter the name for your app; for exampe, `My M365 app`.</span></span>
1. <span data-ttu-id="ccc38-115">Para o tipo de [tipos de conta com suporte](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), selecione **contas em qualquer diretório organizacional (qualquer diretório do Azure ad-multilocatário) e contas pessoais da Microsoft (por exemplo, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="ccc38-115">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="ccc38-116">No campo **URI de redirecionamento** , na lista suspensa, selecione **Web** e, no campo URL, digite `http://localhost:3000` .</span><span class="sxs-lookup"><span data-stu-id="ccc38-116">In the **Redirect URI** field, in the dropdown, select **Web**, and in the URL field, enter `http://localhost:3000`.</span></span>
1. <span data-ttu-id="ccc38-117">Confirme as alterações selecionando o botão **registrar** .</span><span class="sxs-lookup"><span data-stu-id="ccc38-117">Confirm changes by selecting the **Register** button.</span></span>

## <a name="enable-oauth-implicit-flow"></a><span data-ttu-id="ccc38-118">Habilitar o fluxo implícito do OAuth</span><span class="sxs-lookup"><span data-stu-id="ccc38-118">Enable OAuth implicit flow</span></span>

<span data-ttu-id="ccc38-119">Na maioria dos casos, você usará o Microsoft Graph Toolkit em aplicativos do lado do cliente que consistem apenas em código do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="ccc38-119">In most cases, you will use Microsoft Graph Toolkit in client-side applications that consist only of client-side code.</span></span> <span data-ttu-id="ccc38-120">Como os aplicativos do lado do cliente não podem armazenar segredos com segurança, você precisa usar o [fluxo implícito do OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), que assume a identidade de um aplicativo com base em sua ID e URL.</span><span class="sxs-lookup"><span data-stu-id="ccc38-120">Because client-side apps can't store secrets securely, you need to use [OAuth implicit flow](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), which assumes an app's identity based on its ID and URL.</span></span>

1. <span data-ttu-id="ccc38-121">No portal do Azure, abra seu registro de aplicativo recém-criado.</span><span class="sxs-lookup"><span data-stu-id="ccc38-121">In the Azure Portal, open your newly created app registration.</span></span>
1. <span data-ttu-id="ccc38-122">No menu, escolha **autenticação**.</span><span class="sxs-lookup"><span data-stu-id="ccc38-122">From the menu, choose **Authentication**.</span></span>
1. <span data-ttu-id="ccc38-123">Na seção **concessão implícita** , habilite os **tokens de acesso** e as opções de **token de ID** .</span><span class="sxs-lookup"><span data-stu-id="ccc38-123">In the **Implicit grant** section, enable both **Access tokens** and **ID tokens** options.</span></span>
1. <span data-ttu-id="ccc38-124">Confirme suas alterações escolhendo o botão **salvar** .</span><span class="sxs-lookup"><span data-stu-id="ccc38-124">Confirm your changes by choosing the **Save** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ccc38-125">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ccc38-125">Next steps</span></span>

- <span data-ttu-id="ccc38-126">[Criar um aplicativo Web](./build-a-web-app.md) (JavaScript de baunilha)</span><span class="sxs-lookup"><span data-stu-id="ccc38-126">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="ccc38-127">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ccc38-127">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="ccc38-128">Usar o kit de ferramentas reagir</span><span class="sxs-lookup"><span data-stu-id="ccc38-128">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="ccc38-129">Usar o kit de ferramentas com angular</span><span class="sxs-lookup"><span data-stu-id="ccc38-129">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
