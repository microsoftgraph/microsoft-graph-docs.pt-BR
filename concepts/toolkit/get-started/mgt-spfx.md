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
      <div>
        <mgt-person person-query="me"></mgt-person>
      </div>`;
  }

  // [...] trimmed for brevity
}
```

### <a name="react"></a>React

Se você estiver criando uma Web Part usando React, poderá usar o `@microsoft/mgt-react` pacote. No entanto, certifique-se de importar todos os React do `@microsoft/mgt-react/dist/es6/spfx` caminho. Isso garantirá que sua solução use apenas componentes do Microsoft Graph Toolkit que já estão registrados na página, em vez de instalar seus próprios componentes.

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
> Certifique-se de que todas as Graph Toolkit da Microsoft em sua solução sejam de:
> * `@microsoft/mgt-spfx` ou 
> * `@microsoft/mgt-react/dist/es6/spfx`
> 
> Não importe de nenhum outro pacote do Microsoft Graph Toolkit ( ) para evitar empacotar sua própria cópia do kit de ferramentas e colidir `@microsoft/mgt-*` com a biblioteca compartilhada.

## <a name="see-also"></a>Confira também

* [Criar uma web part SharePoint com o microsoft Graph Toolkit](./build-a-sharepoint-web-part.md)
* [Saiba mais sobre provedores de autenticação](../providers/providers.md)
