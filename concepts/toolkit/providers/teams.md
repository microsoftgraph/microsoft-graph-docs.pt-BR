---
title: Provedor do Microsoft Teams
description: Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 463fa4afdfd4e0dd3e3cb09ad155f0cae08fb347
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664034"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="50136-103">Provedor do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="50136-103">Microsoft Teams provider</span></span>

<span data-ttu-id="50136-104">Use o provedor de equipes dentro da guia do Microsoft Teams para facilitar a autenticação e o acesso ao Microsoft Graph a todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="50136-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="50136-105">Para saber mais sobre provedores de autenticação, consulte [Providers](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="50136-105">To learn more about authentication providers, see [providers](./providers.md).</span></span>

><span data-ttu-id="50136-106">**Dica:** Para obter detalhes sobre como começar a criar um aplicativo do Microsoft Teams com o provedor Teams, consulte o guia criar um guia de introdução ao [Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md) .</span><span class="sxs-lookup"><span data-stu-id="50136-106">**Tip:** For details about how to get started with creating a Microsoft Teams application with the Teams Provider, see the [Build a Microsoft Teams tab](../get-started/build-a-microsoft-teams-tab.md) getting started guide.</span></span>

## <a name="get-started"></a><span data-ttu-id="50136-107">Introdução</span><span class="sxs-lookup"><span data-stu-id="50136-107">Get started</span></span>

<span data-ttu-id="50136-108">Antes de usar o provedor do Teams, você precisará certificar-se de que você referenciou o [SDK do Microsoft Teams](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) na sua página.</span><span class="sxs-lookup"><span data-stu-id="50136-108">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) in your page.</span></span>

# <a name="npm"></a>[<span data-ttu-id="50136-109">npm</span><span class="sxs-lookup"><span data-stu-id="50136-109">npm</span></span>](#tab/ts)

<span data-ttu-id="50136-110">Certifique-se de instalar o kit de ferramentas e o SDK do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="50136-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="50136-111">Em seguida, importe e use o provedor.</span><span class="sxs-lookup"><span data-stu-id="50136-111">Next, import and use the provider.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="50136-112">onde `config` é</span><span class="sxs-lookup"><span data-stu-id="50136-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
}
```

# <a name="unpkg"></a>[<span data-ttu-id="50136-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="50136-113">unpkg</span></span>](#tab/html)

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="/AUTH-PATH"
  scopes="User.Read,People.Read..."
  authority=""
></mgt-teams-provider>
```

### <a name="mgt-teams-provider-attributes"></a><span data-ttu-id="50136-114">provedores de gerenciamento de equipes</span><span class="sxs-lookup"><span data-stu-id="50136-114">mgt-teams-provider attributes</span></span>
| <span data-ttu-id="50136-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="50136-115">Attribute</span></span> | <span data-ttu-id="50136-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="50136-116">Description</span></span> |
| --- | --- |
| <span data-ttu-id="50136-117">Client-ID</span><span class="sxs-lookup"><span data-stu-id="50136-117">client-id</span></span>   | <span data-ttu-id="50136-118">ID do cliente de cadeia de caracteres (consulte [Configure Your Teams app](#configure-your-teams-app).</span><span class="sxs-lookup"><span data-stu-id="50136-118">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="50136-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50136-119">Required.</span></span> |
| <span data-ttu-id="50136-120">auth-Popup-URL</span><span class="sxs-lookup"><span data-stu-id="50136-120">auth-popup-url</span></span>  | <span data-ttu-id="50136-121">Caminho absoluto ou relativo para a página que manipulará a autenticação no pop-up (consulte [criar a página pop-up](#create-the-popup-page)).</span><span class="sxs-lookup"><span data-stu-id="50136-121">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="50136-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50136-122">Required.</span></span> |
| <span data-ttu-id="50136-123">escopos</span><span class="sxs-lookup"><span data-stu-id="50136-123">scopes</span></span>  | <span data-ttu-id="50136-124">Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar.</span><span class="sxs-lookup"><span data-stu-id="50136-124">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="50136-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="50136-125">Optional.</span></span> |
| <span data-ttu-id="50136-126">depende de</span><span class="sxs-lookup"><span data-stu-id="50136-126">depends-on</span></span> | <span data-ttu-id="50136-127">Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="50136-127">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="50136-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="50136-128">Optional.</span></span> |
| <span data-ttu-id="50136-129">autoridades</span><span class="sxs-lookup"><span data-stu-id="50136-129">authority</span></span>    | <span data-ttu-id="50136-130">Cadeia de caracteres de autoridade.</span><span class="sxs-lookup"><span data-stu-id="50136-130">Authority string.</span></span> <span data-ttu-id="50136-131">O padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="50136-131">The default is the common authority.</span></span> <span data-ttu-id="50136-132">Para aplicativos de locatário único, use a ID de locatário ou o nome do locatário.</span><span class="sxs-lookup"><span data-stu-id="50136-132">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="50136-133">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="50136-133">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="50136-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="50136-134">Optional.</span></span> |

---

### <a name="create-the-popup-page"></a><span data-ttu-id="50136-135">Criar a página pop-up</span><span class="sxs-lookup"><span data-stu-id="50136-135">Create the popup page</span></span>

<span data-ttu-id="50136-136">Para entrar com suas credenciais do Microsoft Teams, você precisa fornecer uma URL que o aplicativo Teams abrirá em um pop-up, o que irá seguir o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="50136-136">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="50136-137">Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método.</span><span class="sxs-lookup"><span data-stu-id="50136-137">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="50136-138">Essa é a única coisa que esta página precisa fazer.</span><span class="sxs-lookup"><span data-stu-id="50136-138">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="50136-139">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="50136-139">For example:</span></span>

# <a name="npm"></a>[<span data-ttu-id="50136-140">npm</span><span class="sxs-lookup"><span data-stu-id="50136-140">npm</span></span>](#tab/ts)

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = MicrosoftTeams;
TeamsProvider.handleAuth();
```

# <a name="unpkg"></a>[<span data-ttu-id="50136-141">unpkg</span><span class="sxs-lookup"><span data-stu-id="50136-141">unpkg</span></span>](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```
---

### <a name="configure-redirect-uris"></a><span data-ttu-id="50136-142">Configurar URIs de redirecionamento</span><span class="sxs-lookup"><span data-stu-id="50136-142">Configure redirect URIs</span></span>

<span data-ttu-id="50136-143">Após publicar a página pop-up no seu site, você precisará usar a URL na `auth-popup-url/authPopupUrl` propriedade.</span><span class="sxs-lookup"><span data-stu-id="50136-143">After you publish the popup page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="50136-144">Essa URL também precisa ser configurada como um URI de redirecionamento válido em sua configuração de aplicativo no portal do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50136-144">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="50136-145">Configurar seu aplicativo do teams</span><span class="sxs-lookup"><span data-stu-id="50136-145">Configure your Teams app</span></span>

<span data-ttu-id="50136-146">Se você estiver apenas começando a usar o Teams apps, consulte [adicionar guias aos aplicativos do Microsoft Teams](/microsoftteams/platform/concepts/tabs/tabs-overview).</span><span class="sxs-lookup"><span data-stu-id="50136-146">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="50136-147">Você também pode usar o [app Studio](/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50136-147">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>
### <a name="creating-an-appclient-id"></a><span data-ttu-id="50136-148">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="50136-148">Creating an app/client ID</span></span>
<span data-ttu-id="50136-149">Para obter uma ID de cliente, você precisa [registrar seu aplicativo](../get-started/add-aad-app-registration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50136-149">In order to get a client ID, you need to [register your application](../get-started/add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="50136-150">**Observação**: o MSAL só dá suporte ao fluxo implícito do OAuth.</span><span class="sxs-lookup"><span data-stu-id="50136-150">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="50136-151">Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="50136-151">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="50136-152">Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="50136-152">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="see-also"></a><span data-ttu-id="50136-153">Também consulte</span><span class="sxs-lookup"><span data-stu-id="50136-153">See also</span></span>
* [<span data-ttu-id="50136-154">Exemplo de guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="50136-154">Microsoft Teams tab sample</span></span>](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [<span data-ttu-id="50136-155">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="50136-155">Build a Microsoft Teams tab</span></span>](../get-started/build-a-microsoft-teams-tab.md)