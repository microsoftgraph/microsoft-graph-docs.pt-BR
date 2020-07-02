---
title: Introdução ao Microsoft Graph Toolkit
description: Comece a usar o Microsoft Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 2e352a71b7e1f068bfb6dbd13a6ed151dd1b84b0
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007063"
---
# <a name="get-started-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="9c4f8-103">Introdução ao Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="9c4f8-103">Get started with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9c4f8-104">O Microsoft Graph Toolkit pode ser incluído facilmente no seu aplicativo Web, na Web Part do SharePoint ou na guia Microsoft Teams. Os componentes são criados em padrões da Web existentes e são compatíveis com qualquer estrutura da Web e navegador moderno.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-104">The Microsoft Graph Toolkit can easily be included in your web application, SharePoint web part, or Microsoft Teams tab. The components are built on existing web standards and are compatible with any web framework and modern browser.</span></span> <span data-ttu-id="9c4f8-105">Este tópico descreve como começar a usar o Microsoft Graph Toolkit em seu projeto.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-105">This topic describes how to get started using the Microsoft Graph Toolkit in your project.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

<span data-ttu-id="9c4f8-106">Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote do NPM.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-106">You can use the Microsoft Graph Toolkit in your application by referencing the loader directly (via unpkg), or by installing the npm package.</span></span>

## <a name="use-via-mgt-loader"></a><span data-ttu-id="9c4f8-107">Usar via gerenciamento-carregador</span><span class="sxs-lookup"><span data-stu-id="9c4f8-107">Use via mgt-loader</span></span>

<span data-ttu-id="9c4f8-108">Para usar o kit de ferramentas via gerenciamento-Loader, confira o exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-108">To use the toolkit via mgt-loader, see the following example.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

<span data-ttu-id="9c4f8-109">Você pode começar a usar os componentes na sua página HTML.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-109">You can then start using the components in your HTML page.</span></span> <span data-ttu-id="9c4f8-110">A seguir está um exemplo de trabalho completo com o provedor MSAL.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-110">The following is a full working example with the MSAL provider.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> <span data-ttu-id="9c4f8-111">**Observação:** O MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-111">**Note:** MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> <span data-ttu-id="9c4f8-112">Se você está apenas começando e deseja jogar, é possível usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no Visual Studio Code.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-112">If you're just getting started and want to play around, you can use [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code.</span></span>

## <a name="use-via-npm-es6-modules"></a><span data-ttu-id="9c4f8-113">Usar via NPM (módulos es6)</span><span class="sxs-lookup"><span data-stu-id="9c4f8-113">Use via NPM (es6 modules)</span></span>

<span data-ttu-id="9c4f8-114">Usando os módulos do es6, você tem controle total sobre o processo de agrupamento e pode agrupar apenas o código necessário para o seu site.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-114">By using the es6 modules, you have full control of the bundling process and you can bundle only the code you need for your site.</span></span> <span data-ttu-id="9c4f8-115">Primeiro, adicione o pacote NPM:</span><span class="sxs-lookup"><span data-stu-id="9c4f8-115">First, add the npm package:</span></span>

```bash
npm install @microsoft/mgt
```

<span data-ttu-id="9c4f8-116">Agora, você pode fazer referência a todos os componentes na página que está usando:</span><span class="sxs-lookup"><span data-stu-id="9c4f8-116">Now you can reference all components at the page you are using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="9c4f8-117">Ou, apenas faça referência ao componente de que você precisa e Evite carregar tudo o mais:</span><span class="sxs-lookup"><span data-stu-id="9c4f8-117">Or, just reference the component you need and avoid loading everything else:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

<span data-ttu-id="9c4f8-118">Da mesma forma, para adicionar um provedor, você pode adicioná-lo como um componente:</span><span class="sxs-lookup"><span data-stu-id="9c4f8-118">Similarly, to add a provider, you can add it as a component:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

<span data-ttu-id="9c4f8-119">Ou, adicione-o em seu código:</span><span class="sxs-lookup"><span data-stu-id="9c4f8-119">Or, add it in your code:</span></span>

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a><span data-ttu-id="9c4f8-120">Provedores</span><span class="sxs-lookup"><span data-stu-id="9c4f8-120">Providers</span></span>

<span data-ttu-id="9c4f8-121">Os componentes funcionam melhor quando usados com um [provedor](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="9c4f8-121">The components work best when used with a [provider](./providers.md).</span></span> <span data-ttu-id="9c4f8-122">O provedor expõe a autenticação e as APIs que os componentes usam para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-122">The provider exposes authentication and APIs that the components use to call Microsoft Graph.</span></span>

<span data-ttu-id="9c4f8-123">O kit de ferramentas contém provedores para o [MSAL](./providers/msal.md), o [SharePoint](./providers/sharepoint.md)e o Microsoft [Teams](./providers/teams.md).</span><span class="sxs-lookup"><span data-stu-id="9c4f8-123">The toolkit contains providers for [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), and [Teams](./providers/teams.md).</span></span> <span data-ttu-id="9c4f8-124">Você também pode usar sua própria lógica de autenticação criando um [provedor personalizado](./providers/custom.md)ou usando o [proxyprovider](./providers/proxy.md) com sua própria autenticação de backend.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-124">You can also use your own authentication logic by creating a [custom provider](./providers/custom.md), or using the [ProxyProvider](./providers/proxy.md) with your own backend authentication.</span></span> 

## <a name="polyfills"></a><span data-ttu-id="9c4f8-125">Polyfills</span><span class="sxs-lookup"><span data-stu-id="9c4f8-125">Polyfills</span></span>

<span data-ttu-id="9c4f8-126">Se você estiver usando os módulos es6 do pacote do NPM, certifique-se de incluir os metapreenchimentos no projeto, pois eles não serão incluídos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-126">If you're using the es6 modules from the npm package, make sure to include polyfills in your project as they are not included automatically.</span></span> <span data-ttu-id="9c4f8-127">Para saber mais, confira [polipreenchimentos](https://www.webcomponents.org/polyfills).</span><span class="sxs-lookup"><span data-stu-id="9c4f8-127">To learn more, see [polyfills](https://www.webcomponents.org/polyfills).</span></span>

<span data-ttu-id="9c4f8-128">Se você estiver usando o script mgt-loader.js do pacote no unpkg, os metapreenchimentos já estão incluídos.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-128">If you're using the mgt-loader.js script from the bundle on unpkg, the polyfills are already included.</span></span>

### <a name="sharepoint"></a><span data-ttu-id="9c4f8-129">Do</span><span class="sxs-lookup"><span data-stu-id="9c4f8-129">Sharepoint</span></span>

<span data-ttu-id="9c4f8-130">Se você planeja suportar o IE11 em suas WebParts do SPFx, o processo a seguir descreve as etapas necessárias para garantir a compatibilidade entre navegadores:</span><span class="sxs-lookup"><span data-stu-id="9c4f8-130">If you plan to support IE11 in your SPFx webparts, the following process describes the necessary steps to ensure cross-browser compatibility:</span></span> 

1. <span data-ttu-id="9c4f8-131">Instale os seguintes pacotes:</span><span class="sxs-lookup"><span data-stu-id="9c4f8-131">Install the following packages:</span></span>
```cmd
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
npm install @microsoft/mgt
```

2. <span data-ttu-id="9c4f8-132">Insira o seguinte config no gulpfile.js logo acima do build.initialze (Gulp);</span><span class="sxs-lookup"><span data-stu-id="9c4f8-132">Insert the following config in your gulpfile.js just above your build.initialze(gulp);</span></span>
```ts
build.configureWebpack.mergeConfig({
  additionalConfiguration: (generatedConfiguration) => {
    generatedConfiguration.module.rules.push(
      {
        test: /\.m?js$/, use:
        {
          loader: "babel-loader",
          options:
          {
            presets: [["@babel/preset-env",
              {
                targets: {
                  "ie": "11"
                }
              }]]
          }
        }
      }
    );

    return generatedConfiguration;
  }
});
```


3. <span data-ttu-id="9c4f8-133">No arquivo \* WebPart. TS, importe os seguintes metapreenchimentos antes da importação dos provedores</span><span class="sxs-lookup"><span data-stu-id="9c4f8-133">In your \*WebPart.ts file, import the following polyfills before import of the providers</span></span>
```ts
import 'regenerator-runtime/runtime';
import 'core-js/es/number';
import 'core-js/es/math';
import 'core-js/es/string';
import 'core-js/es/date';
import 'core-js/es/array';
import 'core-js/es/regexp';
import '@webcomponents/webcomponentsjs/webcomponents-bundle.js';
```

<span data-ttu-id="9c4f8-134">Para saber mais, confira [SharePoint Provider](./providers/sharepoint.md).</span><span class="sxs-lookup"><span data-stu-id="9c4f8-134">To learn more, see [sharepoint provider](./providers/sharepoint.md).</span></span>

## <a name="using-the-components-with-react-angular-and-other-frameworks"></a><span data-ttu-id="9c4f8-135">Usando os componentes com reagir, angular e outras estruturas</span><span class="sxs-lookup"><span data-stu-id="9c4f8-135">Using the components with React, Angular, and other frameworks</span></span>

<span data-ttu-id="9c4f8-136">Os componentes Web são baseados em vários padrões da Web e podem ser usados com qualquer estrutura que você já esteja usando.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-136">Web components are based on several web standards and can be used with any framework you're already using.</span></span> <span data-ttu-id="9c4f8-137">No entanto, nem todas as estruturas lidam com os componentes da Web da mesma maneira.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-137">However, not all frameworks handle web components the same way.</span></span> <span data-ttu-id="9c4f8-138">Para saber mais sobre as considerações que podem ser aplicadas dependendo da sua estrutura, confira o projeto [elementos personalizados em qualquer lugar](https://custom-elements-everywhere.com/) .</span><span class="sxs-lookup"><span data-stu-id="9c4f8-138">To learn more about the considerations that might apply depending on your framework, see the [Custom Elements Everywhere](https://custom-elements-everywhere.com/) project.</span></span>

<span data-ttu-id="9c4f8-139">As seções a seguir fornecem uma visão geral rápida do uso dos componentes do Microsoft Graph Toolkit com reagir e angulares.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-139">The following sections provide a quick overview of using the Microsoft Graph Toolkit components with React and Angular.</span></span>

### <a name="react"></a><span data-ttu-id="9c4f8-140">React</span><span class="sxs-lookup"><span data-stu-id="9c4f8-140">React</span></span>

<span data-ttu-id="9c4f8-141">Reagir transfere todos os dados para elementos personalizados na forma de atributos HTML.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-141">React passes all data to Custom Elements in the form of HTML attributes.</span></span> <span data-ttu-id="9c4f8-142">Para dados primitivos, isso é bom, mas não funciona ao transmitir dados ricos, como objetos ou matrizes.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-142">For primitive data this is fine, but it does not work when passing rich data, like objects or arrays.</span></span> <span data-ttu-id="9c4f8-143">Nesses casos, você precisará usar um `ref` para passar no objeto.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-143">In those cases you will need to use a `ref` to pass in the object.</span></span>

<span data-ttu-id="9c4f8-144">Ex</span><span class="sxs-lookup"><span data-stu-id="9c4f8-144">Ex:</span></span>

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

<span data-ttu-id="9c4f8-145">Como reagir implementa seu próprio sistema de eventos sintético, ele não pode escutar eventos DOM provenientes de elementos personalizados sem o uso de uma solução alternativa.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-145">Because React implements its own synthetic event system, it cannot listen for DOM events coming from custom elements without the use of a workaround.</span></span> <span data-ttu-id="9c4f8-146">Você precisará usar um `ref` para fazer referência aos componentes do kit de ferramentas e anexar manualmente ouvintes de eventos com addEventListener, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-146">You will need to use a `ref` to reference the toolkit components and manually attach event listeners with addEventListener, as shown in the following example.</span></span>

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

#### <a name="react-typescript-and-tsx"></a><span data-ttu-id="9c4f8-147">Reagir, typescript e TSX</span><span class="sxs-lookup"><span data-stu-id="9c4f8-147">React, Typescript, and TSX</span></span>

<span data-ttu-id="9c4f8-148">Um problema conhecido pode ocorrer quando você usa elementos personalizados com reagir e typescript.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-148">A known issue can occur when you use custom elements with React and Typescript.</span></span> <span data-ttu-id="9c4f8-149">O typescript gerará um erro ao tentar usar um componente no TSX.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-149">Typescript will throw an error when trying to use a component in tsx.</span></span> <span data-ttu-id="9c4f8-150">A solução alternativa é definir o elemento personalizado em seu código, conforme mostrado.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-150">The workaround is to define the custom element in your code, as shown.</span></span>

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

<span data-ttu-id="9c4f8-151">Você pode usá-lo no seu TSX como `<mgt-login></mgt-login>` .</span><span class="sxs-lookup"><span data-stu-id="9c4f8-151">You can then use it in your tsx as `<mgt-login></mgt-login>`.</span></span>

### <a name="angular"></a><span data-ttu-id="9c4f8-152">Angular</span><span class="sxs-lookup"><span data-stu-id="9c4f8-152">Angular</span></span>

<span data-ttu-id="9c4f8-153">A sintaxe de associação padrão do angular sempre definirá Propriedades em um elemento.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-153">Angular's default binding syntax will always set properties on an element.</span></span> <span data-ttu-id="9c4f8-154">Isso funciona bem para dados ricos, como objetos e matrizes, e também funciona bem para valores primitivos.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-154">This works well for rich data, like objects and arrays, and also works well for primitive values.</span></span>

<span data-ttu-id="9c4f8-155">Para usar elementos personalizados, primeiro, habilite os elementos personalizados em seu `app.module.ts` adicionando o `CUSTOM_ELEMENT_SCHEMA` ao `@NgModule() decorator` , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-155">To use custom elements, first, enable custom elements in your `app.module.ts` by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator`, as shown in the following example.</span></span>

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

<span data-ttu-id="9c4f8-156">Você pode importar o componente que gostaria de usar em seu \* arquivo Component. TS.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-156">You can then import the component you'd like to use in your component \*.ts file.</span></span>

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

<span data-ttu-id="9c4f8-157">Por fim, use o componente como faria normalmente no seu modelo.</span><span class="sxs-lookup"><span data-stu-id="9c4f8-157">Finally, use the component as you normally would in your template.</span></span>

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```

