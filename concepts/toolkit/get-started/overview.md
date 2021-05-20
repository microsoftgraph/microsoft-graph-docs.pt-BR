---
title: Começando com o Graph Toolkit da Microsoft
description: Comece a usar o Graph Toolkit microsoft em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e84350a7835cac7914f5238110f74b3383047e13
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579589"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="eddd6-103">Começando com o Graph Toolkit da Microsoft</span><span class="sxs-lookup"><span data-stu-id="eddd6-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="eddd6-104">Os componentes Graph Toolkit da Microsoft podem ser facilmente adicionados ao seu aplicativo web, SharePoint parte da Web ou Microsoft Teams guias.</span><span class="sxs-lookup"><span data-stu-id="eddd6-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="eddd6-105">Os componentes são baseados em padrões da Web e podem ser usados em projetos JavaScript simples ou com estruturas web populares, como Reach, Angular, Vue.js e muito mais.</span><span class="sxs-lookup"><span data-stu-id="eddd6-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="eddd6-106">Você pode assistir a este vídeo curto para ver como é rápido e fácil começar com o Toolkit.</span><span class="sxs-lookup"><span data-stu-id="eddd6-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="eddd6-107">Para um tutorial passo a passo, consulte o [módulo Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/).</span><span class="sxs-lookup"><span data-stu-id="eddd6-107">For a step-by-step tutorial, see the [Get started with Microsoft Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> 

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="eddd6-108">Configure o locatário do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="eddd6-108">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="eddd6-109">Para se desenvolver com o Toolkit, você precisa ter acesso a um inquilino Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="eddd6-109">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="eddd6-110">Se você não tiver uma, você pode obter uma assinatura gratuita de Microsoft 365 [desenvolvedores, aderindo ao programa de desenvolvedores Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="eddd6-110">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="eddd6-111">Para obter detalhes sobre como configurar sua assinatura, consulte [Configurar uma assinatura de desenvolvedor Microsoft 365](/office/developer-program/microsoft-365-developer-program-get-started).</span><span class="sxs-lookup"><span data-stu-id="eddd6-111">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="eddd6-112">Defina seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="eddd6-112">Set up your development environment</span></span>
<span data-ttu-id="eddd6-113">Para se desenvolver com o Toolkit, você precisará de um editor de texto ou IDE.</span><span class="sxs-lookup"><span data-stu-id="eddd6-113">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="eddd6-114">Você pode usar o editor ou IDE de sua escolha ou instalar e usar [Visual Studio Code](https://code.visualstudio.com/download) gratuitamente.</span><span class="sxs-lookup"><span data-stu-id="eddd6-114">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="eddd6-115">Você também precisará de um navegador moderno como Microsoft Edge, Google Chrome ou Firefox.</span><span class="sxs-lookup"><span data-stu-id="eddd6-115">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="eddd6-116">Você também precisará de uma versão LTS de Node.js, que você pode instalar a partir de [nodejs.org](https://nodejs.org).</span><span class="sxs-lookup"><span data-stu-id="eddd6-116">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="eddd6-117">Usando o Graph Toolkit da Microsoft</span><span class="sxs-lookup"><span data-stu-id="eddd6-117">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="eddd6-118">Você pode usar o Microsoft Graph Toolkit em seu aplicativo fazendo referência diretamente ao carregador (via unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="eddd6-118">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="eddd6-119">unpkg</span><span class="sxs-lookup"><span data-stu-id="eddd6-119">unpkg</span></span>](#tab/html)
<span data-ttu-id="eddd6-120">Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="eddd6-120">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="eddd6-121">npm</span><span class="sxs-lookup"><span data-stu-id="eddd6-121">npm</span></span>](#tab/npm)
<span data-ttu-id="eddd6-122">O uso do Toolkit através de módulos ES6 lhe dará controle total do processo de agrupamento e permitirá que você empacota apenas o código necessário para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eddd6-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="eddd6-123">Para usar os módulos ES6, adicione o pacote npm ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="eddd6-123">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="eddd6-124">Agora você pode referenciar todos os componentes da página que você está usando:</span><span class="sxs-lookup"><span data-stu-id="eddd6-124">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="eddd6-125">Pacotes NPM</span><span class="sxs-lookup"><span data-stu-id="eddd6-125">NPM packages</span></span>

<span data-ttu-id="eddd6-126">O Microsoft Graph Toolkit é composto por vários pacotes NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="eddd6-126">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="eddd6-127"><b>@microsoft/mgt-elemento</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-127"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="eddd6-128">O `@microsoft/mgt-element` pacote principal que contém apenas as classes base usadas para a construção de componentes e provedores.</span><span class="sxs-lookup"><span data-stu-id="eddd6-128">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="eddd6-129">Este pacote expõe todas as classes e interfaces necessárias para construir seus próprios componentes e exporta a [interface IProvider e a classe SimpleProvider](../providers/custom.md) para a construção de provedores personalizados.</span><span class="sxs-lookup"><span data-stu-id="eddd6-129">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="eddd6-130"><b>@microsoft/mgt-componentes</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-130"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="eddd6-131">O `@microsoft/mgt-components` pacote contém todos os componentes da Microsoft Graph conectados da Web, como , e muito `Person` `PeoplePicker` mais.</span><span class="sxs-lookup"><span data-stu-id="eddd6-131">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="eddd6-132">**Provedores**</span><span class="sxs-lookup"><span data-stu-id="eddd6-132">**Providers**</span></span>

<span data-ttu-id="eddd6-133">Os provedores estão disponíveis através de um único pacote e podem ser instalados conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="eddd6-133">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="eddd6-134">Os seguintes pacotes de provedores estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="eddd6-134">The following provider packages are available:</span></span>

- <span data-ttu-id="eddd6-135"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-135"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="eddd6-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` `mgt-msal-provider` componente e o componente.</span><span class="sxs-lookup"><span data-stu-id="eddd6-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="eddd6-137">O provedor MSAL usa msal.js para autenticar em aplicativos web e Aplicativos Web Progressivos (PWAs).</span><span class="sxs-lookup"><span data-stu-id="eddd6-137">The MSAL provider uses msal.js for authenticating in web apps and Progressive Web Apps (PWAs).</span></span>

- <span data-ttu-id="eddd6-138"><b>@micosoft/mgt-msal2-provider</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-138"><b>@micosoft/mgt-msal2-provider</b></span></span>

    <span data-ttu-id="eddd6-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contém o `Msal2Provider` `mgt-msal2-provider` componente e o componente.</span><span class="sxs-lookup"><span data-stu-id="eddd6-139">[`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contains the `Msal2Provider` and `mgt-msal2-provider` component.</span></span> <span data-ttu-id="eddd6-140">O provedor MSAL usa o navegador MSAL para autenticar em aplicativos web e PWAs.</span><span class="sxs-lookup"><span data-stu-id="eddd6-140">The MSAL provider uses msal-browser for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="eddd6-141"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-141"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="eddd6-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` `mgt-teams-provider` componente e o componente.</span><span class="sxs-lookup"><span data-stu-id="eddd6-142">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="eddd6-143">O provedor de Microsoft Teams permite a autenticação no aplicativo de guia Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="eddd6-143">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="eddd6-144"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-144"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="eddd6-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)contém o `SharePointProvider` para autenticar em um ambiente SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eddd6-145">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="eddd6-146"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-146"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="eddd6-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md)contém o `ProxyProvider` aplicativo para que o proxy Graph chamadas através de um serviço backend.</span><span class="sxs-lookup"><span data-stu-id="eddd6-147">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="eddd6-148"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-148"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="eddd6-149">O `@microsoft/mgt` pacote principal que inclui todos os pacotes acima e re-exporta-los para que eles estejam disponíveis através de um único pacote que você pode instalar.</span><span class="sxs-lookup"><span data-stu-id="eddd6-149">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="eddd6-150"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-150"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="eddd6-151">O [`@microsoft/mgt-react`](./mgt-react.md) pacote contém todos os componentes React gerados automaticamente e requer dependência do `@microsoft/mgt` pacote.</span><span class="sxs-lookup"><span data-stu-id="eddd6-151">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

<span data-ttu-id="eddd6-152"><b>@microsoft/mgt-spfx</b></span><span class="sxs-lookup"><span data-stu-id="eddd6-152"><b>@microsoft/mgt-spfx</b></span></span>

<span data-ttu-id="eddd6-153">O [`@microsoft/mgt-spfx`](./mgt-spfx.md) pacote contém uma biblioteca Estrutura do SharePoint necessária para usar o Microsoft Graph Toolkit em soluções Estrutura do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="eddd6-153">The [`@microsoft/mgt-spfx`](./mgt-spfx.md) package contains a SharePoint Framework library that's required to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

## <a name="polyfills"></a><span data-ttu-id="eddd6-154">Polifilis</span><span class="sxs-lookup"><span data-stu-id="eddd6-154">Polyfills</span></span>

<span data-ttu-id="eddd6-155">Se você estiver usando os módulos ES6 do pacote npm e estiver [mirando um navegador como o IE11](https://caniuse.com/#search=components) que não suporta componentes da Web nativamente, você precisará incluir polifildos em seu projeto, pois eles não estão automaticamente incluídos.</span><span class="sxs-lookup"><span data-stu-id="eddd6-155">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="eddd6-156">Os polyfills ajudam a preencher os recursos ausentes do navegador em navegadores que ainda estão em processo de atualização para suportar os padrões do Web Component.</span><span class="sxs-lookup"><span data-stu-id="eddd6-156">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support Web Component standards.</span></span> <span data-ttu-id="eddd6-157">Para obter instruções e saber mais, consulte [a documentação de polifilis](https://www.webcomponents.org/polyfills).</span><span class="sxs-lookup"><span data-stu-id="eddd6-157">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="eddd6-158">Os polifilis já estão incluídos se você estiver usando o Toolkit através do script mgt-loader.</span><span class="sxs-lookup"><span data-stu-id="eddd6-158">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="eddd6-159">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="eddd6-159">Next Steps</span></span>
<span data-ttu-id="eddd6-160">Agora você está pronto para começar a desenvolver com o microsoft Graph Toolkit!</span><span class="sxs-lookup"><span data-stu-id="eddd6-160">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="eddd6-161">Os seguintes guias estão disponíveis para ajudá-lo a começar:</span><span class="sxs-lookup"><span data-stu-id="eddd6-161">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="eddd6-162">Registrar um aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="eddd6-162">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="eddd6-163">[Construa um aplicativo web (JavaScript)](./build-a-web-app.md) (baunilha JavaScript)</span><span class="sxs-lookup"><span data-stu-id="eddd6-163">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="eddd6-164">Criar um aplicativo web (React)</span><span class="sxs-lookup"><span data-stu-id="eddd6-164">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="eddd6-165">Criar um aplicativo web (Angular)</span><span class="sxs-lookup"><span data-stu-id="eddd6-165">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="eddd6-166">Criar uma web part do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="eddd6-166">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="eddd6-167">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eddd6-167">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
