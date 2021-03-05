---
title: Provedor de eletrônica
description: O provedor MSAL para o Eletrônica usa o msal-node para entrar nos usuários e adquirir tokens para usar com o Microsoft Graph.
localization_priority: Normal
author: amrutha95
ms.openlocfilehash: a9e391f96988f8beaf8395e872a6efa08efca8f5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471419"
---
# <a name="electron-provider"></a><span data-ttu-id="aa5b4-103">Provedor de eletrônica</span><span class="sxs-lookup"><span data-stu-id="aa5b4-103">Electron provider</span></span>

<span data-ttu-id="aa5b4-104">O provedor Demão usa [o nó msal](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph em um aplicativo Demão.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-104">The Electron provider uses [msal-node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/lib/msal-node) to sign in users and acquire tokens to use with Microsoft Graph in an Electron application.</span></span>

<span data-ttu-id="aa5b4-105">Para saber mais sobre provedores de autenticação, consulte [provedores](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="aa5b4-105">To learn more about authentication providers, see [providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="aa5b4-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="aa5b4-106">Get started</span></span>
### <a name="install-the-packages"></a><span data-ttu-id="aa5b4-107">Instalar os pacotes</span><span class="sxs-lookup"><span data-stu-id="aa5b4-107">Install the packages</span></span>

```bash
npm install @microsoft/mgt-element @microsoft/mgt-electron-provider
```
<span data-ttu-id="aa5b4-108">Você precisa inicializar oTronProvider no processo de renderização (front-end) e oTronAuthenticator no processo principal (back-end).</span><span class="sxs-lookup"><span data-stu-id="aa5b4-108">You need to initialize ElectronProvider in the renderer process (front end), and ElectronAuthenticator in the main process (back end).</span></span>


### <a name="initializing-electronprovider-in-the-renderer-process-rendererts"></a><span data-ttu-id="aa5b4-109">Inicializando oTronProvider no processo de renderizador (renderer.ts)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-109">Initializing ElectronProvider in the renderer process (renderer.ts)</span></span>

<span data-ttu-id="aa5b4-110">OTronProvider é responsável por se comunicar com oTronAuthenticator (no processo principal) para solicitar tokens de acesso e receber informações sobre o estado conectado que são necessárias para que os componentes funcionem.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-110">The ElectronProvider is responsible for communicating with ElectronAuthenticator (in the main process) to request access tokens and receive information regarding logged in state that are required for the components to work.</span></span> 

```ts
import {Providers} from '@microsoft/mgt-element';
import {ElectronProvider} from '@microsoft/mgt-electron-provider/dist/Provider';
import '@microsoft/mgt-components';

// initialize the auth provider globally
Providers.globalProvider = new ElectronProvider();
```

### <a name="initializing-electronauthenticator-in-the-main-process-maints"></a><span data-ttu-id="aa5b4-111">Inicializando o EletrônicaAuthenticator no processo principal (main.ts)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-111">Initializing ElectronAuthenticator in the main process (main.ts)</span></span>

<span data-ttu-id="aa5b4-112">OTronAuthenticator é responsável por configurar as variáveis de configuração para autenticação MSAL, adquirir tokens de acesso e se comunicar com oTronProvider.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-112">The ElectronAuthenticator is responsible for setting up the configuration variables for MSAL authentication, acquiring access tokens, and communicating with ElectronProvider.</span></span>
<span data-ttu-id="aa5b4-113">Inicializar oTronAuthenticator no processo principal e configurar as variáveis de configuração, como id do cliente.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-113">Initialize the ElectronAuthenticator in the main process and set up the configuration variables such as client-id.</span></span>

```ts
import { ElectronAuthenticator, MsalElectronConfig } from '@microsoft/mgt-electron-provider/dist/Authenticator'; 

let config: MsalElectronConfig = {
  clientId: '<your_client_id>',
  authority: '<your_authority_url>', //optional
  mainWindow: mainWindow, 
  scopes: ['user.read'] //We recommend pre-consenting all the required scopes on the Azure portal
};

ElectronAuthenticator.initialize(config);
```
 
| <span data-ttu-id="aa5b4-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="aa5b4-114">Attribute</span></span>    | <span data-ttu-id="aa5b4-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa5b4-115">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="aa5b4-116">clientId</span><span class="sxs-lookup"><span data-stu-id="aa5b4-116">clientId</span></span>    | <span data-ttu-id="aa5b4-117">ID do cliente de cadeia de caracteres (consulte Criando uma ID de aplicativo/cliente).</span><span class="sxs-lookup"><span data-stu-id="aa5b4-117">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="aa5b4-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-118">Required.</span></span>                                                                                                                                                                                                           |                                                                                                                                                                               |
| <span data-ttu-id="aa5b4-119">escopos</span><span class="sxs-lookup"><span data-stu-id="aa5b4-119">scopes</span></span>       | <span data-ttu-id="aa5b4-120">Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-120">Comma-separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="aa5b4-121">Recomendado.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-121">Recommended.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="aa5b4-122">authority</span><span class="sxs-lookup"><span data-stu-id="aa5b4-122">authority</span></span>    | <span data-ttu-id="aa5b4-123">Cadeia de caracteres de autoridade - padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-123">Authority string - default is the common authority.</span></span> <span data-ttu-id="aa5b4-124">Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-124">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="aa5b4-125">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="aa5b4-125">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="aa5b4-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-126">Optional.</span></span> |                                                                                                                                                                                          |
| <span data-ttu-id="aa5b4-127">mainWindow</span><span class="sxs-lookup"><span data-stu-id="aa5b4-127">mainWindow</span></span>  | <span data-ttu-id="aa5b4-128">Instância do BrowserWindow principal que requer autenticação.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-128">Instance of the main BrowserWindow that requires authentication.</span></span>|
| <span data-ttu-id="aa5b4-129">cachePlugin</span><span class="sxs-lookup"><span data-stu-id="aa5b4-129">cachePlugin</span></span> | <span data-ttu-id="aa5b4-130">Plug-in de cache que você gostaria de usar para armazenamento persistente de tokens.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-130">Cache plugin you would like to use for persistent storage of tokens.</span></span> <span data-ttu-id="aa5b4-131">Consulte [Extensões de Autenticação da Microsoft para Nó](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions).</span><span class="sxs-lookup"><span data-stu-id="aa5b4-131">See [Microsoft Authentication Extensions for Node](https://github.com/AzureAD/microsoft-authentication-library-for-js/tree/dev/extensions/msal-node-extensions).</span></span> <span data-ttu-id="aa5b4-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-132">Optional.</span></span> | 

><span data-ttu-id="aa5b4-133">**Observação:** Atualmente, o provedor não dá suporte a suporte incremental.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-133">**Note:** Currently, the provider does not support incremental support.</span></span> <span data-ttu-id="aa5b4-134">Como prática prática, certifique-se de concordar com todos os escopos necessários aos componentes.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-134">As a best practice, be sure to consent to all the scopes that the components require.</span></span>
    
## <a name="create-an-appclient-id"></a><span data-ttu-id="aa5b4-135">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="aa5b4-135">Create an app/client ID</span></span>

### <a name="add-new-application-registration-in-azure-active-directory-to-get-a-client-id"></a><span data-ttu-id="aa5b4-136">Adicionar novo registro de aplicativo no Azure Active Directory para obter uma ID do cliente</span><span class="sxs-lookup"><span data-stu-id="aa5b4-136">Add new application registration in Azure Active Directory to get a client ID</span></span>

<span data-ttu-id="aa5b4-137">Para criar um aplicativo no Azure Active Directory, adicione um novo registro de aplicativo e configure um nome de aplicativo e URI de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-137">To create an application in Azure Active Directory, add a new application registration, and then configure an app name and redirect URI.</span></span>

<span data-ttu-id="aa5b4-138">Para criar o aplicativo no Azure Active Directory:</span><span class="sxs-lookup"><span data-stu-id="aa5b4-138">To create the app in Azure Active Directory:</span></span>

1. <span data-ttu-id="aa5b4-139">Vá para o [portal do Azure](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="aa5b4-139">Go to the [Azure portal](https://portal.azure.com).</span></span>
1. <span data-ttu-id="aa5b4-140">No menu, selecione **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-140">From the menu, select **Azure Active Directory**.</span></span>
1. <span data-ttu-id="aa5b4-141">No menu do Azure Active Directory, selecione **Registros de aplicativos**.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-141">From the Azure Active Directory menu, select **App registrations**.</span></span>
1. <span data-ttu-id="aa5b4-142">No menu superior, selecione o **botão Novo registro.**</span><span class="sxs-lookup"><span data-stu-id="aa5b4-142">From the top menu, select the **New registration** button.</span></span>
1. <span data-ttu-id="aa5b4-143">Insira o nome do seu aplicativo; por exemplo, `My Electron-App` .</span><span class="sxs-lookup"><span data-stu-id="aa5b4-143">Enter the name for your app; for example, `My Electron-App`.</span></span>
1. <span data-ttu-id="aa5b4-144">Para o tipo de tipos de conta com [suporte,](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)selecione Contas em qualquer diretório organizacional (Qualquer diretório do **Azure AD - Multitenant) e contas pessoais da Microsoft (por exemplo, Skype, Xbox)**.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-144">For the type of [supported account types](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app), select **Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)**.</span></span>
1. <span data-ttu-id="aa5b4-145">No campo **Redirecionar URI,** no menu suspenso, selecione **Cliente público/nativo (área** de trabalho móvel &) e, no campo URL, digite `msal://redirect` .</span><span class="sxs-lookup"><span data-stu-id="aa5b4-145">In the **Redirect URI** field, in the dropdown, select **Public client/native (mobile & desktop)**, and in the URL field, enter `msal://redirect`.</span></span>
1. <span data-ttu-id="aa5b4-146">Confirme as alterações selecionando o **botão Registrar.**</span><span class="sxs-lookup"><span data-stu-id="aa5b4-146">Confirm changes by selecting the **Register** button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="aa5b4-147">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="aa5b4-147">Next steps</span></span>

* <span data-ttu-id="aa5b4-148">Confira o tutorial passo a passo para [criar um aplicativo de eletrônica.](../get-started/build-an-electron-app.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-148">Check out the step-by-step tutorial for [building an electron app](../get-started/build-an-electron-app.md).</span></span>
* <span data-ttu-id="aa5b4-149">Dê uma olhada em um [aplicativo Detron de](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) exemplo que mostra como usar o provedor Demão.</span><span class="sxs-lookup"><span data-stu-id="aa5b4-149">Take a look at a [sample Electron application](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/main/samples/electron-app) that shows how to use the Electron provider.</span></span>
