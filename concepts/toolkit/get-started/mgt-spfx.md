---
title: Estrutura do SharePoint biblioteca do Microsoft Graph Toolkit
description: Use a Estrutura do SharePoint do Microsoft Graph Toolkit para usar o Microsoft Graph Toolkit em Estrutura do SharePoint soluções.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 5868f9fd523055d50f985f2fc8c8840563d56b28
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629487"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a><span data-ttu-id="110ed-103">Estrutura do SharePoint biblioteca do Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="110ed-103">SharePoint Framework library for Microsoft Graph Toolkit</span></span>

<span data-ttu-id="110ed-104">Use a Estrutura do SharePoint do Microsoft Graph Toolkit para usar o Microsoft Graph Toolkit em Estrutura do SharePoint soluções.</span><span class="sxs-lookup"><span data-stu-id="110ed-104">Use the SharePoint Framework library for Microsoft Graph Toolkit to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

<span data-ttu-id="110ed-105">Para impedir que vários componentes registrem seu próprio conjunto de componentes do Microsoft Graph Toolkit na página, você deve implantar essa biblioteca em seu locatário e fazer referência aos componentes do Microsoft Graph Toolkit que você usa em sua solução a partir desta biblioteca.</span><span class="sxs-lookup"><span data-stu-id="110ed-105">To prevent multiple components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy this library to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this library.</span></span>

## <a name="installation"></a><span data-ttu-id="110ed-106">Instalação</span><span class="sxs-lookup"><span data-stu-id="110ed-106">Installation</span></span>

<span data-ttu-id="110ed-107">Para carregar os componentes Graph Toolkit Microsoft da biblioteca, adicione o pacote como uma dependência de tempo de execução ao `@microsoft/mgt-spfx` seu Estrutura do SharePoint projeto:</span><span class="sxs-lookup"><span data-stu-id="110ed-107">To load Microsoft Graph Toolkit components from the library, add the `@microsoft/mgt-spfx` package as a runtime dependency to your SharePoint Framework project:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

<span data-ttu-id="110ed-108">ou</span><span class="sxs-lookup"><span data-stu-id="110ed-108">or</span></span>

```bash
yarn add @microsoft/mgt-spfx
```

<span data-ttu-id="110ed-109">Antes de implantar seu pacote Estrutura do SharePoint no locatário, você precisará implantar o pacote Estrutura do SharePoint `@microsoft/mgt-spfx` para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="110ed-109">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the `@microsoft/mgt-spfx` SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="110ed-110">Você pode baixar o pacote correspondente à versão do que você usou em seu projeto, na seção `@microsoft/mgt-spfx` [Versões](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="110ed-110">You can download the package corresponding to the version of `@microsoft/mgt-spfx` that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="110ed-111">Como apenas uma versão da biblioteca Estrutura do SharePoint do Microsoft Graph Toolkit pode ser instalada no locatário, antes de usar o Microsoft Graph Toolkit em sua solução, determine se sua organização ou cliente já tem uma versão da biblioteca Estrutura do SharePoint implantada e use a mesma versão.</span><span class="sxs-lookup"><span data-stu-id="110ed-111">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

## <a name="usage"></a><span data-ttu-id="110ed-112">Uso</span><span class="sxs-lookup"><span data-stu-id="110ed-112">Usage</span></span>

<span data-ttu-id="110ed-113">Ao criar Estrutura do SharePoint web parts e extensões, consulte o microsoft Graph Toolkit `Provider` `SharePointProvider` e do `@microsoft/mgt-spfx` pacote.</span><span class="sxs-lookup"><span data-stu-id="110ed-113">When building SharePoint Framework web parts and extensions, reference the Microsoft Graph Toolkit `Provider` and `SharePointProvider` from the `@microsoft/mgt-spfx` package.</span></span> <span data-ttu-id="110ed-114">Isso garantirá que sua solução use o Microsoft Graph Toolkit componentes que já estão registrados na página, em vez de instalar seus próprios componentes.</span><span class="sxs-lookup"><span data-stu-id="110ed-114">This will ensure that your solution will use Microsoft Graph Toolkit components that are already registered on the page, rather than instantiating its own.</span></span> <span data-ttu-id="110ed-115">O processo de instação é o mesmo para todas as Web Parts, independentemente da estrutura JavaScript usada.</span><span class="sxs-lookup"><span data-stu-id="110ed-115">The instantiation process is the same for all web parts no matter which JavaScript framework they use.</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';

// [...] trimmed for brevity

export default class MgtWebPart extends BaseClientSideWebPart<IMgtWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  // [...] trimmed for brevity
}
```

<span data-ttu-id="110ed-116">Ao criar web parts usando uma estrutura diferente React, você pode carregar componentes diretamente na Web Part:</span><span class="sxs-lookup"><span data-stu-id="110ed-116">When building web parts using a framework other than React, you can load components directly in your web part:</span></span>

```ts
export default class MgtNoFrameworkWebPart extends BaseClientSideWebPart<IMgtNoFrameworkWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  public render(): void {
    this.domElement.innerHTML = `
      <div>
        <mgt-person person-query="me"></mgt-person>
      </div>`;
  }

  // [...] trimmed for brevity
}
```

### <a name="react"></a><span data-ttu-id="110ed-117">React</span><span class="sxs-lookup"><span data-stu-id="110ed-117">React</span></span>

<span data-ttu-id="110ed-118">Se você estiver criando uma Web Part usando React, poderá usar o `@microsoft/mgt-react` pacote.</span><span class="sxs-lookup"><span data-stu-id="110ed-118">If you're building a web part using React, you can use the `@microsoft/mgt-react` package.</span></span> <span data-ttu-id="110ed-119">No entanto, certifique-se de importar todos os React do `@microsoft/mgt-react/dist/es6/spfx` caminho.</span><span class="sxs-lookup"><span data-stu-id="110ed-119">However, make sure to import all React components from the `@microsoft/mgt-react/dist/es6/spfx` path.</span></span> <span data-ttu-id="110ed-120">Isso garantirá que sua solução use apenas componentes do Microsoft Graph Toolkit que já estão registrados na página, em vez de instalar seus próprios componentes.</span><span class="sxs-lookup"><span data-stu-id="110ed-120">This will ensure that your solution will only use Microsoft Graph Toolkit components that are already registered on the page, rather than instantiating its own.</span></span>

```tsx
import { Person } from '@microsoft/mgt-react/dist/es6/spfx';
import { ViewType } from '@microsoft/mgt-spfx';

// [...] trimmed for brevity

export default class MgtReact extends React.Component<IMgtReactProps, {}> {
  public render(): React.ReactElement<IMgtReactProps> {
    return (
      <div className={ styles.mgtReact }>
        <Person personQuery="me" view={ViewType.image}></Person>
      </div>
    );
  }
}
```

>[!IMPORTANT]
> <span data-ttu-id="110ed-121">Certifique-se de que todas as Graph Toolkit da Microsoft em sua solução sejam de:</span><span class="sxs-lookup"><span data-stu-id="110ed-121">Make sure all Microsoft Graph Toolkit imports in your solution are from either:</span></span>
> * <span data-ttu-id="110ed-122">`@microsoft/mgt-spfx` ou </span><span class="sxs-lookup"><span data-stu-id="110ed-122">`@microsoft/mgt-spfx` or</span></span>
> * `@microsoft/mgt-react/dist/es6/spfx`
> 
> <span data-ttu-id="110ed-123">Não importe de nenhum outro pacote do Microsoft Graph Toolkit ( ) para evitar empacotar sua própria cópia do kit de ferramentas e colidir `@microsoft/mgt-*` com a biblioteca compartilhada.</span><span class="sxs-lookup"><span data-stu-id="110ed-123">Do not import from any other Microsoft Graph Toolkit packages (`@microsoft/mgt-*`) to avoid packaging your own copy of the toolkit and colliding with the shared library.</span></span>

## <a name="see-also"></a><span data-ttu-id="110ed-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="110ed-124">See also</span></span>

* [<span data-ttu-id="110ed-125">Criar uma web part SharePoint com o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="110ed-125">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>](./build-a-sharepoint-web-part.md)
* [<span data-ttu-id="110ed-126">Saiba mais sobre provedores de autenticação</span><span class="sxs-lookup"><span data-stu-id="110ed-126">Learn about authentication providers</span></span>](../providers/providers.md)
