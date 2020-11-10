---
title: Introdução ao Microsoft Graph Toolkit
description: Introdução ao uso do Microsoft Graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e3739bb6180e19569ae40e873d3a018bbb541833
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977132"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="d0a2b-103">Introdução ao Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d0a2b-103">Getting started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d0a2b-104">Os componentes do Microsoft Graph Toolkit podem ser adicionados facilmente ao aplicativo Web, à Web Part do SharePoint ou às guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-104">The Microsoft Graph Toolkit components can easily be added to your web application, SharePoint web part, or Microsoft Teams tabs.</span></span> <span data-ttu-id="d0a2b-105">Os componentes são baseados em padrões da Web e podem ser usados em projetos de JavaScript simples ou com estruturas da Web populares, como REACH, angular, Vue.js e muito mais.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-105">The components are based on web standards and can be used in both plain JavaScript projects or with popular web frameworks such as Reach, Angular, Vue.js, and more.</span></span>

<span data-ttu-id="d0a2b-106">Você pode assistir a esse pequeno vídeo para ver como é rápido e fácil começar a usar o kit de ferramentas.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-106">You can watch this short video to see how quick and easy it is to get started with the Toolkit.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a><span data-ttu-id="d0a2b-107">Configurar seu locatário do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d0a2b-107">Set up your Microsoft 365 tenant</span></span>
<span data-ttu-id="d0a2b-108">Para desenvolver com o kit de ferramentas, você precisa acessar um Microsoft 365 locatário.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-108">In order to develop with the Toolkit, you need access to a Microsoft 365 tenant.</span></span> <span data-ttu-id="d0a2b-109">Se você não tiver um, poderá obter uma assinatura gratuita do desenvolvedor do Microsoft 365, [participando do programa de desenvolvedor do microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).</span><span class="sxs-lookup"><span data-stu-id="d0a2b-109">If you don't have one, you can get a free Microsoft 365 developer subscription by [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program).</span></span> <span data-ttu-id="d0a2b-110">Para obter detalhes sobre como configurar sua assinatura, consulte [set up a Microsoft 365 Developer Subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span><span class="sxs-lookup"><span data-stu-id="d0a2b-110">For details about how to configure your subscription, see [Set up a Microsoft 365 developer subscription](/office/developer-program/microsoft-365-developer-program-get-started).</span></span>

## <a name="set-up-your-development-environment"></a><span data-ttu-id="d0a2b-111">Defina seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="d0a2b-111">Set up your development environment</span></span>
<span data-ttu-id="d0a2b-112">Para desenvolver com o kit de ferramentas, você precisará de um editor de texto ou IDE.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-112">To develop with the Toolkit, you will need a text editor or IDE.</span></span> <span data-ttu-id="d0a2b-113">Você pode usar o editor ou o IDE de sua escolha ou instalar e usar o [Visual Studio Code](https://code.visualstudio.com/download) gratuitamente.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-113">You can use the editor or IDE of your choice or install and use [Visual Studio Code](https://code.visualstudio.com/download) for free.</span></span> <span data-ttu-id="d0a2b-114">Você também precisará de um navegador da Web moderno, como o Microsoft Edge, Google Chrome ou Firefox.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-114">You will also need a modern web browser like Microsoft Edge, Google Chrome, or Firefox.</span></span> <span data-ttu-id="d0a2b-115">Você também precisará de uma versão do LTS do Node.js, que pode ser instalada no [NodeJS.org](https://nodejs.org).</span><span class="sxs-lookup"><span data-stu-id="d0a2b-115">You'll also need an LTS version of Node.js, which you can install from [nodejs.org](https://nodejs.org).</span></span>

## <a name="using-the-microsoft-graph-toolkit"></a><span data-ttu-id="d0a2b-116">Usando o kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d0a2b-116">Using the Microsoft Graph Toolkit</span></span>
<span data-ttu-id="d0a2b-117">Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote NPM.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-117">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg) or by installing the npm package.</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="d0a2b-118">Usar via gerenciamento-carregador</span><span class="sxs-lookup"><span data-stu-id="d0a2b-118">Use via mgt-loader</span></span>
<span data-ttu-id="d0a2b-119">Para usar o kit de ferramentas via gerenciamento-Loader, adicione a referência em um script ao seu código:</span><span class="sxs-lookup"><span data-stu-id="d0a2b-119">To use the Toolkit via mgt-loader, add the reference in a script to your code:</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="d0a2b-120">Usar via NPM (módulos ES6)</span><span class="sxs-lookup"><span data-stu-id="d0a2b-120">Use via npm (ES6 modules)</span></span>
<span data-ttu-id="d0a2b-121">O uso do kit de ferramentas por meio de módulos ES6 fornecerá controle total do processo de agrupamento e permitirá que você reúna apenas o código necessário para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-121">Using the Toolkit via ES6 modules will give you full control of the bundling process and allow you to bundle only the code you need for your application.</span></span> <span data-ttu-id="d0a2b-122">Para usar os módulos ES6, adicione o pacote NPM ao seu projeto:</span><span class="sxs-lookup"><span data-stu-id="d0a2b-122">To use the ES6 modules, add the npm package to your project:</span></span>

```bash
npm install @microsoft/mgt
```
<span data-ttu-id="d0a2b-123">Agora, você pode fazer referência a todos os componentes na página que você está usando:</span><span class="sxs-lookup"><span data-stu-id="d0a2b-123">Now you can reference all the components in the page you're using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="d0a2b-124">Ou, apenas faça referência ao componente de que você precisa e Evite carregar tudo o mais:</span><span class="sxs-lookup"><span data-stu-id="d0a2b-124">Or, just reference the component you need and avoid loading everything else:</span></span>
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

#### <a name="polyfills"></a><span data-ttu-id="d0a2b-125">Polyfills</span><span class="sxs-lookup"><span data-stu-id="d0a2b-125">Polyfills</span></span>

<span data-ttu-id="d0a2b-126">Se você estiver usando os módulos ES6 do pacote do NPM e estiver [direcionando um navegador como o IE11](https://caniuse.com/#search=components) que não ofereça suporte a componentes Web nativamente, será necessário incluir os metapreenchimentos no seu projeto, pois eles não serão incluídos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-126">If you're using the ES6 modules from the npm package and you're [targeting a browser such as IE11](https://caniuse.com/#search=components) that does not support web components natively, you will need to include polyfills in your project, as they are not automatically included.</span></span> <span data-ttu-id="d0a2b-127">Os metapreenchimentos ajudam a preencher os recursos de navegador ausentes em navegadores que ainda estejam no processo de atualização para suportar os padrões do webcComponent.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-127">Polyfills help to fill in missing browser capabilities in browsers that are still in the process of updating to support webcComponent standards.</span></span> <span data-ttu-id="d0a2b-128">Para obter instruções e saber mais, confira [documentação dos metaabastecimentos](https://www.webcomponents.org/polyfills).</span><span class="sxs-lookup"><span data-stu-id="d0a2b-128">For instructions and to learn more, see [polyfills documentation](https://www.webcomponents.org/polyfills).</span></span> 

<span data-ttu-id="d0a2b-129">Os metapreenchimentos já estão incluídos se você estiver usando o kit de ferramentas através do script de gerenciamento de Complementos.</span><span class="sxs-lookup"><span data-stu-id="d0a2b-129">The polyfills are already included if you're using the Toolkit via the mgt-loader script.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0a2b-130">Próximas Etapas</span><span class="sxs-lookup"><span data-stu-id="d0a2b-130">Next Steps</span></span>
<span data-ttu-id="d0a2b-131">Agora você está pronto para começar a desenvolver com o Microsoft Graph Toolkit!</span><span class="sxs-lookup"><span data-stu-id="d0a2b-131">You're now ready to start developing with the Microsoft Graph Toolkit!</span></span> <span data-ttu-id="d0a2b-132">Os seguintes guias estão disponíveis para ajudá-lo a começar:</span><span class="sxs-lookup"><span data-stu-id="d0a2b-132">The following guides are available to help you get started:</span></span>

- [<span data-ttu-id="d0a2b-133">Criar um aplicativo do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="d0a2b-133">Create an Azure Active Directory app</span></span>](./add-aad-app-registration.md)
- <span data-ttu-id="d0a2b-134">[Criar um aplicativo Web](./build-a-web-app.md) (JavaScript de baunilha)</span><span class="sxs-lookup"><span data-stu-id="d0a2b-134">[Build a web application](./build-a-web-app.md) (vanilla JavaScript)</span></span>
- [<span data-ttu-id="d0a2b-135">Criar uma web part do Microsoft Office SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="d0a2b-135">Build a SharePoint web part</span></span>](./build-a-sharepoint-web-part.md)
- [<span data-ttu-id="d0a2b-136">Criar uma guia do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d0a2b-136">Build a Microsoft Teams tab</span></span>](./build-a-microsoft-teams-tab.md)
- [<span data-ttu-id="d0a2b-137">Usar o kit de ferramentas reagir</span><span class="sxs-lookup"><span data-stu-id="d0a2b-137">Use the Toolkit with React</span></span>](./use-toolkit-with-react.md)
- [<span data-ttu-id="d0a2b-138">Usar o kit de ferramentas com angular</span><span class="sxs-lookup"><span data-stu-id="d0a2b-138">Use the Toolkit with Angular</span></span>](./use-toolkit-with-angular.md)
