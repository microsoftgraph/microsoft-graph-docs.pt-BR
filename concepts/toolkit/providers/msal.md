---
title: Provedor MSAL
description: O provedor MSAL usa MSAL. js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: aa3eecb6bd9f2adae7ff689f30ab69539e1d27f1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955775"
---
# <a name="msal-provider"></a><span data-ttu-id="cdcc4-103">Provedor MSAL</span><span class="sxs-lookup"><span data-stu-id="cdcc4-103">MSAL provider</span></span>

<span data-ttu-id="cdcc4-104">O provedor MSAL usa [MSAL. js](https://github.com/AzureAD/microsoft-authentication-library-for-js) para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="cdcc4-105">Para saber mais, veja [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="cdcc4-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="cdcc4-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="cdcc4-106">Get started</span></span>

<span data-ttu-id="cdcc4-107">Você pode inicializar o provedor MSAL em HTML ou JavaScript.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="cdcc4-108">Inicializar na página HTML</span><span class="sxs-lookup"><span data-stu-id="cdcc4-108">Initialize in your HTML page</span></span>

<span data-ttu-id="cdcc4-109">Inicializar o provedor MSAL em HTML é a maneira mais simples de criar um novo provedor.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="cdcc4-110">Use o `mgt-msal-provider` componente para definir a **ID do cliente** e outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="cdcc4-111">Isso criará uma nova `UserAgentApplication` instância que será usada para todos os tokens de autenticação e aquisição.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   scopes="user.read,people.read"
                   authority=""></mgt-msal-provider>
```

| <span data-ttu-id="cdcc4-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="cdcc4-112">Attribute</span></span> | <span data-ttu-id="cdcc4-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdcc4-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="cdcc4-114">Client-ID</span><span class="sxs-lookup"><span data-stu-id="cdcc4-114">client-id</span></span>   | <span data-ttu-id="cdcc4-115">String Client ID (consulte Creating a app/Client ID).</span><span class="sxs-lookup"><span data-stu-id="cdcc4-115">String client ID (see Creating an app/client ID).</span></span> <span data-ttu-id="cdcc4-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-116">Required.</span></span>|
| <span data-ttu-id="cdcc4-117">tipo de logon</span><span class="sxs-lookup"><span data-stu-id="cdcc4-117">login-type</span></span>  | <span data-ttu-id="cdcc4-118">A enumeração `redirect` entre `popup` e o valor padrão `redirect`é.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-118">Enumeration between `redirect` and `popup` - default value is `redirect`.</span></span> <span data-ttu-id="cdcc4-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-119">Optional.</span></span> |
| <span data-ttu-id="cdcc4-120">escopos</span><span class="sxs-lookup"><span data-stu-id="cdcc4-120">scopes</span></span>  | <span data-ttu-id="cdcc4-121">Cadeias de caracteres separadas por vírgula para escopos para os quais o usuário deve se concordar.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-121">Comma separated strings for scopes the user must consent to on sign in.</span></span> <span data-ttu-id="cdcc4-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-122">Optional.</span></span>|
| <span data-ttu-id="cdcc4-123">autoridades</span><span class="sxs-lookup"><span data-stu-id="cdcc4-123">authority</span></span>  | <span data-ttu-id="cdcc4-124">A cadeia de caracteres de autoridade-padrão é a autoridade comum.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-124">Authority string - default is the common authority.</span></span> <span data-ttu-id="cdcc4-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-125">Optional.</span></span>|
| <span data-ttu-id="cdcc4-126">depende de</span><span class="sxs-lookup"><span data-stu-id="cdcc4-126">depends-on</span></span> | <span data-ttu-id="cdcc4-127">Cadeia de caracteres de seletor de elemento de outro componente de provedor de prioridade mais alta.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-127">Element selector string of another higher priority provider component.</span></span> <span data-ttu-id="cdcc4-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-128">Optional.</span></span> |

### <a name="initialize-in-javascript"></a><span data-ttu-id="cdcc4-129">Inicializar em JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdcc4-129">Initialize in JavaScript</span></span>

<span data-ttu-id="cdcc4-130">Você pode fornecer mais opções inicializando o provedor no JavaScript.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-130">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="cdcc4-131">onde MsalConfig é:</span><span class="sxs-lookup"><span data-stu-id="cdcc4-131">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="cdcc4-132">Você deve fornecer um `clientId` (para criar um novo `UserAgentApplication`).</span><span class="sxs-lookup"><span data-stu-id="cdcc4-132">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="cdcc4-133">Para saber mais, confira a [documentação do MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span><span class="sxs-lookup"><span data-stu-id="cdcc4-133">To learn more, see the [MSAL documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="cdcc4-134">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="cdcc4-134">Creating an app/client ID</span></span>

<span data-ttu-id="cdcc4-135">Para obter detalhes sobre como registrar um aplicativo e obter uma ID de cliente, consulte [registrar um aplicativo início rápido](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app).</span><span class="sxs-lookup"><span data-stu-id="cdcc4-135">For details about how to register an app and get a client ID, see [Register an app quick start](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="cdcc4-136">**Observação:** MSAL só oferece suporte ao fluxo implícito para OAuth.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-136">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="cdcc4-137">Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="cdcc4-137">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="cdcc4-138">Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="cdcc4-138">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>
