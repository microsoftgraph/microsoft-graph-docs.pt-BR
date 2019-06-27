---
title: Provedor MSAL
description: O provedor MSAL usa MSAL. js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b66fd9a640c6baa84767e1ab08821b80384a5464
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242937"
---
# <a name="msal-provider"></a><span data-ttu-id="65924-103">Provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="65924-103">MSAL provider</span></span>

<span data-ttu-id="65924-104">O provedor MSAL usa [MSAL. js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="65924-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="65924-105">Para saber mais, veja [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="65924-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="65924-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="65924-106">Get started</span></span>

<span data-ttu-id="65924-107">Você pode inicializar o provedor MSAL em HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="65924-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="65924-108">Inicializar na página HTML</span><span class="sxs-lookup"><span data-stu-id="65924-108">Initialize in your HTML page</span></span>

<span data-ttu-id="65924-109">Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor.</span><span class="sxs-lookup"><span data-stu-id="65924-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="65924-110">Use o `mgt-msal-provider` componente para definir a **ID do cliente** e outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="65924-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="65924-111">Isso criará uma nova `UserAgentApplication` instância que será usada para todos os tokens de autenticação e aquisição.</span><span class="sxs-lookup"><span data-stu-id="65924-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   authority=""></mgt-msal-provider>
```

><span data-ttu-id="65924-112">**Observação:** `login-type` e `authority` são opcionais.</span><span class="sxs-lookup"><span data-stu-id="65924-112">**Note:** `login-type` and `authority` are optional.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="65924-113">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="65924-113">Initialize in JavaScript</span></span>

<span data-ttu-id="65924-114">Você pode fornecer mais opções inicializando o provedor no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="65924-114">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="65924-115">onde MsalConfig é:</span><span class="sxs-lookup"><span data-stu-id="65924-115">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="65924-116">Você deve fornecer um `clientId` (para criar um novo `UserAgentApplication`).</span><span class="sxs-lookup"><span data-stu-id="65924-116">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="65924-117">Para saber mais, confira a [documentação do MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span><span class="sxs-lookup"><span data-stu-id="65924-117">To learn more, see the [MSAL documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="65924-118">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="65924-118">Creating an app/client ID</span></span>

<span data-ttu-id="65924-119">Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte o [início rápido registrar um aplicativo](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app).</span><span class="sxs-lookup"><span data-stu-id="65924-119">For details about how to register an app and get a client ID, see the [Register an app quick start](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="65924-120">**Observação:** MSAL só oferece suporte ao fluxo implícito para OAuth.</span><span class="sxs-lookup"><span data-stu-id="65924-120">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="65924-121">Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="65924-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="65924-122">Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para tokens de **acesso** e tokens de **ID**.</span><span class="sxs-lookup"><span data-stu-id="65924-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>
