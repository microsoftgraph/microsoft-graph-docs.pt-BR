---
title: Introdução ao Microsoft Graph Toolkit
description: Introdução ao uso do Microsoft Graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: f1451213822e2489f04bb454c355125ed95b1aed
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664125"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="3f639-103">Introdução ao Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="3f639-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3f639-104">Os componentes do Microsoft Graph Toolkit podem ser adicionados facilmente ao aplicativo Web, à Web Part do SharePoint ou às guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3f639-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="3f639-105">Os componentes são baseados em padrões da Web e podem ser usados em projetos de JavaScript simples ou com estruturas da Web populares, como REACH, angular, Vue.js e muito mais.</span><span class="sxs-lookup"><span data-stu-id="3f639-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="3f639-106">Você pode assistir a esse pequeno vídeo para ver como é rápido e fácil começar a usar o kit de ferramentas.</span><span class="sxs-lookup"><span data-stu-id="3f639-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="3f639-107">Configurar seu locatário do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3f639-107">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="3f639-108">Para desenvolver com o kit de ferramentas, você precisa acessar um Microsoft 365 locatário.</span><span class="sxs-lookup"><span data-stu-id="3f639-108">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="3f639-109">Se você não tiver um, poderá obter uma assinatura gratuita do desenvolvedor do Microsoft 365, [participando do programa de desenvolvedor do microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="3f639-109">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="3f639-110">Para obter detalhes sobre como configurar sua assinatura, consulte [set up a Microsoft 365 Developer Subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span><span class="sxs-lookup"><span data-stu-id="3f639-110">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="3f639-111">Defina seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="3f639-111">Set up your development environment</span></span>
<span data-ttu-id="3f639-112">Para desenvolver com o kit de ferramentas, você precisará de um editor de texto ou IDE.</span><span class="sxs-lookup"><span data-stu-id="3f639-112">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="3f639-113">Você pode usar o editor ou o IDE de sua escolha ou instalar e usar o [Visual Studio Code](https://code.visualstudio.com/download) gratuitamente.</span><span class="sxs-lookup"><span data-stu-id="3f639-113">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="3f639-114">Você também precisará de um navegador da Web moderno, como o Microsoft Edge, Google Chrome ou Firefox.</span><span class="sxs-lookup"><span data-stu-id="3f639-114">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="3f639-115">Você também precisará de uma versão do LTS do Node.js, que pode ser instalada no [NodeJS.org](https://nodejs.org).</span><span class="sxs-lookup"><span data-stu-id="3f639-115">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="3f639-116">Usando o kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3f639-116">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="3f639-117">Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote NPM.</span><span class="sxs-lookup"><span data-stu-id="3f639-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

# <a name="unpkg"></a>[<span data-ttu-id="3f639-118">unpkg</span><span class="sxs-lookup"><span data-stu-id="3f639-118">unpkg</span></span>](#tab/html)
<span data-ttu-id="3f639-119">Para usar o kit de ferramentas via gerenciamento-Loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="3f639-119">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[<span data-ttu-id="3f639-120">npm</span><span class="sxs-lookup"><span data-stu-id="3f639-120">npm</span></span>](#tab/npm)
<span data-ttu-id="3f639-121">O uso do kit de ferramentas por meio de módulos ES6 fornecerá controle total do processo de agrupamento e permitirá que você reúna apenas o código necessário para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3f639-121">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="3f639-122">Para usar os módulos ES6, adicione o pacote NPM ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="3f639-122">To use the ES6 modules, add the npm package to your project:</span></span>

```cmd
npm install @microsoft/mgt
```
<span data-ttu-id="3f639-123">Agora, você pode fazer referência a todos os componentes na página que você está usando:</span><span class="sxs-lookup"><span data-stu-id="3f639-123">Now you can reference all the components in the page you're using:</span></span>

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a><span data-ttu-id="3f639-124">Pacotes NPM</span><span class="sxs-lookup"><span data-stu-id="3f639-124">NPM packages</span></span>

<span data-ttu-id="3f639-125">O Microsoft Graph Toolkit é composto por vários pacotes do NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3f639-125">The Microsoft Graph Toolkit is made up of several NPM packages, allowing you to only include the code you need for your applications.</span></span>

<span data-ttu-id="3f639-126"><b>@microsoft/MGT-Element</b></span><span class="sxs-lookup"><span data-stu-id="3f639-126"><b>@microsoft/mgt-element</b></span></span>

<span data-ttu-id="3f639-127">O `@microsoft/mgt-element` é o pacote principal que contém apenas as classes base usadas para criar componentes e provedores.</span><span class="sxs-lookup"><span data-stu-id="3f639-127">The `@microsoft/mgt-element` is the core package that contains only the base classes used for building components and providers.</span></span> <span data-ttu-id="3f639-128">Este pacote expõe todas as classes e interfaces necessárias para criar seus próprios componentes e exporta a [interface IProvider e a classe simpleprovider](../providers/custom.md) para a criação de provedores personalizados.</span><span class="sxs-lookup"><span data-stu-id="3f639-128">This package exposes all  necessary classes and interfaces needed to build your own components and exports the [IProvider interface and SimpleProvider class](../providers/custom.md) for building custom providers.</span></span>

<span data-ttu-id="3f639-129"><b>@microsoft/MGT-Components</b></span><span class="sxs-lookup"><span data-stu-id="3f639-129"><b>@microsoft/mgt-components</b></span></span>

<span data-ttu-id="3f639-130">O `@microsoft/mgt-components` pacote contém todos os componentes da Web conectados ao Microsoft Graph, como `Person` , `PeoplePicker` e mais.</span><span class="sxs-lookup"><span data-stu-id="3f639-130">The `@microsoft/mgt-components` package contains all Microsoft Graph connected web components, such as `Person`, `PeoplePicker`, and more.</span></span> 

<span data-ttu-id="3f639-131">**Provedores**</span><span class="sxs-lookup"><span data-stu-id="3f639-131">**Providers**</span></span>

<span data-ttu-id="3f639-132">Os provedores estão disponíveis por meio de um único pacote e podem ser instalados conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="3f639-132">Providers are available via a single package and can be installed as needed.</span></span> <span data-ttu-id="3f639-133">Os seguintes pacotes de provedor estão disponíveis:</span><span class="sxs-lookup"><span data-stu-id="3f639-133">The following provider packages are available:</span></span>

- <span data-ttu-id="3f639-134"><b>@micosoft/MGT-MSAL-Provider</b></span><span class="sxs-lookup"><span data-stu-id="3f639-134"><b>@micosoft/mgt-msal-provider</b></span></span>

    <span data-ttu-id="3f639-135">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` `mgt-msal-provider` componente e.</span><span class="sxs-lookup"><span data-stu-id="3f639-135">[`@micosoft/mgt-msal-provider`](../providers/msal.md) contains the `MsalProvider` and `mgt-msal-provider` component.</span></span> <span data-ttu-id="3f639-136">O provedor MSAL utiliza msal.js para autenticação em aplicativos Web e PWAs.</span><span class="sxs-lookup"><span data-stu-id="3f639-136">The msal provider leverages msal.js for authenticating in web apps and PWAs.</span></span>

-  <span data-ttu-id="3f639-137"><b>@microsoft/MGT-Teams-Provider</b></span><span class="sxs-lookup"><span data-stu-id="3f639-137"><b>@microsoft/mgt-teams-provider</b></span></span>

    <span data-ttu-id="3f639-138">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` `mgt-teams-provider` componente e.</span><span class="sxs-lookup"><span data-stu-id="3f639-138">[`@microsoft/mgt-teams-provider`](../providers/teams.md) contains the `TeamsProvider` and `mgt-teams-provider` component.</span></span> <span data-ttu-id="3f639-139">O provedor do Microsoft Teams habilita a autenticação no aplicativo de guia do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3f639-139">The Microsoft Teams provider enables authentication in Microsoft Teams tab application.</span></span>

- <span data-ttu-id="3f639-140"><b>@microsoft/MGT-SharePoint-Provider</b></span><span class="sxs-lookup"><span data-stu-id="3f639-140"><b>@microsoft/mgt-sharepoint-provider</b></span></span>

    <span data-ttu-id="3f639-141">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contém o `SharePointProvider` para autenticação em um ambiente do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3f639-141">[`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contains the `SharePointProvider` for authenticating in a SharePoint environment.</span></span> 

- <span data-ttu-id="3f639-142"><b>@microsoft/MGT-proxy-Provider</b></span><span class="sxs-lookup"><span data-stu-id="3f639-142"><b>@microsoft/mgt-proxy-provider</b></span></span>

    <span data-ttu-id="3f639-143">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contém o `ProxyProvider` aplicativo para o qual o proxy Graph chama por meio de um serviço de back-end.</span><span class="sxs-lookup"><span data-stu-id="3f639-143">[`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contains the `ProxyProvider` for application that proxy Graph calls through a backend service.</span></span> 

<span data-ttu-id="3f639-144"><b>@microsoft/MGT</b></span><span class="sxs-lookup"><span data-stu-id="3f639-144"><b>@microsoft/mgt</b></span></span>

<span data-ttu-id="3f639-145">O `@microsoft/mgt` é o pacote principal que inclui todos os pacotes acima e os exporta novamente para que estejam disponíveis por meio de um único pacote que você possa instalar.</span><span class="sxs-lookup"><span data-stu-id="3f639-145">The `@microsoft/mgt` is the main package that includes all above packages and re-exports them so they are available via a single package you can install.</span></span> 

<span data-ttu-id="3f639-146"><b>@microsoft/MGT-React</b></span><span class="sxs-lookup"><span data-stu-id="3f639-146"><b>@microsoft/mgt-react</b></span></span>

<span data-ttu-id="3f639-147">O [`@microsoft/mgt-react`](./mgt-react.md) pacote contém todos os componentes de reagir gerados automaticamente e assume a dependência do `@microsoft/mgt` pacote.</span><span class="sxs-lookup"><span data-stu-id="3f639-147">The [`@microsoft/mgt-react`](./mgt-react.md) package contains all auto-generated React components and takes dependency on the `@microsoft/mgt` package.</span></span>

## <a name="polyfills"></a><span data-ttu-id="3f639-148">Polyfills</span><span class="sxs-lookup"><span data-stu-id="3f639-148">Polyfills</span></span>

<span data-ttu-id="3f639-149">Se você estiver usando os módulos ES6 do pacote do NPM e estiver [direcionando um navegador como o IE11](https://caniuse.com/#search=components) que não ofereça suporte a componentes Web nativamente, será necessário incluir os metapreenchimentos no seu projeto, pois eles não serão incluídos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3f639-149">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="3f639-150">Os metapreenchimentos ajudam a preencher os recursos de navegador ausentes em navegadores que ainda estejam no processo de atualização para suporte aos padrões de componente da Web.</span><span class="sxs-lookup"><span data-stu-id="3f639-150">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support Web Component standards.</span></span> <span data-ttu-id="3f639-151">Para obter instruções e saber mais, confira [documentação dos metaabastecimentos](https://www.webcomponents.org/polyfills).</span><span class="sxs-lookup"><span data-stu-id="3f639-151">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="3f639-152">Os metapreenchimentos já estão incluídos se você estiver usando o kit de ferramentas através do script de gerenciamento de Complementos.</span><span class="sxs-lookup"><span data-stu-id="3f639-152">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3f639-153">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3f639-153">Next Steps</span></span>
<span data-ttu-id="3f639-154">Agora você está pronto para começar a desenvolver com o Microsoft Graph Toolkit!</span><span class="sxs-lookup"><span data-stu-id="3f639-154">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="3f639-155">Os seguintes guias estão disponíveis para ajudá-lo a começar:</span><span class="sxs-lookup"><span data-stu-id="3f639-155">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="3f639-156">Registrar um aplicativo no Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="3f639-156">Register an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="3f639-157">[Criar um aplicativo Web (JavaScript)](./build-a-web-app.md) (JavaScript de baunilha)</span><span class="sxs-lookup"><span data-stu-id="3f639-157">[Build a web app (JavaScript)](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="3f639-158">Criar um aplicativo web (React)</span><span class="sxs-lookup"><span data-stu-id="3f639-158">Build a web app (React)</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="3f639-159">Criar um aplicativo web (Angular)</span><span class="sxs-lookup"><span data-stu-id="3f639-159">Build a web app (Angular)</span></span>](./use-toolkit-with-angular.md)
- [<span data-ttu-id="3f639-160">Criar uma web part do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3f639-160">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="3f639-161">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3f639-161">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
