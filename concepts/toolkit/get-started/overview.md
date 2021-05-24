---
title: Iniciando o microsoft Graph Toolkit
description: Começar a usar o microsoft Graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 68260cf83f0e9bec34d2c3b23911d04c53143e76
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629151"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="6d20c-103">Iniciando o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="6d20c-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="6d20c-104">Os componentes Graph Toolkit microsoft podem ser facilmente adicionados ao seu aplicativo Web, SharePoint Web Part ou Microsoft Teams guias.</span><span class="sxs-lookup"><span data-stu-id="6d20c-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="6d20c-105">Os componentes são baseados em padrões web e podem ser usados em projetos JavaScript simples ou com estruturas da Web populares, como Reach, Angular, Vue.js e muito mais.</span><span class="sxs-lookup"><span data-stu-id="6d20c-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="6d20c-106">Você pode assistir a este vídeo curto para ver como é rápido e fácil começar com o Toolkit.</span><span class="sxs-lookup"><span data-stu-id="6d20c-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="6d20c-107">Para obter um tutorial passo a passo, consulte o [módulo Introdução ao microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/).</span><span class="sxs-lookup"><span data-stu-id="6d20c-107">For a step-by-step tutorial, see the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> 

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="6d20c-108">Configure o locatário do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6d20c-108">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="6d20c-109">Para desenvolver com o Toolkit, você precisa de acesso a um locatário Microsoft 365 locatário.</span><span class="sxs-lookup"><span data-stu-id="6d20c-109">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="6d20c-110">Se você não tiver um, poderá obter uma assinatura de desenvolvedor gratuita Microsoft 365 in [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="6d20c-110">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="6d20c-111">Para obter detalhes sobre como configurar sua assinatura, consulte [Configurar uma assinatura Microsoft 365 desenvolvedor.](/office/developer-program/microsoft-365-developer-program-get-started)</span><span class="sxs-lookup"><span data-stu-id="6d20c-111">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="6d20c-112">Defina seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="6d20c-112">Set up your development environment</span></span>
<span data-ttu-id="6d20c-113">Para desenvolver com o Toolkit, você precisará de um editor de texto ou IDE.</span><span class="sxs-lookup"><span data-stu-id="6d20c-113">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="6d20c-114">Você pode usar o editor ou o IDE de sua escolha ou instalar e [usar](https://code.visualstudio.com/download) Visual Studio Code gratuitamente.</span><span class="sxs-lookup"><span data-stu-id="6d20c-114">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="6d20c-115">Você também precisará de um navegador da Web moderno como Microsoft Edge, Google Chrome ou Firefox.</span><span class="sxs-lookup"><span data-stu-id="6d20c-115">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="6d20c-116">Você também precisará de uma versão LTS do Node.js, que pode ser instalada [nodejs.org](https://nodejs.org).</span><span class="sxs-lookup"><span data-stu-id="6d20c-116">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="6d20c-117">Usando o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="6d20c-117">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="6d20c-118">Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="6d20c-118">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="6d20c-119">unpkg</span><span class="sxs-lookup"><span data-stu-id="6d20c-119">unpkg</span></span>](#tab/html)
<span data-ttu-id="6d20c-120">Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="6d20c-120">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="6d20c-121">npm</span><span class="sxs-lookup"><span data-stu-id="6d20c-121">npm</span></span>](#tab/npm)
<span data-ttu-id="6d20c-122">Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6d20c-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="6d20c-123">Para usar os módulos ES6, adicione o pacote npm ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="6d20c-123">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="6d20c-124">Agora você pode fazer referência a todos os componentes na página que está usando:</span><span class="sxs-lookup"><span data-stu-id="6d20c-124">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="6d20c-125">Pacotes NPM</span><span class="sxs-lookup"><span data-stu-id="6d20c-125">NPM packages</span></span>

<span data-ttu-id="6d20c-126">O microsoft Graph Toolkit é feito de vários pacotes NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="6d20c-126">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="6d20c-127"><b>@microsoft/mgt-element</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-127"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="6d20c-128">O `@microsoft/mgt-element` é o pacote principal que contém apenas as classes base usadas para criar componentes e provedores.</span><span class="sxs-lookup"><span data-stu-id="6d20c-128">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="6d20c-129">Este pacote expõe todas as classes e interfaces necessárias necessárias para criar seus próprios componentes e exporta a interface IProvider e a [classe SimpleProvider](../providers/custom.md) para a criação de provedores personalizados.</span><span class="sxs-lookup"><span data-stu-id="6d20c-129">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="6d20c-130"><b>@microsoft/mgt-components</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-130"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="6d20c-131">O `@microsoft/mgt-components` pacote contém todos os Graph Da Microsoft conectados, como , e muito `Person` `PeoplePicker` mais.</span><span class="sxs-lookup"><span data-stu-id="6d20c-131">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="6d20c-132">**Provedores**</span><span class="sxs-lookup"><span data-stu-id="6d20c-132">**Providers**</span></span>

<span data-ttu-id="6d20c-133">Os provedores estão disponíveis por meio de um único pacote e podem ser instalados conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="6d20c-133">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="6d20c-134">Os seguintes pacotes de provedor estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="6d20c-134">The following provider packages are available:</span></span>

- <span data-ttu-id="6d20c-135"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-135"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="6d20c-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` componente `mgt-msal-provider` e.</span><span class="sxs-lookup"><span data-stu-id="6d20c-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="6d20c-137">O provedor MSAL usa msal.js para autenticação em aplicativos Web e PWAs (Progressive Web Apps).</span><span class="sxs-lookup"><span data-stu-id="6d20c-137">The MSAL provider uses msal.js for authenticating in web apps and Progressive Web Apps (PWAs).</span></span>

- <span data-ttu-id="6d20c-138"><b>@micosoft/mgt-msal2-provider</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-138"><b>@micosoft/mgt-msal2-provider</b></span></span>

    <span data-ttu-id="6d20c-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contém o `Msal2Provider` componente `mgt-msal2-provider` e.</span><span class="sxs-lookup"><span data-stu-id="6d20c-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contains the `Msal2Provider` and `mgt-msal2-provider` component.</span></span> <span data-ttu-id="6d20c-140">O provedor MSAL usa o msal-browser para autenticação em aplicativos Web e PWAs.</span><span class="sxs-lookup"><span data-stu-id="6d20c-140">The MSAL provider uses msal-browser for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="6d20c-141"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-141"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="6d20c-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` componente `mgt-teams-provider` e.</span><span class="sxs-lookup"><span data-stu-id="6d20c-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="6d20c-143">O Microsoft Teams habilita a autenticação no Microsoft Teams guia.</span><span class="sxs-lookup"><span data-stu-id="6d20c-143">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="6d20c-144"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-144"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="6d20c-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)contém a `SharePointProvider` para autenticação em um SharePoint ambiente.</span><span class="sxs-lookup"><span data-stu-id="6d20c-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="6d20c-146"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-146"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="6d20c-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md)contém o `ProxyProvider` aplicativo para que o proxy Graph chamadas por meio de um serviço back-end.</span><span class="sxs-lookup"><span data-stu-id="6d20c-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="6d20c-148"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-148"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="6d20c-149">O é o pacote principal que inclui todos os pacotes acima e os reexporta para que eles sejam disponibilizados por meio de um `@microsoft/mgt` único pacote que você pode instalar.</span><span class="sxs-lookup"><span data-stu-id="6d20c-149">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="6d20c-150"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-150"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="6d20c-151">O pacote contém todos os componentes de React gerados automaticamente e tem [`@microsoft/mgt-react`](./mgt-react.md) dependência do `@microsoft/mgt` pacote.</span><span class="sxs-lookup"><span data-stu-id="6d20c-151">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

<span data-ttu-id="6d20c-152"><b>@microsoft/mgt-spfx</b></span><span class="sxs-lookup"><span data-stu-id="6d20c-152"><b>@microsoft/mgt-spfx</b></span></span>

<span data-ttu-id="6d20c-153">O pacote contém uma Estrutura do SharePoint que é necessária para usar o [`@microsoft/mgt-spfx`](./mgt-spfx.md) Microsoft Graph Toolkit em Estrutura do SharePoint soluções.</span><span class="sxs-lookup"><span data-stu-id="6d20c-153">The [`@microsoft/mgt-spfx`](./mgt-spfx.md) package contains a SharePoint Framework library that's required to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6d20c-154">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6d20c-154">Next Steps</span></span>
<span data-ttu-id="6d20c-155">Agora você está pronto para começar a desenvolver com o microsoft Graph Toolkit!</span><span class="sxs-lookup"><span data-stu-id="6d20c-155">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="6d20c-156">Os guias a seguir estão disponíveis para ajudá-lo a começar:</span><span class="sxs-lookup"><span data-stu-id="6d20c-156">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="6d20c-157">Registrar um aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="6d20c-157">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="6d20c-158">[Criar um aplicativo Web (JavaScript)](./build-a-web-app.md) (javascript de baunilha)</span><span class="sxs-lookup"><span data-stu-id="6d20c-158">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="6d20c-159">Criar um aplicativo web (React)</span><span class="sxs-lookup"><span data-stu-id="6d20c-159">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="6d20c-160">Criar um aplicativo web (Angular)</span><span class="sxs-lookup"><span data-stu-id="6d20c-160">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="6d20c-161">Criar uma web part do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6d20c-161">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="6d20c-162">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="6d20c-162">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
