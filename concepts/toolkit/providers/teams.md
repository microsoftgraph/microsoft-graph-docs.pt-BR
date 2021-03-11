---
title: Provedor do Microsoft Teams
description: Use o provedor do Teams dentro de sua guia do Microsoft Teams para facilitar a autenticação e o acesso do Microsoft Graph a todos os componentes.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 2d4bff6363cc87256f7ec3f9456fbd11f011b48e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719750"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="84958-103">Provedor do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="84958-103">Microsoft Teams provider</span></span>

<span data-ttu-id="84958-104">Use o provedor do Teams dentro de sua guia do Microsoft Teams para facilitar a autenticação e o acesso do Microsoft Graph a todos os componentes.</span><span class="sxs-lookup"><span data-stu-id="84958-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="84958-105">Para saber mais sobre provedores de autenticação, consulte [provedores](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="84958-105">To learn more about authentication providers, see [providers](./providers.md).</span></span>

><span data-ttu-id="84958-106">**Dica:** Para obter detalhes sobre como começar a criar um aplicativo do Microsoft Teams com o Provedor do Teams, consulte o guia [Criar uma guia do Microsoft Teams](../get-started/build-a-microsoft-teams-tab.md) começando.</span><span class="sxs-lookup"><span data-stu-id="84958-106">**Tip:** For details about how to get started with creating a Microsoft Teams application with the Teams Provider, see the [Build a Microsoft Teams tab](../get-started/build-a-microsoft-teams-tab.md) getting started guide.</span></span>

## <a name="get-started"></a><span data-ttu-id="84958-107">Introdução</span><span class="sxs-lookup"><span data-stu-id="84958-107">Get started</span></span>

<span data-ttu-id="84958-108">Antes de usar o provedor do Teams, você precisará se certificar de ter referenciado o [SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) do Microsoft Teams em sua página.</span><span class="sxs-lookup"><span data-stu-id="84958-108">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](/javascript/api/overview/msteams-client?view=msteams-client-js-latest&preserve-view=true#using-the-sdk) in your page.</span></span>

# <a name="npm"></a>[<span data-ttu-id="84958-109">npm</span><span class="sxs-lookup"><span data-stu-id="84958-109">npm</span></span>](#tab/ts)

<span data-ttu-id="84958-110">Instale o kit de ferramentas e o SDK do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="84958-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```cmd
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="84958-111">Em seguida, importe e use o provedor.</span><span class="sxs-lookup"><span data-stu-id="84958-111">Next, import and use the provider.</span></span>

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="84958-112">onde `config` está</span><span class="sxs-lookup"><span data-stu-id="84958-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string; // see below for creating the popup page
  scopes?: string[];
  msalOptions?: Configuration;
}
```

# <a name="unpkg"></a>[<span data-ttu-id="84958-113">unpkg</span><span class="sxs-lookup"><span data-stu-id="84958-113">unpkg</span></span>](#tab/html)

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

### <a name="mgt-teams-provider-attributes"></a><span data-ttu-id="84958-114">atributos mgt-teams-provider</span><span class="sxs-lookup"><span data-stu-id="84958-114">mgt-teams-provider attributes</span></span>
| <span data-ttu-id="84958-115">Atributo</span><span class="sxs-lookup"><span data-stu-id="84958-115">Attribute</span></span> | <span data-ttu-id="84958-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="84958-116">Description</span></span> |
| --- | --- |
| <span data-ttu-id="84958-117">client-id</span><span class="sxs-lookup"><span data-stu-id="84958-117">client-id</span></span>   | <span data-ttu-id="84958-118">ID do cliente de cadeia de caracteres (consulte [Configure your Teams app](#configure-your-teams-app).</span><span class="sxs-lookup"><span data-stu-id="84958-118">String client ID (see [Configure your Teams app](#configure-your-teams-app).</span></span> <span data-ttu-id="84958-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84958-119">Required.</span></span> |
| <span data-ttu-id="84958-120">auth-popup-url</span><span class="sxs-lookup"><span data-stu-id="84958-120">auth-popup-url</span></span>  | <span data-ttu-id="84958-121">Caminho absoluto ou relativo para a página que manipulará a auth no pop-up (consulte [Criar a página pop-up](#create-the-popup-page)).</span><span class="sxs-lookup"><span data-stu-id="84958-121">Absolute or relative path to the page that will handle auth in the popup (see [Create the popup page](#create-the-popup-page)).</span></span> <span data-ttu-id="84958-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84958-122">Required.</span></span> |
| <span data-ttu-id="84958-123">escopos</span><span class="sxs-lookup"><span data-stu-id="84958-123">scopes</span></span>  | <span data-ttu-id="84958-124">Cadeias de caracteres separadas por vírgulas para escopos que o usuário deve consentir ao entrar.</span><span class="sxs-lookup"><span data-stu-id="84958-124">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="84958-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="84958-125">Optional.</span></span> |
| <span data-ttu-id="84958-126">depends-on</span><span class="sxs-lookup"><span data-stu-id="84958-126">depends-on</span></span> | <span data-ttu-id="84958-127">Cadeia de caracteres do seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="84958-127">Element selector string of another higher-priority provider component.</span></span> <span data-ttu-id="84958-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="84958-128">Optional.</span></span> |
| <span data-ttu-id="84958-129">authority</span><span class="sxs-lookup"><span data-stu-id="84958-129">authority</span></span>    | <span data-ttu-id="84958-130">Cadeia de caracteres de autoridade.</span><span class="sxs-lookup"><span data-stu-id="84958-130">Authority string.</span></span> <span data-ttu-id="84958-131">O padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="84958-131">The default is the common authority.</span></span> <span data-ttu-id="84958-132">Para aplicativos de locatário único, use sua ID de locatário ou nome de locatário.</span><span class="sxs-lookup"><span data-stu-id="84958-132">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="84958-133">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="84958-133">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="84958-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="84958-134">Optional.</span></span> |

---

### <a name="create-the-popup-page"></a><span data-ttu-id="84958-135">Criar a página pop-up</span><span class="sxs-lookup"><span data-stu-id="84958-135">Create the popup page</span></span>

<span data-ttu-id="84958-136">Para entrar com suas credenciais do Teams, você precisa fornecer uma URL que o aplicativo do Teams abrirá em um pop-up, que seguirá o fluxo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="84958-136">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="84958-137">Essa URL precisa estar em seu domínio e precisa chamar o `TeamsProvider.handleAuth();` método.</span><span class="sxs-lookup"><span data-stu-id="84958-137">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="84958-138">Essa é a única coisa que essa página precisa fazer.</span><span class="sxs-lookup"><span data-stu-id="84958-138">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="84958-139">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="84958-139">For example:</span></span>

# <a name="npm"></a>[<span data-ttu-id="84958-140">npm</span><span class="sxs-lookup"><span data-stu-id="84958-140">npm</span></span>](#tab/ts)

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {Providers, TeamsProvider} from '@microsoft/mgt';

TeamsProvider.microsoftTeamsLib = microsoftTeams;
TeamsProvider.handleAuth();
```

# <a name="unpkg"></a>[<span data-ttu-id="84958-141">unpkg</span><span class="sxs-lookup"><span data-stu-id="84958-141">unpkg</span></span>](#tab/html)

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<script>
  mgt.TeamsProvider.handleAuth();
</script>
```
---

### <a name="configure-redirect-uris"></a><span data-ttu-id="84958-142">Configurar URIs de redirecionamento</span><span class="sxs-lookup"><span data-stu-id="84958-142">Configure redirect URIs</span></span>

<span data-ttu-id="84958-143">Depois de publicar a página pop-up em seu site, você precisará usar a URL na `auth-popup-url/authPopupUrl` propriedade.</span><span class="sxs-lookup"><span data-stu-id="84958-143">After you publish the popup page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="84958-144">Essa URL também precisa ser configurada como um URI de redirecionamento válido na configuração do aplicativo no portal do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84958-144">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="84958-145">Configurar seu aplicativo do Teams</span><span class="sxs-lookup"><span data-stu-id="84958-145">Configure your Teams app</span></span>

<span data-ttu-id="84958-146">Se você está apenas começando com aplicativos do Teams, consulte [Adicionar guias aos aplicativos do Microsoft Teams.](/microsoftteams/platform/concepts/tabs/tabs-overview)</span><span class="sxs-lookup"><span data-stu-id="84958-146">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="84958-147">Você também pode usar [o App Studio](/microsoftteams/platform/get-started/get-started-app-studio) para desenvolver rapidamente o manifesto do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84958-147">You can also use [App Studio](/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>
### <a name="creating-an-appclient-id"></a><span data-ttu-id="84958-148">Criando uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="84958-148">Creating an app/client ID</span></span>
<span data-ttu-id="84958-149">Para obter uma ID do cliente, você precisa registrar [seu aplicativo](../get-started/add-aad-app-registration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84958-149">In order to get a client ID, you need to [register your application](../get-started/add-aad-app-registration.md) in Azure AD.</span></span> 
><span data-ttu-id="84958-150">**Observação**: O MSAL só dá suporte ao Fluxo Implícito para OAuth.</span><span class="sxs-lookup"><span data-stu-id="84958-150">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="84958-151">Certifique-se de habilitar o Fluxo Implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="84958-151">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="84958-152">Em **Autenticação**, encontre a seção **Concessão implícita** e selecione as caixas de seleção para **tokens de Acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="84958-152">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> 

## <a name="see-also"></a><span data-ttu-id="84958-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="84958-153">See also</span></span>
* [<span data-ttu-id="84958-154">Exemplo de guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="84958-154">Microsoft Teams tab sample</span></span>](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)
* [<span data-ttu-id="84958-155">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="84958-155">Build a Microsoft Teams tab</span></span>](../get-started/build-a-microsoft-teams-tab.md)