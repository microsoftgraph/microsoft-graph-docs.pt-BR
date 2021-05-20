---
title: Estrutura do SharePoint biblioteca do Microsoft Graph Toolkit
description: Use a Estrutura do SharePoint do Microsoft Graph Toolkit para usar o Microsoft Graph Toolkit em Estrutura do SharePoint soluções.
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 17a6e899003dec34a6dac41daaeba7e2c0e3fba1
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579796"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a><span data-ttu-id="fb7d5-103">Estrutura do SharePoint biblioteca do Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="fb7d5-103">SharePoint Framework library for Microsoft Graph Toolkit</span></span>

<span data-ttu-id="fb7d5-104">Use a Estrutura do SharePoint do Microsoft Graph Toolkit para usar o Microsoft Graph Toolkit em Estrutura do SharePoint soluções.</span><span class="sxs-lookup"><span data-stu-id="fb7d5-104">Use the SharePoint Framework library for Microsoft Graph Toolkit to use Microsoft Graph Toolkit in SharePoint Framework solutions.</span></span>

<span data-ttu-id="fb7d5-105">Para impedir que vários componentes registrem seu próprio conjunto de componentes do Microsoft Graph Toolkit na página, você deve implantar essa biblioteca em seu locatário e fazer referência aos componentes do Microsoft Graph Toolkit que você usa em sua solução a partir desta biblioteca.</span><span class="sxs-lookup"><span data-stu-id="fb7d5-105">To prevent multiple components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy this library to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this library.</span></span>

## <a name="installation"></a><span data-ttu-id="fb7d5-106">Instalação</span><span class="sxs-lookup"><span data-stu-id="fb7d5-106">Installation</span></span>

<span data-ttu-id="fb7d5-107">Para carregar os componentes Graph Toolkit Microsoft da biblioteca, adicione o pacote como uma dependência de tempo de execução ao `@microsoft/mgt-spfx` seu Estrutura do SharePoint projeto:</span><span class="sxs-lookup"><span data-stu-id="fb7d5-107">To load Microsoft Graph Toolkit components from the library, add the `@microsoft/mgt-spfx` package as a runtime dependency to your SharePoint Framework project:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

<span data-ttu-id="fb7d5-108">ou</span><span class="sxs-lookup"><span data-stu-id="fb7d5-108">or</span></span>

```bash
yarn add @microsoft/mgt-spfx
```

<span data-ttu-id="fb7d5-109">Antes de implantar seu pacote Estrutura do SharePoint no locatário, você precisará implantar o pacote Estrutura do SharePoint `@microsoft/mgt-spfx` para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="fb7d5-109">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the `@microsoft/mgt-spfx` SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="fb7d5-110">Você pode baixar o pacote correspondente à versão do que você usou em seu projeto, na seção `@microsoft/mgt-spfx` [Versões](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="fb7d5-110">You can download the package corresponding to the version of `@microsoft/mgt-spfx` that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="fb7d5-111">Como apenas uma versão da biblioteca Estrutura do SharePoint do Microsoft Graph Toolkit pode ser instalada no locatário, antes de usar o Microsoft Graph Toolkit em sua solução, determine se sua organização ou cliente já tem uma versão da biblioteca Estrutura do SharePoint implantada e use a mesma versão.</span><span class="sxs-lookup"><span data-stu-id="fb7d5-111">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

## <a name="usage"></a><span data-ttu-id="fb7d5-112">Uso</span><span class="sxs-lookup"><span data-stu-id="fb7d5-112">Usage</span></span>

<span data-ttu-id="fb7d5-113">Ao criar Estrutura do SharePoint web parts e extensões, consulte o microsoft Graph Toolkit `Provider` `SharePointProvider` e do `@microsoft/mgt-spfx` pacote.</span><span class="sxs-lookup"><span data-stu-id="fb7d5-113">When building SharePoint Framework web parts and extensions, reference the Microsoft Graph Toolkit `Provider` and `SharePointProvider` from the `@microsoft/mgt-spfx` package.</span></span> <span data-ttu-id="fb7d5-114">Isso garantirá que sua solução use o Microsoft Graph Toolkit componentes que já estão registrados na página, em vez de instalar seus próprios componentes.</span><span class="sxs-lookup"><span data-stu-id="fb7d5-114">This will ensure that your solution will use Microsoft Graph Toolkit components that are already registered on the page, rather than instantiating its own.</span></span> <span data-ttu-id="fb7d5-115">O processo de instação é o mesmo para todas as Web Parts, independentemente da estrutura JavaScript usada.</span><span class="sxs-lookup"><span data-stu-id="fb7d5-115">The instantiation process is the same for all web parts no matter which JavaScript framework they use.</span></span>

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

<span data-ttu-id="fb7d5-116">Ao criar web parts usando uma estrutura diferente React, você pode carregar componentes diretamente na Web Part:</span><span class="sxs-lookup"><span data-stu-id="fb7d5-116">When building web parts using a framework other than React, you can load components directly in your web part:</span></span>

```ts
export default class MgtNoFrameworkWebPart extends BaseClientSideWebPart<IMgtNoFrameworkWebPartProps> {
  protected async onInit() {
    if (!Providers.globalProvider) {
      Providers.globalProvider = new SharePointProvider(this.context);
    }
  }

  public render(): void {
    this.domElement.innerHTML = `
      <div class="${styles.mgtNoFramework}">
        <div class="${styles.container}">
          <div class="${styles.row}">
            <div class="${styles.column}">
              <span class="${styles.title}">No framework webpart</span>
              <mgt-person person-query="me" show-name show-email></mgt-person>
            </div>
          </div>
        </div>
      </div>`;
  }

  // [...] trimmed for brevity
}
```

<span data-ttu-id="fb7d5-117">Se você criar uma Web Part usando React, carregue componentes do `@microsoft/mgt-react` pacote:</span><span class="sxs-lookup"><span data-stu-id="fb7d5-117">If you build a web part using React, load components from the `@microsoft/mgt-react` package:</span></span>

```tsx
import { Person } from '@microsoft/mgt-react';

// [...] trimmed for brevity

export default class MgtReact extends React.Component<IMgtReactProps, {}> {
  public render(): React.ReactElement<IMgtReactProps> {
    return (
      <div className={ styles.mgtReact }>
        <Person personQuery="me" />
      </div>
    );
  }
}
```

## <a name="see-also"></a><span data-ttu-id="fb7d5-118">Confira também</span><span class="sxs-lookup"><span data-stu-id="fb7d5-118">See also</span></span>

* [<span data-ttu-id="fb7d5-119">Criar uma web part SharePoint com o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="fb7d5-119">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>](./build-a-sharepoint-web-part.md)
* [<span data-ttu-id="fb7d5-120">Saiba mais sobre provedores de autenticação</span><span class="sxs-lookup"><span data-stu-id="fb7d5-120">Learn about authentication providers</span></span>](../providers/providers.md)
