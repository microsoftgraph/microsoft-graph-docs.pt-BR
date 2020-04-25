---
title: Provedor MSAL
description: O provedor MSAL usa MSAL. js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 84962c0df0be9012f09ba8a87e17dcd3954d6e22
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806015"
---
# <a name="msal-provider"></a><span data-ttu-id="566b9-103">Provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="566b9-103">MSAL provider</span></span>

<span data-ttu-id="566b9-104">O provedor MSAL usa [MSAL. js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="566b9-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="566b9-105">Para saber mais, veja [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="566b9-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="566b9-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="566b9-106">Get started</span></span>

<span data-ttu-id="566b9-107">Você pode inicializar o provedor MSAL em HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="566b9-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="566b9-108">Inicializar na página HTML</span><span class="sxs-lookup"><span data-stu-id="566b9-108">Initialize in your HTML page</span></span>

<span data-ttu-id="566b9-109">Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor.</span><span class="sxs-lookup"><span data-stu-id="566b9-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="566b9-110">Use o `mgt-msal-provider` componente para definir a **ID do cliente** e outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="566b9-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="566b9-111">Isso criará uma nova `UserAgentApplication` instância que será usada para todos os tokens de autenticação e aquisição.</span><span class="sxs-lookup"><span data-stu-id="566b9-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="566b9-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="566b9-112">Attribute</span></span> | <span data-ttu-id="566b9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="566b9-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="566b9-114">Client-ID</span><span class="sxs-lookup"><span data-stu-id="566b9-114">client-id</span></span>   | <span data-ttu-id="566b9-115">String Client ID (consulte Creating a app/Client ID).</span><span class="sxs-lookup"><span data-stu-id="566b9-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="566b9-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="566b9-116">Required.</span></span>|
| <span data-ttu-id="566b9-117">tipo de logon</span><span class="sxs-lookup"><span data-stu-id="566b9-117">login-type</span></span>  | <span data-ttu-id="566b9-118">A enumeração `redirect` entre `popup` e o valor padrão `redirect`é.</span><span class="sxs-lookup"><span data-stu-id="566b9-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="566b9-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="566b9-119">Optional.</span></span> |
| <span data-ttu-id="566b9-120">escopos</span><span class="sxs-lookup"><span data-stu-id="566b9-120">scopes</span></span>  | <span data-ttu-id="566b9-121">Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar.</span><span class="sxs-lookup"><span data-stu-id="566b9-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="566b9-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="566b9-122">Optional.</span></span>|
| <span data-ttu-id="566b9-123">autoridades</span><span class="sxs-lookup"><span data-stu-id="566b9-123">authority</span></span>  | <span data-ttu-id="566b9-124">A cadeia de caracteres de autoridade-padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="566b9-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="566b9-125">Para aplicativos de locatário único, use a ID de locatário ou o nome do locatário.</span><span class="sxs-lookup"><span data-stu-id="566b9-125">For single-tenant apps, use your tenant ID or tenant name.</span></span> <span data-ttu-id="566b9-126">Por exemplo, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` ou `https://login.microsoftonline.com/[your-tenant-id]`.</span><span class="sxs-lookup"><span data-stu-id="566b9-126">For example, `https://login.microsoftonline.com/[your-tenant-name].onmicrosoft.com` or `https://login.microsoftonline.com/[your-tenant-id]`.</span></span> <span data-ttu-id="566b9-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="566b9-127">Optional.</span></span>|
| <span data-ttu-id="566b9-128">depende de</span><span class="sxs-lookup"><span data-stu-id="566b9-128">depends-on</span></span> | <span data-ttu-id="566b9-129">Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="566b9-129">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="566b9-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="566b9-130">Optional.</span></span> |

### <a name="initialize-in-javascript"></a><span data-ttu-id="566b9-131">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="566b9-131">Initialize in JavaScript</span></span>

<span data-ttu-id="566b9-132">Você pode fornecer mais opções inicializando o provedor no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="566b9-132">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="566b9-133">onde MsalConfig é:</span><span class="sxs-lookup"><span data-stu-id="566b9-133">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="566b9-134">Você deve fornecer um `clientId` (para criar um novo `UserAgentApplication`).</span><span class="sxs-lookup"><span data-stu-id="566b9-134">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="566b9-135">Para saber mais sobre o MSAL. js e as opções adicionais que você pode usar ao inicializar a biblioteca do MSAL, consulte a [documentação do MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-js-initializing-client-applications).</span><span class="sxs-lookup"><span data-stu-id="566b9-135">To learn more about MSAL.js and for additional options you can use when initializing the MSAL library, see the [MSAL documentation](https://docs.microsoft.com/azure/active-directory/develop/msal-js-initializing-client-applications).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="566b9-136">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="566b9-136">Creating an app/client ID</span></span>

<span data-ttu-id="566b9-137">Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte o [início rápido registrar um aplicativo](/azure/active-directory/develop/quickstart-register-app).</span><span class="sxs-lookup"><span data-stu-id="566b9-137">For details about how to register an app and get a client ID, see the [Register an app quick start](/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="566b9-138">**Observação:** MSAL só oferece suporte ao fluxo implícito para OAuth.</span><span class="sxs-lookup"><span data-stu-id="566b9-138">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="566b9-139">Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="566b9-139">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="566b9-140">Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="566b9-140">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span> <span data-ttu-id="566b9-141">Para usar a autoridade comum, defina **Account em qualquer diretório organizacional**.</span><span class="sxs-lookup"><span data-stu-id="566b9-141">To use the common authority, set **Account in any organizational directory**.</span></span> <span data-ttu-id="566b9-142">Para usar um locatário específico, defina o `authority` durante a inicialização.</span><span class="sxs-lookup"><span data-stu-id="566b9-142">To use a specific tenant, set the `authority` during initialization.</span></span>
