---
title: Introdução ao Microsoft Graph Toolkit
description: Comece a usar o Microsoft Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 1537a686d25d885a898603ca576f688abdaab3e4
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639930"
---
# <a name="get-started-with-the-microsoft-graph-toolkit"></a>Introdução ao Microsoft Graph Toolkit

O Microsoft Graph Toolkit pode ser incluído facilmente no seu aplicativo Web, na Web Part do SharePoint ou na guia Microsoft Teams. Os componentes são criados em padrões da Web existentes e são compatíveis com qualquer estrutura da Web e navegador moderno. Este tópico descreve como começar a usar o Microsoft Graph Toolkit em seu projeto.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote do NPM.

## <a name="use-via-mgt-loader"></a>Usar via gerenciamento-carregador

Para usar o kit de ferramentas via gerenciamento-Loader, confira o exemplo a seguir.

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

Você pode começar a usar os componentes na sua página HTML. A seguir está um exemplo de trabalho completo com o provedor MSAL.

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> **Observação:** O MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação. Se você está apenas começando e deseja jogar, é possível usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no Visual Studio Code.

## <a name="use-via-npm-es6-modules"></a>Usar via NPM (módulos es6)

Usando os módulos do es6, você tem controle total sobre o processo de agrupamento e pode agrupar apenas o código necessário para o seu site. Primeiro, adicione o pacote NPM:

```bash
npm install @microsoft/mgt
```

Agora, você pode fazer referência a todos os componentes na página que está usando:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

Ou, apenas faça referência ao componente de que você precisa e Evite carregar tudo o mais:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

Da mesma forma, para adicionar um provedor, você pode adicioná-lo como um componente:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

Ou, adicione-o em seu código:

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a>Provedores

Os componentes funcionam melhor quando usados com um [provedor](./providers.md). O provedor expõe a autenticação e as APIs que os componentes usam para chamar o Microsoft Graph.

O kit de ferramentas contém provedores para o [MSAL](./providers/msal.md), o [SharePoint](./providers/sharepoint.md)e o Microsoft [Teams](./providers/teams.md). Você também pode usar sua própria lógica de autenticação criando um [provedor personalizado](./providers/custom.md)ou usando o [proxyprovider](./providers/proxy.md) com sua própria autenticação de backend. 

## <a name="polyfills"></a>Polyfills

Se você estiver usando os módulos es6 do pacote do NPM, certifique-se de incluir os metapreenchimentos no projeto, pois eles não serão incluídos automaticamente. Para saber mais, confira [polipreenchimentos](https://www.webcomponents.org/polyfills).

Se você estiver usando o script MGT-Loader. js do pacote no unpkg, os metapreenchimentos já estão incluídos.


## <a name="using-the-components-with-react-angular-and-other-frameworks"></a>Usando os componentes com reagir, angular e outras estruturas

Os componentes Web são baseados em vários padrões da Web e podem ser usados com qualquer estrutura que você já esteja usando. No entanto, nem todas as estruturas lidam com os componentes da Web da mesma maneira. Para saber mais sobre as considerações que podem ser aplicadas dependendo da sua estrutura, confira o projeto [elementos personalizados em qualquer lugar](https://custom-elements-everywhere.com/) .

As seções a seguir fornecem uma visão geral rápida do uso dos componentes do Microsoft Graph Toolkit com reagir e angulares.

### <a name="react"></a>React

Reagir transfere todos os dados para elementos personalizados na forma de atributos HTML. Para dados primitivos, isso é bom, mas não funciona ao transmitir dados ricos, como objetos ou matrizes. Nesses casos, você precisará usar um `ref` para passar no objeto.

Ex

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

Como reagir implementa seu próprio sistema de eventos sintético, ele não pode escutar eventos DOM provenientes de elementos personalizados sem o uso de uma solução alternativa. Você precisará usar um `ref` para fazer referência aos componentes do kit de ferramentas e anexar manualmente ouvintes de eventos com addEventListener, conforme mostrado no exemplo a seguir.

```jsx
// you can just import a single component
import '@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js';

class App extends Component {
  render() {
    return <mgt-login ref="loginComponent" />;
  }

  componentDidMount() {
    this.refs.loginComponent.addEventListener('loginCompleted', e => {
      // handle event
    });
  }
}
```

#### <a name="react-typescript-and-tsx"></a>Reagir, typescript e TSX

Um problema conhecido pode ocorrer quando você usa elementos personalizados com reagir e typescript. O typescript gerará um erro ao tentar usar um componente no TSX. A solução alternativa é definir o elemento personalizado em seu código, conforme mostrado.

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

Você pode usá-lo no seu TSX como `<mgt-login></mgt-login>`.

### <a name="angular"></a>Angular

A sintaxe de associação padrão do angular sempre definirá Propriedades em um elemento. Isso funciona bem para dados ricos, como objetos e matrizes, e também funciona bem para valores primitivos.

Para usar elementos personalizados, primeiro, habilite os elementos personalizados `app.module.ts` em seu adicionando `CUSTOM_ELEMENT_SCHEMA` o ao `@NgModule() decorator`, conforme mostrado no exemplo a seguir.

```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule {}
```

Você pode importar o componente que gostaria de usar em seu arquivo Component \*. TS.

```ts
import { Component } from '@angular/core';
import '@microsoft/mgt/dist/es6/components/mgt-person/mgt-person';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  person = {
    displayName: 'Nikola Metulev'
  };
}
```

Por fim, use o componente como faria normalmente no seu modelo.

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```
