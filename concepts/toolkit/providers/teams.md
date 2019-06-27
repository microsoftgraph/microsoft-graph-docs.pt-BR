---
title: Provedor do Microsoft Teams
description: Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 348980225f04adfac4ded6f79a72654fbeec81e7
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242933"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="867ca-103">Provedor do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="867ca-103">Microsoft Teams provider</span></span>

<span data-ttu-id="867ca-104">Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="867ca-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="867ca-105">Para saber mais, veja [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="867ca-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="867ca-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="867ca-106">Get started</span></span>

<span data-ttu-id="867ca-107">Antes de usar o provedor do Teams, você precisará certificar-se de que você referenciou o [SDK do Microsoft Teams](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) na sua página.</span><span class="sxs-lookup"><span data-stu-id="867ca-107">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

<span data-ttu-id="867ca-108">O exemplo a seguir usa o provedor em HTML (via CDN).</span><span class="sxs-lookup"><span data-stu-id="867ca-108">The following example uses the provider in HTML (via CDN).</span></span>

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
></mgt-teams-provider>
```

<span data-ttu-id="867ca-109">O exemplo a seguir usa o provedor em módulos JS (via NPM).</span><span class="sxs-lookup"><span data-stu-id="867ca-109">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="867ca-110">Certifique-se de instalar o kit de ferramentas e o SDK do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="867ca-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="867ca-111">Em seguida, importe e use o provedor.</span><span class="sxs-lookup"><span data-stu-id="867ca-111">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt'; 
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="867ca-112">onde `config` é</span><span class="sxs-lookup"><span data-stu-id="867ca-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="867ca-113">Para ver um exemplo completo, confira o [exemplo de guia do Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span><span class="sxs-lookup"><span data-stu-id="867ca-113">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="867ca-114">Configurar seu aplicativo do teams</span><span class="sxs-lookup"><span data-stu-id="867ca-114">Configure your Teams app</span></span>

<span data-ttu-id="867ca-115">Se você estiver apenas começando a usar o Teams apps, consulte [adicionar guias aos aplicativos do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="867ca-115">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="867ca-116">Você também pode usar o [app Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="867ca-116">You can also use [App Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="867ca-117">Após instalar seu aplicativo com uma guia e você estiver pronto para usar os componentes, você precisará certificar-se de que seu aplicativo tem as permissões corretas para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="867ca-117">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="867ca-118">Para configurar seu aplicativo com as permissões necessárias:</span><span class="sxs-lookup"><span data-stu-id="867ca-118">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="867ca-119">Recuperar seu nome de domínio</span><span class="sxs-lookup"><span data-stu-id="867ca-119">Retrieve your domain name</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="867ca-120">Criar um novo registro de aplicativo</span><span class="sxs-lookup"><span data-stu-id="867ca-120">Create a new app registration</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [<span data-ttu-id="867ca-121">Conceder sua permissão de aplicativo</span><span class="sxs-lookup"><span data-stu-id="867ca-121">Grant your application permission</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="867ca-122">É importante adicionar a permissão certa na **página Adicionar acesso à API**.</span><span class="sxs-lookup"><span data-stu-id="867ca-122">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="867ca-123">Você precisará de um administrador para adicionar e aprovar as permissões, dependendo de qual componente você precisa.</span><span class="sxs-lookup"><span data-stu-id="867ca-123">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="867ca-124">**Dica:** Se você não tiver certeza sobre as permissões a serem adicionadas, consulte a documentação de cada componente.</span><span class="sxs-lookup"><span data-stu-id="867ca-124">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="867ca-125">Habilitar fluxo de concessão implícito</span><span class="sxs-lookup"><span data-stu-id="867ca-125">Enable implicit grant Flow</span></span>

<span data-ttu-id="867ca-126">Certifique-se de habilitar o fluxo de concessão implícito; Esse é um requisito para aplicativos Web que solicitam tokens do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="867ca-126">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="867ca-127">No portal do Azure, ao gerenciar o registro do aplicativo, edite o manifesto `oauth2AllowImplicitFlow` e `true`altere para.</span><span class="sxs-lookup"><span data-stu-id="867ca-127">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="867ca-128">Criar a página pop-up</span><span class="sxs-lookup"><span data-stu-id="867ca-128">Create the popup page</span></span>

<span data-ttu-id="867ca-129">Para entrar com suas credenciais do Microsoft Teams, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up, o que irá seguir o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="867ca-129">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="867ca-130">Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método.</span><span class="sxs-lookup"><span data-stu-id="867ca-130">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="867ca-131">Essa é a única coisa que esta página precisa fazer.</span><span class="sxs-lookup"><span data-stu-id="867ca-131">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="867ca-132">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="867ca-132">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>        
  mgt.TeamsProvider.handleAuth();
</script>
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="867ca-133">Configurar URIs de redirecionamento</span><span class="sxs-lookup"><span data-stu-id="867ca-133">Configure redirect URIs</span></span>

<span data-ttu-id="867ca-134">Após publicar esta página no seu site, você precisará usar a URL na `auth-popup-url/authPopupUrl` propriedade.</span><span class="sxs-lookup"><span data-stu-id="867ca-134">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="867ca-135">Essa URL também precisa ser configurada como um URI de redirecionamento válido em sua configuração de aplicativo no portal do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="867ca-135">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
