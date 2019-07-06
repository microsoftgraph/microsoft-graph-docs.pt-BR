---
title: Kit de ferramentas do Microsoft Graph (versão prévia)
description: O kit de ferramentas do Microsoft Graph é uma coleção de componentes da Web e auxiliares da estrutura para acessar e trabalhar com o Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ca55500217ab23f9e6a2744da61f332e745af398
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576400"
---
# <a name="microsoft-graph-toolkit-preview"></a>Kit de ferramentas do Microsoft Graph (versão prévia)

O kit de ferramentas do Microsoft Graph é uma coleção de componentes da Web e auxiliares da estrutura para acessar e trabalhar com o Microsoft Graph. Todos os componentes podem acessar o Microsoft Graph sem a necessidade de personalização.

> [!NOTE]
> Esta biblioteca está em versão prévia e está no desenvolvimento inicial. Esperamos fazer alterações e melhorias em todos os componentes e APIs com base nos comentários da Comunidade.

## <a name="get-started"></a>Introdução

Você pode usar os componentes referenciando o carregador diretamente (via unpkg) ou instalando o pacote do NPM.

Para obter detalhes sobre como começar a usar o kit de ferramentas do Microsoft Graph, consulte o [vídeo](https://www.youtube.com/watch?v=oZCGb2MMxa0)introdução.

### <a name="use-via-mgt-loader"></a>Usar via gerenciamento-carregador

Consulte o exemplo do seguintes [jsfiddle](https://jsfiddle.net/metulev/9phqxLd5/).

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

### <a name="use-via-npm-es6-modules"></a>Usar via NPM (módulos es6)

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

ou, adicione-o em seu código:

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a>Provedores

Os componentes funcionam melhor quando usados com um [provedor](./providers.md). O provedor expõe a autenticação e as APIs que os componentes usam para chamar o Microsoft Graph.

O kit de ferramentas contém provedores para os suplementos do [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md)e Office (em breve). Você também pode criar seus próprios provedores, estendendo a classe abstrata [IProvider].

## <a name="polyfills"></a>Polyfills

Se você estiver usando os módulos es6 do pacote do NPM, certifique-se de incluir os metapreenchimentos no projeto, pois eles não serão incluídos automaticamente. Para saber mais, confira polipreenchimentos. [](https://www.webcomponents.org/polyfills)

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
