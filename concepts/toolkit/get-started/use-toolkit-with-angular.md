---
title: Use o microsoft Graph Toolkit com Angular
description: Começar a usar o microsoft Graph Toolkit em um Angular aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 1390b29c94fef292433e1e422fa5c44fd480e1eb
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579883"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a><span data-ttu-id="d7672-103">Use o microsoft Graph Toolkit com Angular</span><span class="sxs-lookup"><span data-stu-id="d7672-103">Use the Microsoft Graph Toolkit with Angular</span></span>

<span data-ttu-id="d7672-104">Os Graph Toolkit da Microsoft funcionam muito bem com estruturas da Web, como Angular além de JavaScript e HTML de baunilha.</span><span class="sxs-lookup"><span data-stu-id="d7672-104">Microsoft Graph Toolkit components work great with web frameworks like Angular in addition to vanilla JavaScript and HTML.</span></span> <span data-ttu-id="d7672-105">Este tópico descreve como usar o microsoft Graph Toolkit com Angular.</span><span class="sxs-lookup"><span data-stu-id="d7672-105">This topic describes how to use the Microsoft Graph Toolkit with Angular.</span></span> <span data-ttu-id="d7672-106">Para um passo a passo passo que descreve como criar um novo aplicativo Angular e usar o Microsoft Graph Toolkit, consulte [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span><span class="sxs-lookup"><span data-stu-id="d7672-106">For a step-by-step walkthrough that describes how to create a new Angular application and use the Microsoft Graph Toolkit, see [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="d7672-107">Adicionar o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="d7672-107">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d7672-108">Primeiro, você precisa habilitar elementos personalizados em seu aplicativo Angular adicionando o `CUSTOM_ELEMENT_SCHEMA` ao `@NgModule() decorator` em `app.module.ts` .</span><span class="sxs-lookup"><span data-stu-id="d7672-108">First, you need to enable custom elements in your Angular application by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator` in `app.module.ts`.</span></span> <span data-ttu-id="d7672-109">O exemplo a seguir mostra como fazer isso:</span><span class="sxs-lookup"><span data-stu-id="d7672-109">The following example shows how to do this:</span></span>
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
<span data-ttu-id="d7672-110">Em seguida, adicione o microsoft Graph Toolkit ao seu projeto instalando o pacote npm com:</span><span class="sxs-lookup"><span data-stu-id="d7672-110">Next, add the Microsoft Graph Toolkit to your project by installing the npm package with:</span></span>
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a><span data-ttu-id="d7672-111">Inicializar um provedor</span><span class="sxs-lookup"><span data-stu-id="d7672-111">Initialize a provider</span></span>

<span data-ttu-id="d7672-112">Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="d7672-112">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="d7672-113">Para saber mais, confira [Usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="d7672-113">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="d7672-114">O provedor usado depende do contexto no qual sua solução será usada.</span><span class="sxs-lookup"><span data-stu-id="d7672-114">The provider you use depends on the context in which your solution will be used.</span></span>

<span data-ttu-id="d7672-115">O exemplo a seguir mostra como adicionar o [Provedor MSAL 2](../providers/msal2.md), mas você pode seguir o mesmo modelo com qualquer um dos provedores.</span><span class="sxs-lookup"><span data-stu-id="d7672-115">The following example shows how to add the [MSAL 2 Provider](../providers/msal2.md), but you can follow the same model with any of the providers.</span></span>
>[!NOTE] 
><span data-ttu-id="d7672-116">Se você estiver usando o Provedor MSAL no momento e quiser atualizar para o Provedor MSAL 2, siga as etapas no artigo do provedor [MSAL 2.](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider)</span><span class="sxs-lookup"><span data-stu-id="d7672-116">If you are currently using the MSAL Provider and would like to update to the MSAL 2 Provider, follow the steps in the [MSAL 2 provider](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider) article.</span></span>

<span data-ttu-id="d7672-117">Import the provider and set it to initialize when the application initializes.</span><span class="sxs-lookup"><span data-stu-id="d7672-117">Import the provider and set it to initialize when the application initializes.</span></span> <span data-ttu-id="d7672-118">Substitua `<YOUR-CLIENT-ID>` pela ID do cliente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d7672-118">Replace `<YOUR-CLIENT-ID>` with the client ID for your application.</span></span>

```ts
import { Component, OnInit } from '@angular/core';
import { Providers, Msal2Provider } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new Msal2Provider({
            clientId: '<YOUR-CLIENT-ID>'
        });
    }
}
```
### <a name="create-an-appclient-id"></a><span data-ttu-id="d7672-119">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="d7672-119">Create an app/client ID</span></span>
<span data-ttu-id="d7672-120">Para obter uma ID do cliente, você precisa registrar [seu aplicativo](../../auth-register-app-v2.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d7672-120">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 

## <a name="add-components"></a><span data-ttu-id="d7672-121">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="d7672-121">Add components</span></span>

<span data-ttu-id="d7672-122">Agora, você pode usar qualquer um dos componentes do Microsoft Graph Toolkit como faria normalmente em seus modelos HTML.</span><span class="sxs-lookup"><span data-stu-id="d7672-122">Now, you can use any of the Microsoft Graph Toolkit components as you normally would in your HTML templates.</span></span> <span data-ttu-id="d7672-123">Por exemplo, para adicionar o [componente Person](../components/person.md), adicione o seguinte ao seu modelo:</span><span class="sxs-lookup"><span data-stu-id="d7672-123">For example, to add the [Person component](../components/person.md),  add the following to your template:</span></span>

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a><span data-ttu-id="d7672-124">Personalização de componentes com Angular</span><span class="sxs-lookup"><span data-stu-id="d7672-124">Customizing components with Angular</span></span>

<span data-ttu-id="d7672-125">Todos os Graph Toolkit microsoft [suportam modelos personalizados](../customize-components/templates.md), que permitem modificar o conteúdo de um componente.</span><span class="sxs-lookup"><span data-stu-id="d7672-125">All Microsoft Graph Toolkit components support [custom templates](../customize-components/templates.md), which allow you to modify the content of a component.</span></span> <span data-ttu-id="d7672-126">A sintaxe padrão para personalizar os componentes é usar chaves duplas para se referir aos dados de propriedade de cada um dos itens retornados, conforme mostrado:</span><span class="sxs-lookup"><span data-stu-id="d7672-126">The default syntax for customizing the components is to use double braces to refer to the property data for each of the returned items, as shown:</span></span>

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

<span data-ttu-id="d7672-127">No Angular, no entanto, chaves duplas são usadas para vinculação de dados e o compilador Angular lançará um erro se você tentar usar a sintaxe de chave dupla.</span><span class="sxs-lookup"><span data-stu-id="d7672-127">In Angular, however, double braces are used for data binding and the Angular compiler will throw an error if you try to use the double brace syntax.</span></span>

<span data-ttu-id="d7672-128">Você pode evitar esses erros alterando os caracteres padrão usados pelo Toolkit para algo diferente de chaves duplas usando `TemplateHelper` o .</span><span class="sxs-lookup"><span data-stu-id="d7672-128">You can avoid these errors by changing the default characters used by the Toolkit to something other than double braces by using the `TemplateHelper`.</span></span> <span data-ttu-id="d7672-129">É melhor fazer isso em seu componente de aplicativo de nível superior para que ele se aplique globalmente.</span><span class="sxs-lookup"><span data-stu-id="d7672-129">It is best to do this in your top-level App component so that it applies globally.</span></span>

<span data-ttu-id="d7672-130">Importe e `TemplateHelper` use o método para definir sua sintaxe de associação `.setBindingSyntax()` personalizada.</span><span class="sxs-lookup"><span data-stu-id="d7672-130">Import the `TemplateHelper` and use the `.setBindingSyntax()` method to set your custom binding syntax.</span></span>

```ts
import { Component, OnInit } from '@angular/core';
import { Providers, Msal2Provider, TemplateHelper } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new Msal2Provider({ clientId: '<YOUR-CLIENT-ID>'})
        TemplateHelper.setBindingSyntax('[[',']]');
    }
}
```
<span data-ttu-id="d7672-131">Agora, você pode usar sua sintaxe de associação personalizada para definir modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="d7672-131">Now, you can use your custom binding syntax to define custom templates.</span></span>

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a><span data-ttu-id="d7672-132">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d7672-132">Next steps</span></span>
- <span data-ttu-id="d7672-133">Confira este tutorial passo a passo sobre como [criar um Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span><span class="sxs-lookup"><span data-stu-id="d7672-133">Check out this step-by-step tutorial on [building an Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>
- <span data-ttu-id="d7672-134">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="d7672-134">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="d7672-135">Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="d7672-135">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="d7672-136">Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="d7672-136">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
