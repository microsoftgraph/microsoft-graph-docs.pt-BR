---
title: Iniciando o microsoft Graph Toolkit
description: Começar a usar o microsoft Graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e84350a7835cac7914f5238110f74b3383047e13
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579589"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="bf259-103">Iniciando o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bf259-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bf259-104">Os componentes Graph Toolkit microsoft podem ser facilmente adicionados ao seu aplicativo Web, SharePoint Web Part ou Microsoft Teams guias.</span><span class="sxs-lookup"><span data-stu-id="bf259-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="bf259-105">Os componentes são baseados em padrões web e podem ser usados em projetos JavaScript simples ou com estruturas da Web populares, como Reach, Angular, Vue.js e muito mais.</span><span class="sxs-lookup"><span data-stu-id="bf259-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="bf259-106">Você pode assistir a este vídeo curto para ver como é rápido e fácil começar com o Toolkit.</span><span class="sxs-lookup"><span data-stu-id="bf259-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="bf259-107">Para obter um tutorial passo a passo, consulte o [módulo Introdução ao microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/).</span><span class="sxs-lookup"><span data-stu-id="bf259-107">For a step-by-step tutorial, see the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> 

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="bf259-108">Configure o locatário do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bf259-108">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="bf259-109">Para desenvolver com o Toolkit, você precisa de acesso a um locatário Microsoft 365 locatário.</span><span class="sxs-lookup"><span data-stu-id="bf259-109">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="bf259-110">Se você não tiver um, poderá obter uma assinatura de desenvolvedor gratuita Microsoft 365 in [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="bf259-110">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="bf259-111">Para obter detalhes sobre como configurar sua assinatura, consulte [Configurar uma assinatura Microsoft 365 desenvolvedor.](/office/developer-program/microsoft-365-developer-program-get-started)</span><span class="sxs-lookup"><span data-stu-id="bf259-111">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="bf259-112">Defina seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="bf259-112">Set up your development environment</span></span>
<span data-ttu-id="bf259-113">Para desenvolver com o Toolkit, você precisará de um editor de texto ou IDE.</span><span class="sxs-lookup"><span data-stu-id="bf259-113">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="bf259-114">Você pode usar o editor ou o IDE de sua escolha ou instalar e [usar](https://code.visualstudio.com/download) Visual Studio Code gratuitamente.</span><span class="sxs-lookup"><span data-stu-id="bf259-114">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="bf259-115">Você também precisará de um navegador da Web moderno como Microsoft Edge, Google Chrome ou Firefox.</span><span class="sxs-lookup"><span data-stu-id="bf259-115">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="bf259-116">Você também precisará de uma versão LTS do Node.js, que pode ser instalada [nodejs.org](https://nodejs.org).</span><span class="sxs-lookup"><span data-stu-id="bf259-116">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="bf259-117">Usando o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bf259-117">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="bf259-118">Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="bf259-118">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="bf259-119">unpkg</span><span class="sxs-lookup"><span data-stu-id="bf259-119">unpkg</span></span>](#tab/html)
<span data-ttu-id="bf259-120">Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="bf259-120">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="bf259-121">npm</span><span class="sxs-lookup"><span data-stu-id="bf259-121">npm</span></span>](#tab/npm)
<span data-ttu-id="bf259-122">Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf259-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="bf259-123">Para usar os módulos ES6, adicione o pacote npm ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="bf259-123">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="bf259-124">Agora você pode fazer referência a todos os componentes na página que está usando:</span><span class="sxs-lookup"><span data-stu-id="bf259-124">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="bf259-125">Pacotes NPM</span><span class="sxs-lookup"><span data-stu-id="bf259-125">NPM packages</span></span>

<span data-ttu-id="bf259-126">O microsoft Graph Toolkit é feito de vários pacotes NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bf259-126">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="bf259-127"><b>@microsoft/mgt-element</b></span><span class="sxs-lookup"><span data-stu-id="bf259-127"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="bf259-128">O `@microsoft/mgt-element` é o pacote principal que contém apenas as classes base usadas para criar componentes e provedores.</span><span class="sxs-lookup"><span data-stu-id="bf259-128">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="bf259-129">Este pacote expõe todas as classes e interfaces necessárias necessárias para criar seus próprios componentes e exporta a interface IProvider e a [classe SimpleProvider](../providers/custom.md) para a criação de provedores personalizados.</span><span class="sxs-lookup"><span data-stu-id="bf259-129">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="bf259-130"><b>@microsoft/mgt-components</b></span><span class="sxs-lookup"><span data-stu-id="bf259-130"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="bf259-131">O `@microsoft/mgt-components` pacote contém todos os Graph Da Microsoft conectados, como , e muito `Person` `PeoplePicker` mais.</span><span class="sxs-lookup"><span data-stu-id="bf259-131">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="bf259-132">**Provedores**</span><span class="sxs-lookup"><span data-stu-id="bf259-132">**Providers**</span></span>

<span data-ttu-id="bf259-133">Os provedores estão disponíveis por meio de um único pacote e podem ser instalados conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="bf259-133">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="bf259-134">Os seguintes pacotes de provedor estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="bf259-134">The following provider packages are available:</span></span>

- <span data-ttu-id="bf259-135"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="bf259-135"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="bf259-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` componente `mgt-msal-provider` e.</span><span class="sxs-lookup"><span data-stu-id="bf259-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="bf259-137">O provedor MSAL usa msal.js para autenticação em aplicativos Web e PWAs (Progressive Web Apps).</span><span class="sxs-lookup"><span data-stu-id="bf259-137">The MSAL provider uses msal.js for authenticating in web apps and Progressive Web Apps (PWAs).</span></span>

- <span data-ttu-id="bf259-138"><b>@micosoft/mgt-msal2-provider</b></span><span class="sxs-lookup"><span data-stu-id="bf259-138"><b>@micosoft/mgt-msal2-provider</b></span></span>

    <span data-ttu-id="bf259-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contém o `Msal2Provider` componente `mgt-msal2-provider` e.</span><span class="sxs-lookup"><span data-stu-id="bf259-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contains the `Msal2Provider` and `mgt-msal2-provider` component.</span></span> <span data-ttu-id="bf259-140">O provedor MSAL usa o msal-browser para autenticação em aplicativos Web e PWAs.</span><span class="sxs-lookup"><span data-stu-id="bf259-140">The MSAL provider uses msal-browser for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="bf259-141"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="bf259-141"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="bf259-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` componente `mgt-teams-provider` e.</span><span class="sxs-lookup"><span data-stu-id="bf259-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="bf259-143">O Microsoft Teams habilita a autenticação no Microsoft Teams guia.</span><span class="sxs-lookup"><span data-stu-id="bf259-143">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="bf259-144"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="bf259-144"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="bf259-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)contém a `SharePointProvider` para autenticação em um SharePoint ambiente.</span><span class="sxs-lookup"><span data-stu-id="bf259-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="bf259-146"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="bf259-146"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="bf259-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md)contém o `ProxyProvider` aplicativo para que o proxy Graph chamadas por meio de um serviço back-end.</span><span class="sxs-lookup"><span data-stu-id="bf259-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="bf259-148"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="bf259-148"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="bf259-149">O é o pacote principal que inclui todos os pacotes acima e os reexporta para que eles sejam disponibilizados por meio de um `@microsoft/mgt` único pacote que você pode instalar.</span><span class="sxs-lookup"><span data-stu-id="bf259-149">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="bf259-150"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="bf259-150"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="bf259-151">O pacote contém todos os componentes de React gerados automaticamente e tem [`@microsoft/mgt-react`](./mgt-react.md) dependência do `@microsoft/mgt` pacote.</span><span class="sxs-lookup"><span data-stu-id="bf259-151">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

<span data-ttu-id="bf259-152"><b>@microsoft/mgt-spfx</b></span><span class="sxs-lookup"><span data-stu-id="bf259-152"><b>@microsoft/mgt-spfx</b></span></span>

<span data-ttu-id="bf259-153">O pacote contém uma Estrutura do SharePoint que é necessária para usar o [`@microsoft/mgt-spfx`](./mgt-spfx.md) Microsoft Graph Toolkit em Estrutura do SharePoint soluções.</span><span class="sxs-lookup"><span data-stu-id="bf259-153">The [`@microsoft/mgt-spfx`](./mgt-spfx.md) package contains a SharePoint Framework library that's required to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

## <a name="polyfills"></a><span data-ttu-id="bf259-154">Polyfills</span><span class="sxs-lookup"><span data-stu-id="bf259-154">Polyfills</span></span>

<span data-ttu-id="bf259-155">Se você estiver usando os módulos ES6 do pacote npm e estiver direcionando um navegador, como [o IE11,](https://caniuse.com/#search=components) que não dá suporte a componentes web de forma nativa, você precisará incluir polyfills em seu projeto, pois eles não são incluídos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="bf259-155">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="bf259-156">Polyfills ajudam a preencher os recursos ausentes do navegador em navegadores que ainda estão em processo de atualização para dar suporte aos padrões do Componente Web.</span><span class="sxs-lookup"><span data-stu-id="bf259-156">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support Web Component standards.</span></span> <span data-ttu-id="bf259-157">Para obter instruções e saber mais, consulte [polyfills documentation](https://www.webcomponents.org/polyfills).</span><span class="sxs-lookup"><span data-stu-id="bf259-157">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="bf259-158">Os polyfills já estão incluídos se você estiver usando o Toolkit por meio do script mgt-loader.</span><span class="sxs-lookup"><span data-stu-id="bf259-158">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bf259-159">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="bf259-159">Next Steps</span></span>
<span data-ttu-id="bf259-160">Agora você está pronto para começar a desenvolver com o microsoft Graph Toolkit!</span><span class="sxs-lookup"><span data-stu-id="bf259-160">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="bf259-161">Os guias a seguir estão disponíveis para ajudá-lo a começar:</span><span class="sxs-lookup"><span data-stu-id="bf259-161">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="bf259-162">Registrar um aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="bf259-162">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="bf259-163">[Criar um aplicativo Web (JavaScript)](./build-a-web-app.md) (javascript de baunilha)</span><span class="sxs-lookup"><span data-stu-id="bf259-163">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="bf259-164">Criar um aplicativo web (React)</span><span class="sxs-lookup"><span data-stu-id="bf259-164">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="bf259-165">Criar um aplicativo web (Angular)</span><span class="sxs-lookup"><span data-stu-id="bf259-165">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="bf259-166">Criar uma web part do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bf259-166">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="bf259-167">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="bf259-167">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
