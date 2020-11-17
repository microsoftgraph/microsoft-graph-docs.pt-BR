---
title: Provedor do Microsoft Teams
description: Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b102d216b9a9b4181fa070c6c95f543098fa0ba0
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086603"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="17c5c-103">Provedor do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="17c5c-103">Microsoft Teams provider</span></span>

<span data-ttu-id="17c5c-104">Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="17c5c-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="17c5c-105">Para saber mais sobre provedores de autenticação, consulte [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="17c5c-105">To learn more about authentication providers, see [providers](../providers.md).</span></span>

><span data-ttu-id="17c5c-106">**Dica:** Para obter detalhes sobre como começar a criar um aplicativo do Microsot Teams com o provedor Teams, consulte o guia [criar uma guia de introdução ao Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md) .</span><span class="sxs-lookup"><span data-stu-id="17c5c-106">**Tip:** For details about how to get started with creating a Microsot Teams application with the Teams Provider, see the [Build a Microsoft Teams tab](../get-started/build-a-microsoft-teams-tab.md) getting started guide.</span></span>

## <a name="get-started"></a><span data-ttu-id="17c5c-107">Introdução</span><span class="sxs-lookup"><span data-stu-id="17c5c-107">Get started</span></span>

<span data-ttu-id="17c5c-108">Antes de usar o provedor do Teams, você precisará certificar-se de que você referenciou o [SDK do Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) na sua página.</span><span class="sxs-lookup"><span data-stu-id="17c5c-108">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

### <a name="via-script-tag"></a><span data-ttu-id="17c5c-109">via marca de script</span><span class="sxs-lookup"><span data-stu-id="17c5c-109">via script tag</span></span>
<span data-ttu-id="17c5c-110">O exemplo a seguir usa o provedor em HTML (via CDN).</span><span class="sxs-lookup"><span data-stu-id="17c5c-110">The following example uses the provider in HTML (via CDN).</span></span>

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

| <span data-ttu-id="17c5c-111">Atributo</span><span class="sxs-lookup"><span data-stu-id="17c5c-111">Attribute</span></span> | <span data-ttu-id="17c5c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="17c5c-112">Description</span></span> |
| --- | --- |
| <span data-ttu-id="17c5c-113">Client-ID</span><span class="sxs-lookup"><span data-stu-id="17c5c-113">client-id</span></span>   | <span data-ttu-id="17c5c-114">ID do cliente de cadeia de caracteres (consulte [Configure Your Teams app](#configure-your-teams-app).</span><span class="sxs-lookup"><span data-stu-id="17c5c-114">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="17c5c-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17c5c-115">Required.</span></span> |
| <span data-ttu-id="17c5c-116">auth-Popup-URL</span><span class="sxs-lookup"><span data-stu-id="17c5c-116">auth-popup-url</span></span>  | <span data-ttu-id="17c5c-117">Caminho absoluto ou relativo para a página que manipulará a autenticação no pop-up (consulte [criar a página pop-up](#create-the-popup-page)).</span><span class="sxs-lookup"><span data-stu-id="17c5c-117">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="17c5c-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17c5c-118">Required.</span></span> |
| <span data-ttu-id="17c5c-119">escopos</span><span class="sxs-lookup"><span data-stu-id="17c5c-119">scopes</span></span>  | <span data-ttu-id="17c5c-120">Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar.</span><span class="sxs-lookup"><span data-stu-id="17c5c-120">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="17c5c-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="17c5c-121">Optional.</span></span> |
| <span data-ttu-id="17c5c-122">depende de</span><span class="sxs-lookup"><span data-stu-id="17c5c-122">depends-on</span></span> | <span data-ttu-id="17c5c-123">Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="17c5c-123">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="17c5c-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="17c5c-124">Optional.</span></span> |
| <span data-ttu-id="17c5c-125">autoridades</span><span class="sxs-lookup"><span data-stu-id="17c5c-125">authority</span></span>    | <span data-ttu-id="17c5c-126">Cadeia de caracteres de autoridade.</span><span class="sxs-lookup"><span data-stu-id="17c5c-126">Authority string.</span></span> <span data-ttu-id="17c5c-127">O padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="17c5c-127">The default is the common authority.</span></span> <span data-ttu-id="17c5c-128">Para aplicativos de locatário único, use a ID de locatário ou o nome do locatário.</span><span class="sxs-lookup"><span data-stu-id="17c5c-128">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="17c5c-129">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="17c5c-129">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="17c5c-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="17c5c-130">Optional.</span></span> |


### <a name="via-npm"></a><span data-ttu-id="17c5c-131">via NPM</span><span class="sxs-lookup"><span data-stu-id="17c5c-131">via NPM</span></span>
<span data-ttu-id="17c5c-132">O exemplo a seguir usa o provedor em módulos JS (via NPM).</span><span class="sxs-lookup"><span data-stu-id="17c5c-132">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="17c5c-133">Certifique-se de instalar o kit de ferramentas e o SDK do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="17c5c-133">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="17c5c-134">Em seguida, importe e use o provedor.</span><span class="sxs-lookup"><span data-stu-id="17c5c-134">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt';
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="17c5c-135">onde `config` é</span><span class="sxs-lookup"><span data-stu-id="17c5c-135">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="17c5c-136">Como alternativa, você pode precisar definir a referência à biblioteca do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="17c5c-136">Alternatively, you might need to set the reference to the Microsoft Teams Library.</span></span> <span data-ttu-id="17c5c-137">Veja um exemplo:</span><span class="sxs-lookup"><span data-stu-id="17c5c-137">Here is an example:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="17c5c-138">Para ver um exemplo completo, confira o [exemplo de guia do Microsoft Teams](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span><span class="sxs-lookup"><span data-stu-id="17c5c-138">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="17c5c-139">Configurar seu aplicativo do teams</span><span class="sxs-lookup"><span data-stu-id="17c5c-139">Configure your Teams app</span></span>

<span data-ttu-id="17c5c-140">Se você estiver apenas começando a usar o Teams apps, consulte [adicionar guias aos aplicativos do Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="17c5c-140">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="17c5c-141">Você também pode usar o [app Studio](/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17c5c-141">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="17c5c-142">Após instalar seu aplicativo com uma guia e você estiver pronto para usar os componentes, você precisará certificar-se de que seu aplicativo tem as permissões corretas para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="17c5c-142">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="17c5c-143">Para configurar seu aplicativo com as permissões necessárias:</span><span class="sxs-lookup"><span data-stu-id="17c5c-143">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="17c5c-144">Recuperar seu nome de domínio</span><span class="sxs-lookup"><span data-stu-id="17c5c-144">Retrieve your domain name</span></span>](/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="17c5c-145">Criar um novo registro de aplicativo</span><span class="sxs-lookup"><span data-stu-id="17c5c-145">Create a new app registration</span></span>](../get-started/add-aad-app-registration.md)
3. [<span data-ttu-id="17c5c-146">Conceder sua permissão de aplicativo</span><span class="sxs-lookup"><span data-stu-id="17c5c-146">Grant your application permission</span></span>](/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="17c5c-147">É importante adicionar a permissão certa na **página Adicionar acesso à API**.</span><span class="sxs-lookup"><span data-stu-id="17c5c-147">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="17c5c-148">Você precisará de um administrador para adicionar e aprovar as permissões, dependendo de qual componente você precisa.</span><span class="sxs-lookup"><span data-stu-id="17c5c-148">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="17c5c-149">**Dica:** Se você não tiver certeza sobre as permissões a serem adicionadas, consulte a documentação de cada componente.</span><span class="sxs-lookup"><span data-stu-id="17c5c-149">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="17c5c-150">Habilitar fluxo de concessão implícito</span><span class="sxs-lookup"><span data-stu-id="17c5c-150">Enable implicit grant Flow</span></span>

<span data-ttu-id="17c5c-151">Certifique-se de habilitar o fluxo de concessão implícito; Esse é um requisito para aplicativos Web que solicitam tokens do lado do cliente.</span><span class="sxs-lookup"><span data-stu-id="17c5c-151">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="17c5c-152">No portal do Azure, ao gerenciar o registro do aplicativo, edite o manifesto e altere `oauth2AllowImplicitFlow` para `true` .</span><span class="sxs-lookup"><span data-stu-id="17c5c-152">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="17c5c-153">Criar a página pop-up</span><span class="sxs-lookup"><span data-stu-id="17c5c-153">Create the popup page</span></span>

<span data-ttu-id="17c5c-154">Para entrar com suas credenciais do Microsoft Teams, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up, o que irá seguir o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="17c5c-154">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="17c5c-155">Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método.</span><span class="sxs-lookup"><span data-stu-id="17c5c-155">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="17c5c-156">Essa é a única coisa que esta página precisa fazer.</span><span class="sxs-lookup"><span data-stu-id="17c5c-156">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="17c5c-157">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="17c5c-157">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```

<span data-ttu-id="17c5c-158">ou por um módulo mencionado na página pop-up de autenticação:</span><span class="sxs-lookup"><span data-stu-id="17c5c-158">or via a module referenced in your auth popup page:</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="17c5c-159">Configurar URIs de redirecionamento</span><span class="sxs-lookup"><span data-stu-id="17c5c-159">Configure redirect URIs</span></span>

<span data-ttu-id="17c5c-160">Após publicar esta página no seu site, você precisará usar a URL na `auth-popup-url/authPopupUrl` propriedade.</span><span class="sxs-lookup"><span data-stu-id="17c5c-160">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="17c5c-161">Essa URL também precisa ser configurada como um URI de redirecionamento válido em sua configuração de aplicativo no portal do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17c5c-161">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
