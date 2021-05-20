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
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a>Estrutura do SharePoint biblioteca do Microsoft Graph Toolkit

Use a Estrutura do SharePoint do Microsoft Graph Toolkit para usar o Microsoft Graph Toolkit em Estrutura do SharePoint soluções.

Para impedir que vários componentes registrem seu próprio conjunto de componentes do Microsoft Graph Toolkit na página, você deve implantar essa biblioteca em seu locatário e fazer referência aos componentes do Microsoft Graph Toolkit que você usa em sua solução a partir desta biblioteca.

## <a name="installation"></a>Instalação

Para carregar os componentes Graph Toolkit Microsoft da biblioteca, adicione o pacote como uma dependência de tempo de execução ao `@microsoft/mgt-spfx` seu Estrutura do SharePoint projeto:

```bash
npm install @microsoft/mgt-spfx
```

ou

```bash
yarn add @microsoft/mgt-spfx
```

Antes de implantar seu pacote Estrutura do SharePoint no locatário, você precisará implantar o pacote Estrutura do SharePoint `@microsoft/mgt-spfx` para seu locatário. Você pode baixar o pacote correspondente à versão do que você usou em seu projeto, na seção `@microsoft/mgt-spfx` [Versões](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) no GitHub.

>[!IMPORTANT]
>Como apenas uma versão da biblioteca Estrutura do SharePoint do Microsoft Graph Toolkit pode ser instalada no locatário, antes de usar o Microsoft Graph Toolkit em sua solução, determine se sua organização ou cliente já tem uma versão da biblioteca Estrutura do SharePoint implantada e use a mesma versão.

## <a name="usage"></a>Uso

Ao criar Estrutura do SharePoint web parts e extensões, consulte o microsoft Graph Toolkit `Provider` `SharePointProvider` e do `@microsoft/mgt-spfx` pacote. Isso garantirá que sua solução use o Microsoft Graph Toolkit componentes que já estão registrados na página, em vez de instalar seus próprios componentes. O processo de instação é o mesmo para todas as Web Parts, independentemente da estrutura JavaScript usada.

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

Ao criar web parts usando uma estrutura diferente React, você pode carregar componentes diretamente na Web Part:

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

Se você criar uma Web Part usando React, carregue componentes do `@microsoft/mgt-react` pacote:

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

## <a name="see-also"></a>Confira também

* [Criar uma web part SharePoint com o microsoft Graph Toolkit](./build-a-sharepoint-web-part.md)
* [Saiba mais sobre provedores de autenticação](../providers/providers.md)
