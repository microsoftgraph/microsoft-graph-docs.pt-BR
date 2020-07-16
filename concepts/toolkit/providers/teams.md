---
title: Provedor do Microsoft Teams
description: Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 62dba210d4fbf7d3540df7fd58d33e275f0065c3
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990252"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="f2189-103">Provedor do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f2189-103">Microsoft Teams provider</span></span>

<span data-ttu-id="f2189-104">Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="f2189-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="f2189-105">Para saber mais, veja [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="f2189-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="f2189-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="f2189-106">Get started</span></span>

<span data-ttu-id="f2189-107">Antes de usar o provedor do Teams, você precisará certificar-se de que você referenciou o [SDK do Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) na sua página.</span><span class="sxs-lookup"><span data-stu-id="f2189-107">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

### <a name="via-script-tag"></a><span data-ttu-id="f2189-108">via marca de script</span><span class="sxs-lookup"><span data-stu-id="f2189-108">via script tag</span></span>
<span data-ttu-id="f2189-109">O exemplo a seguir usa o provedor em HTML (via CDN).</span><span class="sxs-lookup"><span data-stu-id="f2189-109">The following example uses the provider in HTML (via CDN).</span></span>

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
  authority=""
></mgt-teams-provider>
```

| <span data-ttu-id="f2189-110">Atributo</span><span class="sxs-lookup"><span data-stu-id="f2189-110">Attribute</span></span> | <span data-ttu-id="f2189-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2189-111">Description</span></span> |
| --- | --- |
| <span data-ttu-id="f2189-112">Client-ID</span><span class="sxs-lookup"><span data-stu-id="f2189-112">client-id</span></span>   | <span data-ttu-id="f2189-113">ID do cliente de cadeia de caracteres (consulte [Configure Your Teams app](#configure-your-teams-app).</span><span class="sxs-lookup"><span data-stu-id="f2189-113">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="f2189-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2189-114">Required.</span></span> |
| <span data-ttu-id="f2189-115">auth-Popup-URL</span><span class="sxs-lookup"><span data-stu-id="f2189-115">auth-popup-url</span></span>  | <span data-ttu-id="f2189-116">Caminho absoluto ou relativo para a página que manipulará a autenticação no pop-up (consulte [criar a página pop-up](#create-the-popup-page)).</span><span class="sxs-lookup"><span data-stu-id="f2189-116">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="f2189-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2189-117">Required.</span></span> |
| <span data-ttu-id="f2189-118">escopos</span><span class="sxs-lookup"><span data-stu-id="f2189-118">scopes</span></span>  | <span data-ttu-id="f2189-119">Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar.</span><span class="sxs-lookup"><span data-stu-id="f2189-119">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="f2189-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f2189-120">Optional.</span></span> |
| <span data-ttu-id="f2189-121">depende de</span><span class="sxs-lookup"><span data-stu-id="f2189-121">depends-on</span></span> | <span data-ttu-id="f2189-122">Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="f2189-122">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="f2189-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f2189-123">Optional.</span></span> |
| <span data-ttu-id="f2189-124">autoridades</span><span class="sxs-lookup"><span data-stu-id="f2189-124">authority</span></span>    | <span data-ttu-id="f2189-125">Cadeia de caracteres de autoridade.</span><span class="sxs-lookup"><span data-stu-id="f2189-125">Authority string.</span></span> <span data-ttu-id="f2189-126">O padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="f2189-126">The default is the common authority.</span></span> <span data-ttu-id="f2189-127">Para aplicativos de locatário único, use a ID de locatário ou o nome do locatário.</span><span class="sxs-lookup"><span data-stu-id="f2189-127">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="f2189-128">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="f2189-128">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="f2189-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f2189-129">Optional.</span></span> |


### <a name="via-npm"></a><span data-ttu-id="f2189-130">via NPM</span><span class="sxs-lookup"><span data-stu-id="f2189-130">via NPM</span></span>
<span data-ttu-id="f2189-131">O exemplo a seguir usa o provedor em módulos JS (via NPM).</span><span class="sxs-lookup"><span data-stu-id="f2189-131">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="f2189-132">Certifique-se de instalar o kit de ferramentas e o SDK do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f2189-132">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="f2189-133">Em seguida, importe e use o provedor.</span><span class="sxs-lookup"><span data-stu-id="f2189-133">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt';
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="f2189-134">onde `config` é</span><span class="sxs-lookup"><span data-stu-id="f2189-134">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="f2189-135">Como alternativa, você pode precisar definir a referência à biblioteca do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f2189-135">Alternatively, you might need to set the reference to the Microsoft Teams Library.</span></span> <span data-ttu-id="f2189-136">Veja um exemplo:</span><span class="sxs-lookup"><span data-stu-id="f2189-136">Here is an example:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="f2189-137">Para ver um exemplo completo, confira o [exemplo de guia do Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span><span class="sxs-lookup"><span data-stu-id="f2189-137">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="f2189-138">Configurar seu aplicativo do teams</span><span class="sxs-lookup"><span data-stu-id="f2189-138">Configure your Teams app</span></span>

<span data-ttu-id="f2189-139">Se você estiver apenas começando a usar o Teams apps, consulte [adicionar guias aos aplicativos do Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="f2189-139">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="f2189-140">Você também pode usar o [app Studio](/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2189-140">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="f2189-141">Após instalar seu aplicativo com uma guia e você estiver pronto para usar os componentes, você precisará certificar-se de que seu aplicativo tem as permissões corretas para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f2189-141">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="f2189-142">Para configurar seu aplicativo com as permissões necessárias:</span><span class="sxs-lookup"><span data-stu-id="f2189-142">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="f2189-143">Recuperar seu nome de domínio</span><span class="sxs-lookup"><span data-stu-id="f2189-143">Retrieve your domain name</span></span>](/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="f2189-144">Criar um novo registro de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2189-144">Create a new app registration</span></span>](/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [<span data-ttu-id="f2189-145">Conceder sua permissão de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2189-145">Grant your application permission</span></span>](/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="f2189-146">É importante adicionar a permissão certa na **página Adicionar acesso à API**.</span><span class="sxs-lookup"><span data-stu-id="f2189-146">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="f2189-147">Você precisará de um administrador para adicionar e aprovar as permissões, dependendo de qual componente você precisa.</span><span class="sxs-lookup"><span data-stu-id="f2189-147">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="f2189-148">**Dica:** Se você não tiver certeza sobre as permissões a serem adicionadas, consulte a documentação de cada componente.</span><span class="sxs-lookup"><span data-stu-id="f2189-148">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="f2189-149">Habilitar fluxo de concessão implícito</span><span class="sxs-lookup"><span data-stu-id="f2189-149">Enable implicit grant Flow</span></span>

<span data-ttu-id="f2189-150">Certifique-se de habilitar o fluxo de concessão implícito; Esse é um requisito para aplicativos Web que solicitam tokens do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="f2189-150">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="f2189-151">No portal do Azure, ao gerenciar o registro do aplicativo, edite o manifesto e altere `oauth2AllowImplicitFlow` para `true` .</span><span class="sxs-lookup"><span data-stu-id="f2189-151">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="f2189-152">Criar a página pop-up</span><span class="sxs-lookup"><span data-stu-id="f2189-152">Create the popup page</span></span>

<span data-ttu-id="f2189-153">Para entrar com suas credenciais do Microsoft Teams, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up, o que irá seguir o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f2189-153">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="f2189-154">Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método.</span><span class="sxs-lookup"><span data-stu-id="f2189-154">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="f2189-155">Essa é a única coisa que esta página precisa fazer.</span><span class="sxs-lookup"><span data-stu-id="f2189-155">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="f2189-156">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="f2189-156">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

<span data-ttu-id="f2189-157">ou por um módulo mencionado na página pop-up de autenticação:</span><span class="sxs-lookup"><span data-stu-id="f2189-157">or via a module referenced in your auth popup page:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="f2189-158">Configurar URIs de redirecionamento</span><span class="sxs-lookup"><span data-stu-id="f2189-158">Configure redirect URIs</span></span>

<span data-ttu-id="f2189-159">Após publicar esta página no seu site, você precisará usar a URL na `auth-popup-url/authPopupUrl` propriedade.</span><span class="sxs-lookup"><span data-stu-id="f2189-159">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="f2189-160">Essa URL também precisa ser configurada como um URI de redirecionamento válido em sua configuração de aplicativo no portal do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f2189-160">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
