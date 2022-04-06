---
title: Biblioteca da Estrutura do SharePoint para o Kit de ferramentas do Microsoft Graph
description: Use a Estrutura do SharePoint do Microsoft Graph Toolkit usar o Microsoft Graph Toolkit em Estrutura do SharePoint soluções.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 952ff0852f4c1c0cf1efb2be2ab3cbe89d805f00
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588789"
---
# <a name="sharepoint-framework-library-for-microsoft-graph-toolkit"></a>Biblioteca da Estrutura do SharePoint para o Kit de ferramentas do Microsoft Graph

Use a Estrutura do SharePoint do Microsoft Graph Toolkit usar o Microsoft Graph Toolkit em Estrutura do SharePoint soluções.

Para impedir que vários componentes registrem seu próprio conjunto de componentes do Microsoft Graph Toolkit na página, você deve implantar essa biblioteca em seu locatário e fazer referência aos componentes do Microsoft Graph Toolkit que você usa em sua solução a partir desta biblioteca.

> [!CAUTION]
> A Estrutura do SharePoint do Microsoft Graph Toolkit deve ser usada com extensões Estrutura do SharePoint e **web parts não isoladas**. Se você estiver criando web parts isoladas, não use a biblioteca Estrutura do SharePoint para o Microsoft Graph Toolkit. Em vez disso, carregue o Microsoft Graph Toolkit diretamente do pacote @microsoft/mgt (ou @microsoft/mgt-react se você usar React). Estrutura do SharePoint não dá suporte a referenciar componentes de biblioteca de web parts isoladas e isso causará erros de tempo de execução na Web Part isolada.

## <a name="installation"></a>Instalação

Para carregar componentes Graph Toolkit Microsoft da biblioteca, adicione `@microsoft/mgt-spfx` o pacote como uma dependência de tempo de execução ao seu Estrutura do SharePoint projeto:

```bash
npm install @microsoft/mgt-spfx
```

ou

```bash
yarn add @microsoft/mgt-spfx
```

Antes de implantar seu pacote Estrutura do SharePoint no locatário, `@microsoft/mgt-spfx` você precisará implantar o pacote Estrutura do SharePoint para seu locatário. Você pode baixar o pacote correspondente à versão `@microsoft/mgt-spfx` do que você usou em seu projeto, na seção Versões [](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) no GitHub.

>[!IMPORTANT]
>Como apenas uma versão da biblioteca da Estrutura do SharePoint para o Kit de ferramentas do Microsoft Graph pode ser instalada no locatário, antes de usar o Kit de ferramentas do Microsoft Graph em sua solução, determine se sua organização ou cliente já possui uma versão da biblioteca da Estrutura do SharePoint implantada e use o mesma versão.

## <a name="usage"></a>Uso

Ao criar Estrutura do SharePoint web parts e extensões, consulte o microsoft Graph Toolkit `Provider` e `SharePointProvider` do `@microsoft/mgt-spfx` pacote. Isso garantirá que sua solução use os componentes do Microsoft Graph Toolkit que já estão registrados na página, em vez de instalar seus próprios componentes. O processo de instação é o mesmo para todas as Web Parts, independentemente da estrutura JavaScript usada.

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

Ao criar web parts usando uma estrutura diferente React, você pode carregar componentes diretamente em sua Web Part:

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

Se você estiver criando uma Web Part usando React, poderá usar o `@microsoft/mgt-react` pacote. No entanto, certifique-se de importar todos os React do `@microsoft/mgt-react/dist/es6/spfx` caminho. Isso garantirá que sua solução use apenas os componentes do Microsoft Graph Toolkit que já estão registrados na página, em vez de instalar seus próprios componentes.

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
> Não importe de nenhum outro pacote do Microsoft Graph Toolkit (`@microsoft/mgt-*`) para evitar empacotar sua própria cópia do kit de ferramentas e colidir com a biblioteca compartilhada.

## <a name="see-also"></a>Confira também

* [Criar uma web part do Microsoft Office SharePoint Online com o Kit de ferramentas do Microsoft Graph](./build-a-sharepoint-web-part.md)
* [Saiba mais sobre provedores de autenticação](../providers/providers.md)
