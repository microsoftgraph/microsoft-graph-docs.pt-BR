---
title: Iniciando o microsoft graph Toolkit
description: Começar a usar o microsoft graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 3197542066d92978bf151d61a378e7f392633016
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961419"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="71990-103">Iniciando o microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="71990-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="71990-104">Os componentes Toolkit do Microsoft Graph podem ser facilmente adicionados ao aplicativo Web, à Web Part do SharePoint ou às guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="71990-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="71990-105">Os componentes são baseados em padrões web e podem ser usados em projetos JavaScript simples ou com estruturas da Web populares, como Reach, Angular, Vue.js e muito mais.</span><span class="sxs-lookup"><span data-stu-id="71990-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="71990-106">Você pode assistir a este vídeo curto para ver como é rápido e fácil começar com o Toolkit.</span><span class="sxs-lookup"><span data-stu-id="71990-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="71990-107">Para obter um tutorial passo a passo, consulte o módulo Introdução ao [Microsot Graph Toolkit .](/learn/modules/msgraph-toolkit-intro/)</span><span class="sxs-lookup"><span data-stu-id="71990-107">For a step-by-step tutorial, see the [Get started with Microsot Graph Toolkit module](/learn/modules/msgraph-toolkit-intro/).</span></span> 

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="71990-108">Configure o locatário do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="71990-108">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="71990-109">Para desenvolver com o Toolkit, você precisa acessar um locatário do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="71990-109">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="71990-110">Se você não tiver um, poderá obter uma assinatura gratuita de desenvolvedor do Microsoft 365 ins juntando-se ao Programa de Desenvolvedores do [Microsoft 365.](https://developer.microsoft.com/microsoft-365/dev-program)</span><span class="sxs-lookup"><span data-stu-id="71990-110">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="71990-111">Para obter detalhes sobre como configurar sua assinatura, consulte Configurar uma assinatura de [desenvolvedor do Microsoft 365](/office/developer-program/microsoft-365-developer-program-get-started).</span><span class="sxs-lookup"><span data-stu-id="71990-111">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="71990-112">Defina seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="71990-112">Set up your development environment</span></span>
<span data-ttu-id="71990-113">Para desenvolver com o Toolkit, você precisará de um editor de texto ou IDE.</span><span class="sxs-lookup"><span data-stu-id="71990-113">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="71990-114">Você pode usar o editor ou o IDE de sua escolha ou instalar e usar [Visual Studio Código](https://code.visualstudio.com/download) gratuitamente.</span><span class="sxs-lookup"><span data-stu-id="71990-114">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="71990-115">Você também precisará de um navegador da Web moderno, como o Microsoft Edge, o Google Chrome ou o Firefox.</span><span class="sxs-lookup"><span data-stu-id="71990-115">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="71990-116">Você também precisará de uma versão LTS do Node.js, que pode ser instalada [nodejs.org](https://nodejs.org).</span><span class="sxs-lookup"><span data-stu-id="71990-116">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="71990-117">Usando o microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="71990-117">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="71990-118">Você pode usar o microsoft graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (por meio de unpkg) ou instalando o pacote npm.</span><span class="sxs-lookup"><span data-stu-id="71990-118">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="71990-119">unpkg</span><span class="sxs-lookup"><span data-stu-id="71990-119">unpkg</span></span>](#tab/html)
<span data-ttu-id="71990-120">Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="71990-120">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="71990-121">npm</span><span class="sxs-lookup"><span data-stu-id="71990-121">npm</span></span>](#tab/npm)
<span data-ttu-id="71990-122">Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71990-122">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="71990-123">Para usar os módulos ES6, adicione o pacote npm ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="71990-123">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="71990-124">Agora você pode fazer referência a todos os componentes na página que está usando:</span><span class="sxs-lookup"><span data-stu-id="71990-124">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="71990-125">Pacotes NPM</span><span class="sxs-lookup"><span data-stu-id="71990-125">NPM packages</span></span>

<span data-ttu-id="71990-126">O microsoft graph Toolkit é feito de vários pacotes NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="71990-126">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="71990-127"><b>@microsoft/mgt-element</b></span><span class="sxs-lookup"><span data-stu-id="71990-127"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="71990-128">O `@microsoft/mgt-element` é o pacote principal que contém apenas as classes base usadas para criar componentes e provedores.</span><span class="sxs-lookup"><span data-stu-id="71990-128">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="71990-129">Este pacote expõe todas as classes e interfaces necessárias necessárias para criar seus próprios componentes e exporta a interface IProvider e a [classe SimpleProvider](../providers/custom.md) para a criação de provedores personalizados.</span><span class="sxs-lookup"><span data-stu-id="71990-129">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="71990-130"><b>@microsoft/mgt-components</b></span><span class="sxs-lookup"><span data-stu-id="71990-130"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="71990-131">O `@microsoft/mgt-components` pacote contém todos os componentes web conectados do Microsoft Graph, como `Person` , e muito `PeoplePicker` mais.</span><span class="sxs-lookup"><span data-stu-id="71990-131">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="71990-132">**Provedores**</span><span class="sxs-lookup"><span data-stu-id="71990-132">**Providers**</span></span>

<span data-ttu-id="71990-133">Os provedores estão disponíveis por meio de um único pacote e podem ser instalados conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="71990-133">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="71990-134">Os seguintes pacotes de provedor estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="71990-134">The following provider packages are available:</span></span>

- <span data-ttu-id="71990-135"><b>@micosoft/mgt-msal-provider</b></span><span class="sxs-lookup"><span data-stu-id="71990-135"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="71990-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` componente `mgt-msal-provider` e.</span><span class="sxs-lookup"><span data-stu-id="71990-136">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="71990-137">O provedor msal aproveita o msal.js para autenticação em aplicativos Web e PWAs.</span><span class="sxs-lookup"><span data-stu-id="71990-137">The msal provider leverages msal.js for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="71990-138"><b>@microsoft/mgt-teams-provider</b></span><span class="sxs-lookup"><span data-stu-id="71990-138"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="71990-139">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` componente `mgt-teams-provider` e.</span><span class="sxs-lookup"><span data-stu-id="71990-139">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="71990-140">O provedor do Microsoft Teams habilita a autenticação no aplicativo de guia do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="71990-140">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="71990-141"><b>@microsoft/mgt-sharepoint-provider</b></span><span class="sxs-lookup"><span data-stu-id="71990-141"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="71990-142">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contém o `SharePointProvider` para autenticação em um ambiente do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="71990-142">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="71990-143"><b>@microsoft/mgt-proxy-provider</b></span><span class="sxs-lookup"><span data-stu-id="71990-143"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="71990-144">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contém o `ProxyProvider` aplicativo para o que o Proxy Graph chama por meio de um serviço de back-end.</span><span class="sxs-lookup"><span data-stu-id="71990-144">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="71990-145"><b>@microsoft/mgt</b></span><span class="sxs-lookup"><span data-stu-id="71990-145"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="71990-146">O é o pacote principal que inclui todos os pacotes acima e os reexporta para que eles sejam disponibilizados por meio de um `@microsoft/mgt` único pacote que você pode instalar.</span><span class="sxs-lookup"><span data-stu-id="71990-146">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="71990-147"><b>@microsoft/mgt-react</b></span><span class="sxs-lookup"><span data-stu-id="71990-147"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="71990-148">O pacote contém todos os componentes do React gerados automaticamente [`@microsoft/mgt-react`](./mgt-react.md) e tem dependência do `@microsoft/mgt` pacote.</span><span class="sxs-lookup"><span data-stu-id="71990-148">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

## <a name="polyfills"></a><span data-ttu-id="71990-149">Polyfills</span><span class="sxs-lookup"><span data-stu-id="71990-149">Polyfills</span></span>

<span data-ttu-id="71990-150">Se você estiver usando os módulos ES6 do pacote npm e estiver direcionando um navegador, como [o IE11,](https://caniuse.com/#search=components) que não dá suporte a componentes web de forma nativa, você precisará incluir polyfills em seu projeto, pois eles não são incluídos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="71990-150">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="71990-151">Polyfills ajudam a preencher os recursos ausentes do navegador em navegadores que ainda estão em processo de atualização para dar suporte aos padrões do Componente Web.</span><span class="sxs-lookup"><span data-stu-id="71990-151">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support Web Component standards.</span></span> <span data-ttu-id="71990-152">Para obter instruções e saber mais, consulte [polyfills documentation](https://www.webcomponents.org/polyfills).</span><span class="sxs-lookup"><span data-stu-id="71990-152">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="71990-153">Os polyfills já estão incluídos se você estiver usando o Toolkit por meio do script mgt-loader.</span><span class="sxs-lookup"><span data-stu-id="71990-153">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="71990-154">Próximas Etapas</span><span class="sxs-lookup"><span data-stu-id="71990-154">Next Steps</span></span>
<span data-ttu-id="71990-155">Agora você está pronto para começar a desenvolver com o microsoft graph Toolkit!</span><span class="sxs-lookup"><span data-stu-id="71990-155">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="71990-156">Os guias a seguir estão disponíveis para ajudá-lo a começar:</span><span class="sxs-lookup"><span data-stu-id="71990-156">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="71990-157">Registrar um aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="71990-157">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="71990-158">[Criar um aplicativo Web (JavaScript)](./build-a-web-app.md) (javascript de baunilha)</span><span class="sxs-lookup"><span data-stu-id="71990-158">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="71990-159">Criar um aplicativo web (React)</span><span class="sxs-lookup"><span data-stu-id="71990-159">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="71990-160">Criar um aplicativo web (Angular)</span><span class="sxs-lookup"><span data-stu-id="71990-160">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="71990-161">Criar uma web part do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="71990-161">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="71990-162">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="71990-162">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
