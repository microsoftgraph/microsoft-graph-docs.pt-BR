---
title: Provedor MSAL
description: O provedor MSAL usa MSAL.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0edb6fba29c5ee0dcb37199db055761088408be6
ms.sourcegitcommit: 186d738f04e5a558da423f2429165fb4fbe780aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086610"
---
# <a name="msal-provider"></a><span data-ttu-id="5428b-103">Provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="5428b-103">MSAL provider</span></span>

<span data-ttu-id="5428b-104">O provedor MSAL usa [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5428b-104">The MSAL provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with Microsoft Graph.</span></span>

<span data-ttu-id="5428b-105">Para saber mais, veja [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="5428b-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="5428b-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="5428b-106">Get started</span></span>

<span data-ttu-id="5428b-107">Você pode inicializar o provedor MSAL em HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="5428b-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="5428b-108">Inicializar na página HTML</span><span class="sxs-lookup"><span data-stu-id="5428b-108">Initialize in your HTML page</span></span>

<span data-ttu-id="5428b-109">Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor.</span><span class="sxs-lookup"><span data-stu-id="5428b-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="5428b-110">Use o `mgt-msal-provider` componente para definir a **ID do cliente** e outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="5428b-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="5428b-111">Isso criará uma nova `UserAgentApplication` instância que será usada para todos os tokens de autenticação e aquisição.</span><span class="sxs-lookup"><span data-stu-id="5428b-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   redirect-uri="https://my.redirect/uri"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="5428b-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="5428b-112">Attribute</span></span>    | <span data-ttu-id="5428b-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5428b-113">Description</span></span>                                                                                                                                                                                                                                                           |
|--------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5428b-114">Client-ID</span><span class="sxs-lookup"><span data-stu-id="5428b-114">client-id</span></span>    | <span data-ttu-id="5428b-115">String Client ID (consulte Creating a app/Client ID).</span><span class="sxs-lookup"><span data-stu-id="5428b-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="5428b-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5428b-116">Required.</span></span>                                                                                                                                                                                                           |
| <span data-ttu-id="5428b-117">tipo de logon</span><span class="sxs-lookup"><span data-stu-id="5428b-117">login-type</span></span>   | <span data-ttu-id="5428b-118">A enumeração entre `redirect` e o `popup` valor padrão é `redirect` .</span><span class="sxs-lookup"><span data-stu-id="5428b-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="5428b-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5428b-119">Optional.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="5428b-120">escopos</span><span class="sxs-lookup"><span data-stu-id="5428b-120">scopes</span></span>       | <span data-ttu-id="5428b-121">Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar.</span><span class="sxs-lookup"><span data-stu-id="5428b-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="5428b-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5428b-122">Optional.</span></span>                                                                                                                                                                                     |
| <span data-ttu-id="5428b-123">autoridades</span><span class="sxs-lookup"><span data-stu-id="5428b-123">authority</span></span>    | <span data-ttu-id="5428b-124">A cadeia de caracteres de autoridade-padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="5428b-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="5428b-125">Para aplicativos de locatário único, use a ID de locatário ou o nome do locatário.</span><span class="sxs-lookup"><span data-stu-id="5428b-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="5428b-126">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]` .</span><span class="sxs-lookup"><span data-stu-id="5428b-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="5428b-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5428b-127">Optional.</span></span> |
| <span data-ttu-id="5428b-128">Redirect-URI</span><span class="sxs-lookup"><span data-stu-id="5428b-128">redirect-uri</span></span> | <span data-ttu-id="5428b-129">Redirecionar cadeia de caracteres URI-por padrão, o URI de janela atual é usado.</span><span class="sxs-lookup"><span data-stu-id="5428b-129">Redirect URI string - by default the current window URI is used.</span></span> <span data-ttu-id="5428b-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5428b-130">Optional.</span></span>                                                                                                                                                                                            |
| <span data-ttu-id="5428b-131">depende de</span><span class="sxs-lookup"><span data-stu-id="5428b-131">depends-on</span></span>   | <span data-ttu-id="5428b-132">Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="5428b-132">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="5428b-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5428b-133">Optional.</span></span>                                                                                                                                                                                      |

### <a name="initialize-in-javascript"></a><span data-ttu-id="5428b-134">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="5428b-134">Initialize in JavaScript</span></span>

<span data-ttu-id="5428b-135">Você pode fornecer mais opções inicializando o provedor no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="5428b-135">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="5428b-136">onde MsalConfig é:</span><span class="sxs-lookup"><span data-stu-id="5428b-136">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  redirectUri?: string;
  loginType?: LoginType; // LoginType.Popup or LoginType.Redirect (redirect is default)
  loginHint?: string
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="5428b-137">Você deve fornecer um `clientId` (para criar um novo `UserAgentApplication` ).</span><span class="sxs-lookup"><span data-stu-id="5428b-137">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="5428b-138">Para saber mais sobre MSAL.js e para opções adicionais que você pode usar ao inicializar a biblioteca do MSAL, consulte a [documentação do MSAL](/azure/active-directory/develop/msal-js-initializing-client-applications).</span><span class="sxs-lookup"><span data-stu-id="5428b-138">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="5428b-139">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="5428b-139">Creating an app/client ID</span></span>

<span data-ttu-id="5428b-140">Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte [criar um aplicativo do Azure Active Directory](../get-started/add-aad-app-registration.md).</span><span class="sxs-lookup"><span data-stu-id="5428b-140">For details about how to register an app and get a client ID, see [Create an Azure Active Directory app](../get-started/add-aad-app-registration.md).</span></span>