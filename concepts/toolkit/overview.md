---
title: Kit de ferramentas do Microsoft Graph (versão prévia)
description: O kit de ferramentas do Microsoft Graph é uma coleção de componentes da Web e auxiliares da estrutura para acessar e trabalhar com o Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e6d5974029625a8dd1bef0c7b981fcf2b36b747c
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242951"
---
# <a name="microsoft-graph-toolkit-preview"></a><span data-ttu-id="71a11-103">Kit de ferramentas do Microsoft Graph (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="71a11-103">Microsoft Graph Toolkit (preview)</span></span>

<span data-ttu-id="71a11-104">O kit de ferramentas do Microsoft Graph é uma coleção de componentes da Web e auxiliares da estrutura para acessar e trabalhar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71a11-104">The Microsoft Graph Toolkit is a collection of framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="71a11-105">Todos os componentes podem acessar o Microsoft Graph sem a necessidade de personalização.</span><span class="sxs-lookup"><span data-stu-id="71a11-105">ALl components can access Microsoft Graph without any customization required.</span></span>

>[!NOTE]
><span data-ttu-id="71a11-106">Esta biblioteca está em versão prévia e está no desenvolvimento inicial.</span><span class="sxs-lookup"><span data-stu-id="71a11-106">This library is in preview and is in early development.</span></span> <span data-ttu-id="71a11-107">Esperamos fazer alterações e melhorias em todos os componentes e APIs com base nos comentários da Comunidade.</span><span class="sxs-lookup"><span data-stu-id="71a11-107">We expect to make changes and improvements to all components and APIs based on feedback from the community.</span></span>

## <a name="get-started"></a><span data-ttu-id="71a11-108">Introdução</span><span class="sxs-lookup"><span data-stu-id="71a11-108">Get started</span></span>

<span data-ttu-id="71a11-109">Você pode usar os componentes referenciando o carregador diretamente (via unpkg) ou instalando o pacote do NPM.</span><span class="sxs-lookup"><span data-stu-id="71a11-109">You can use the components by referencing the loader directly (via unpkg), or by installing the npm package.</span></span>

<span data-ttu-id="71a11-110">Para obter detalhes sobre como começar a usar o kit de ferramentas do Microsoft Graph, consulte o [vídeo](https://www.youtube.com/watch?v=oZCGb2MMxa0)introdução.</span><span class="sxs-lookup"><span data-stu-id="71a11-110">For details about how to get started with the Microsoft Graph Toolkit, see the [Get started video](https://www.youtube.com/watch?v=oZCGb2MMxa0).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="71a11-111">Usar via gerenciamento-carregador</span><span class="sxs-lookup"><span data-stu-id="71a11-111">Use via mgt-loader</span></span>

<span data-ttu-id="71a11-112">Consulte o exemplo do seguintes [jsfiddle](https://jsfiddle.net/metulev/9phqxLd5/).</span><span class="sxs-lookup"><span data-stu-id="71a11-112">See the folowing [jsfiddle example](https://jsfiddle.net/metulev/9phqxLd5/).</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

<span data-ttu-id="71a11-113">Você pode começar a usar os componentes na sua página HTML.</span><span class="sxs-lookup"><span data-stu-id="71a11-113">You can then start using the components in your HTML page.</span></span> <span data-ttu-id="71a11-114">A seguir está um exemplo de trabalho completo com o provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="71a11-114">The following is a full working example with the MSAL provider.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> <span data-ttu-id="71a11-115">**Observação:** O MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="71a11-115">**Note:** MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> <span data-ttu-id="71a11-116">Se você está apenas começando e deseja jogar, é possível usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="71a11-116">If you're just getting started and want to play around, you can use [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code.</span></span>

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="71a11-117">Usar via NPM (módulos es6)</span><span class="sxs-lookup"><span data-stu-id="71a11-117">Use via NPM (es6 modules)</span></span>

<span data-ttu-id="71a11-118">Usando os módulos do es6, você tem controle total sobre o processo de agrupamento e pode agrupar apenas o código necessário para o seu site.</span><span class="sxs-lookup"><span data-stu-id="71a11-118">By using the es6 modules, you have full control of the bundling process and you can bundle only the code you need for your site.</span></span> <span data-ttu-id="71a11-119">Primeiro, adicione o pacote NPM:</span><span class="sxs-lookup"><span data-stu-id="71a11-119">First, add the npm package:</span></span>

```bash
npm install @microsoft/mgt
```

<span data-ttu-id="71a11-120">Agora, você pode fazer referência a todos os componentes na página que está usando:</span><span class="sxs-lookup"><span data-stu-id="71a11-120">Now you can reference all components at the page you are using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="71a11-121">Ou, apenas faça referência ao componente de que você precisa e Evite carregar tudo o mais:</span><span class="sxs-lookup"><span data-stu-id="71a11-121">Or, just reference the component you need and avoid loading everything else:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

<span data-ttu-id="71a11-122">Da mesma forma, para adicionar um provedor, você pode adicioná-lo como um componente:</span><span class="sxs-lookup"><span data-stu-id="71a11-122">Similarly, to add a provider, you can add it as a component:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

<span data-ttu-id="71a11-123">ou, adicione-o em seu código:</span><span class="sxs-lookup"><span data-stu-id="71a11-123">or, add it in your code:</span></span>

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a><span data-ttu-id="71a11-124">Provedores</span><span class="sxs-lookup"><span data-stu-id="71a11-124">Providers</span></span>

<span data-ttu-id="71a11-125">Os componentes funcionam melhor quando usados com um [provedor](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="71a11-125">The components work best when used with a [provider](./providers.md).</span></span> <span data-ttu-id="71a11-126">O provedor expõe a autenticação e as APIs que os componentes usam para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="71a11-126">The provider exposes authentication and APIs that the components use to call Microsoft Graph.</span></span>

<span data-ttu-id="71a11-127">O kit de ferramentas contém provedores para os suplementos do [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md)e Office (em breve).</span><span class="sxs-lookup"><span data-stu-id="71a11-127">The toolkit contains providers for [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md), and Office Add-ins (coming soon).</span></span> <span data-ttu-id="71a11-128">Você também pode criar seus próprios provedores, estendendo a classe abstrata [IProvider].</span><span class="sxs-lookup"><span data-stu-id="71a11-128">You can also create your own providers by extending the [IProvider] abstract class.</span></span>

## <a name="polyfills"></a><span data-ttu-id="71a11-129">Polyfills</span><span class="sxs-lookup"><span data-stu-id="71a11-129">Polyfills</span></span>

<span data-ttu-id="71a11-130">Se você estiver usando os módulos es6 do pacote do NPM, certifique-se de incluir os metapreenchimentos no projeto, pois eles não serão incluídos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="71a11-130">If you're using the es6 modules from the npm package, make sure to include polyfills in your project as they are not included automatically.</span></span> <span data-ttu-id="71a11-131">Para saber mais, confira polipreenchimentos. [](https://www.webcomponents.org/polyfills)</span><span class="sxs-lookup"><span data-stu-id="71a11-131">To learn more, see [polyfills](https://www.webcomponents.org/polyfills).</span></span>

<span data-ttu-id="71a11-132">Se você estiver usando o script MGT-Loader. js do pacote no unpkg, os metapreenchimentos já estão incluídos.</span><span class="sxs-lookup"><span data-stu-id="71a11-132">If you're using the mgt-loader.js script from the bundle on unpkg, the polyfills are already included.</span></span>


## <a name="using-the-components-with-react-angular-and-other-frameworks"></a><span data-ttu-id="71a11-133">Usando os componentes com reagir, angular e outras estruturas</span><span class="sxs-lookup"><span data-stu-id="71a11-133">Using the components with React, Angular, and other frameworks</span></span>

<span data-ttu-id="71a11-134">Os componentes Web são baseados em vários padrões da Web e podem ser usados com qualquer estrutura que você já esteja usando.</span><span class="sxs-lookup"><span data-stu-id="71a11-134">Web components are based on several web standards and can be used with any framework you're already using.</span></span> <span data-ttu-id="71a11-135">No entanto, nem todas as estruturas lidam com os componentes da Web da mesma maneira.</span><span class="sxs-lookup"><span data-stu-id="71a11-135">However, not all frameworks handle web components the same way.</span></span> <span data-ttu-id="71a11-136">Para saber mais sobre as considerações que podem ser aplicadas dependendo da sua estrutura, confira o projeto [elementos personalizados em qualquer lugar](https://custom-elements-everywhere.com/) .</span><span class="sxs-lookup"><span data-stu-id="71a11-136">To learn more about the considerations that might apply depending on your framework, see the [Custom Elements Everywhere](https://custom-elements-everywhere.com/) project.</span></span>

<span data-ttu-id="71a11-137">As seções a seguir fornecem uma visão geral rápida do uso dos componentes do Microsoft Graph Toolkit com reagir e angulares.</span><span class="sxs-lookup"><span data-stu-id="71a11-137">The following sections provide a quick overview of using the Microsoft Graph Toolkit components with React and Angular.</span></span>

### <a name="react"></a><span data-ttu-id="71a11-138">React</span><span class="sxs-lookup"><span data-stu-id="71a11-138">React</span></span>

<span data-ttu-id="71a11-139">Reagir transfere todos os dados para elementos personalizados na forma de atributos HTML.</span><span class="sxs-lookup"><span data-stu-id="71a11-139">React passes all data to Custom Elements in the form of HTML attributes.</span></span> <span data-ttu-id="71a11-140">Para dados primitivos, isso é bom, mas não funciona ao transmitir dados ricos, como objetos ou matrizes.</span><span class="sxs-lookup"><span data-stu-id="71a11-140">For primitive data this is fine, but it does not work when passing rich data, like objects or arrays.</span></span> <span data-ttu-id="71a11-141">Nesses casos, você precisará usar um `ref` para passar no objeto.</span><span class="sxs-lookup"><span data-stu-id="71a11-141">In those cases you will need to use a `ref` to pass in the object.</span></span>

<span data-ttu-id="71a11-142">Ex</span><span class="sxs-lookup"><span data-stu-id="71a11-142">Ex:</span></span>

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

<span data-ttu-id="71a11-143">Como reagir implementa seu próprio sistema de eventos sintético, ele não pode escutar eventos DOM provenientes de elementos personalizados sem o uso de uma solução alternativa.</span><span class="sxs-lookup"><span data-stu-id="71a11-143">Because React implements its own synthetic event system, it cannot listen for DOM events coming from custom elements without the use of a workaround.</span></span> <span data-ttu-id="71a11-144">Você precisará usar um `ref` para fazer referência aos componentes do kit de ferramentas e anexar manualmente ouvintes de eventos com addEventListener, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="71a11-144">You will need to use a `ref` to reference the toolkit components and manually attach event listeners with addEventListener, as shown in the following example.</span></span>

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

#### <a name="react-typescript-and-tsx"></a><span data-ttu-id="71a11-145">Reagir, typescript e TSX</span><span class="sxs-lookup"><span data-stu-id="71a11-145">React, Typescript, and TSX</span></span>

<span data-ttu-id="71a11-146">Um problema conhecido pode ocorrer quando você usa elementos personalizados com reagir e typescript.</span><span class="sxs-lookup"><span data-stu-id="71a11-146">A known issue can occur when you use custom elements with React and Typescript.</span></span> <span data-ttu-id="71a11-147">O typescript gerará um erro ao tentar usar um componente no TSX.</span><span class="sxs-lookup"><span data-stu-id="71a11-147">Typescript will throw an error when trying to use a component in tsx.</span></span> <span data-ttu-id="71a11-148">A solução alternativa é definir o elemento personalizado em seu código, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="71a11-148">The workaround is to define the custom element in your code, as shown.</span></span>

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

<span data-ttu-id="71a11-149">Você pode usá-lo no seu TSX como `<mgt-login></mgt-login>`.</span><span class="sxs-lookup"><span data-stu-id="71a11-149">You can then use it in your tsx as `<mgt-login></mgt-login>`.</span></span>

### <a name="angular"></a><span data-ttu-id="71a11-150">Angular</span><span class="sxs-lookup"><span data-stu-id="71a11-150">Angular</span></span>

<span data-ttu-id="71a11-151">A sintaxe de associação padrão do angular sempre definirá Propriedades em um elemento.</span><span class="sxs-lookup"><span data-stu-id="71a11-151">Angular's default binding syntax will always set properties on an element.</span></span> <span data-ttu-id="71a11-152">Isso funciona bem para dados ricos, como objetos e matrizes, e também funciona bem para valores primitivos.</span><span class="sxs-lookup"><span data-stu-id="71a11-152">This works well for rich data, like objects and arrays, and also works well for primitive values.</span></span>

<span data-ttu-id="71a11-153">Para usar elementos personalizados, primeiro, habilite os elementos personalizados `app.module.ts` em seu adicionando `CUSTOM_ELEMENT_SCHEMA` o ao `@NgModule() decorator`, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="71a11-153">To use custom elements, first, enable custom elements in your `app.module.ts` by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator`, as shown in the following example.</span></span>

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

<span data-ttu-id="71a11-154">Você pode importar o componente que gostaria de usar em seu arquivo Component \*. TS.</span><span class="sxs-lookup"><span data-stu-id="71a11-154">You can then import the component you'd like to use in your component \*.ts file.</span></span>

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

<span data-ttu-id="71a11-155">Por fim, use o componente como faria normalmente no seu modelo.</span><span class="sxs-lookup"><span data-stu-id="71a11-155">Finally, use the component as you normally would in your template.</span></span>

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```
