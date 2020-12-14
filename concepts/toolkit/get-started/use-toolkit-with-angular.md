---
title: Usar o kit de ferramentas do Microsoft Graph com angular
description: Introdução ao uso do kit de ferramentas do Microsoft Graph em um aplicativo angular.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: a1c0ebc252545491dc57d8910eb283db6d227ccd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664041"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a><span data-ttu-id="4a1a8-103">Usar o kit de ferramentas do Microsoft Graph com angular</span><span class="sxs-lookup"><span data-stu-id="4a1a8-103">Use the Microsoft Graph Toolkit with Angular</span></span>

<span data-ttu-id="4a1a8-104">Os componentes do kit de ferramentas do Microsoft Graph funcionam bem com estruturas da Web como angulares, além de JavaScript e HTML.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-104">Microsoft Graph Toolkit components work great with web frameworks like Angular in addition to vanilla JavaScript and HTML.</span></span> <span data-ttu-id="4a1a8-105">Este tópico descreve como usar o kit de ferramentas do Microsoft Graph com angular.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-105">This topic describes how to use the Microsoft Graph Toolkit with Angular.</span></span> <span data-ttu-id="4a1a8-106">Para obter instruções passo a passo que descrevem como criar um novo aplicativo angular e usar o Microsoft Graph Toolkit, consulte [usando o Microsoft Graph Toolkit com angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span><span class="sxs-lookup"><span data-stu-id="4a1a8-106">For a step-by-step walkthrough that describes how to create a new Angular application and use the Microsoft Graph Toolkit, see [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="4a1a8-107">Adicionar o Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="4a1a8-107">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4a1a8-108">Primeiro, você precisa habilitar elementos personalizados no seu aplicativo angular adicionando o `CUSTOM_ELEMENT_SCHEMA` ao `@NgModule() decorator` `app.module.ts` .</span><span class="sxs-lookup"><span data-stu-id="4a1a8-108">First, you need to enable custom elements in your Angular application by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator` in `app.module.ts`.</span></span> <span data-ttu-id="4a1a8-109">O exemplo a seguir mostra como fazer isso:</span><span class="sxs-lookup"><span data-stu-id="4a1a8-109">The following example shows how to do this:</span></span>
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
<span data-ttu-id="4a1a8-110">Em seguida, adicione o Microsoft Graph Toolkit ao seu projeto instalando o pacote do NPM com:</span><span class="sxs-lookup"><span data-stu-id="4a1a8-110">Next, add the Microsoft Graph Toolkit to your project by installing the npm package with:</span></span>
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a><span data-ttu-id="4a1a8-111">Inicializar um provedor</span><span class="sxs-lookup"><span data-stu-id="4a1a8-111">Initialize a provider</span></span>

<span data-ttu-id="4a1a8-112">Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-112">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="4a1a8-113">Para saber mais, consulte [usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="4a1a8-113">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="4a1a8-114">O provedor que você usa depende do contexto no qual a solução será usada.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-114">The provider you use depends on the context in which your solution will be used.</span></span>

<span data-ttu-id="4a1a8-115">O exemplo a seguir mostra como adicionar o [provedor MSAL](../providers/msal.md), mas você pode seguir o mesmo modelo com qualquer um dos provedores.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-115">The following example shows how to add the [MSAL Provider](../providers/msal.md), but you can follow the same model with any of the providers.</span></span> <span data-ttu-id="4a1a8-116">Importe o provedor e defina-o para ser inicializado quando o aplicativo for inicializado.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-116">Import the provider and set it to initialize when the application initializes.</span></span> <span data-ttu-id="4a1a8-117">Substitua `<YOUR-CLIENT-ID>` pela ID do cliente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-117">Replace `<YOUR-CLIENT-ID>` with the client ID for your application.</span></span>

```ts
import { Component, OnInit } from '@angular/core';
import { Providers, MsalProvider } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new MsalProvider({
            clientId: '<YOUR-CLIENT-ID>'
        });
    }
}
```
### <a name="create-an-appclient-id"></a><span data-ttu-id="4a1a8-118">Criar uma ID de aplicativo/cliente</span><span class="sxs-lookup"><span data-stu-id="4a1a8-118">Create an app/client ID</span></span>
<span data-ttu-id="4a1a8-119">Para obter uma ID de cliente, você precisa [registrar seu aplicativo](../../auth-register-app-v2.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-119">In order to get a client ID, you need to [register your application](../../auth-register-app-v2.md) in Azure AD.</span></span> 
><span data-ttu-id="4a1a8-120">**Observação**: o MSAL só dá suporte ao fluxo implícito do OAuth.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-120">**Note**: MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="4a1a8-121">Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão).</span><span class="sxs-lookup"><span data-stu-id="4a1a8-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="4a1a8-122">Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>

## <a name="add-components"></a><span data-ttu-id="4a1a8-123">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="4a1a8-123">Add components</span></span>

<span data-ttu-id="4a1a8-124">Agora, você pode usar qualquer um dos componentes do Microsoft Graph Toolkit como faria normalmente em seus modelos HTML.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-124">Now, you can use any of the Microsoft Graph Toolkit components as you normally would in your HTML templates.</span></span> <span data-ttu-id="4a1a8-125">Por exemplo, para adicionar o [componente pessoa](../components/person.md), adicione o seguinte ao modelo:</span><span class="sxs-lookup"><span data-stu-id="4a1a8-125">For example, to add the [Person component](../components/person.md),  add the following to your template:</span></span>

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a><span data-ttu-id="4a1a8-126">Personalizando componentes com o angular</span><span class="sxs-lookup"><span data-stu-id="4a1a8-126">Customizing components with Angular</span></span>

<span data-ttu-id="4a1a8-127">Todos os componentes do Microsoft Graph Toolkit dão suporte a [modelos personalizados](../customize-components/templates.md), que permitem modificar o conteúdo de um componente.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-127">All Microsoft Graph Toolkit components support [custom templates](../customize-components/templates.md), which allow you to modify the content of a component.</span></span> <span data-ttu-id="4a1a8-128">A sintaxe padrão para personalizar os componentes é usar chaves duplas para se referir aos dados de propriedade de cada um dos itens retornados, conforme mostrado:</span><span class="sxs-lookup"><span data-stu-id="4a1a8-128">The default syntax for customizing the components is to use double braces to refer to the property data for each of the returned items, as shown:</span></span>

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

<span data-ttu-id="4a1a8-129">No angular, no entanto, chaves duplas são usadas para associação de dados e o compilador angular apresentará um erro se você tentar usar a sintaxe de chave dupla.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-129">In Angular, however, double braces are used for data binding and the Angular compiler will throw an error if you try to use the double brace syntax.</span></span>

<span data-ttu-id="4a1a8-130">Você pode evitar esses erros alterando os caracteres padrão usados pelo kit de ferramentas para algo diferente de chaves duplas usando o `TemplateHelper` .</span><span class="sxs-lookup"><span data-stu-id="4a1a8-130">You can avoid these errors by changing the default characters used by the Toolkit to something other than double braces by using the `TemplateHelper`.</span></span> <span data-ttu-id="4a1a8-131">É melhor fazer isso no seu componente de aplicativo de nível superior para que se aplique globalmente.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-131">It is best to do this in your top-level App component so that it applies globally.</span></span>

<span data-ttu-id="4a1a8-132">Importe o `TemplateHelper` e use o `.setBindingSyntax()` método para definir sua sintaxe de associação personalizada.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-132">Import the `TemplateHelper` and use the `.setBindingSyntax()` method to set your custom binding syntax.</span></span>

```ts
import { Component, OnInit } from '@angular/core';
import { Providers, MsalProvider, TemplateHelper } from '@microsoft/mgt';

@Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css']
})
export class AppComponent implements OnInit {

    ngOnInit()
    {
        Providers.globalProvider = new MsalProvider({ clientId: '<YOUR-CLIENT-ID>'})
        TemplateHelper.setBindingSyntax('[[',']]');
    }
}
```
<span data-ttu-id="4a1a8-133">Agora, você pode usar a sintaxe de associação personalizada para definir modelos personalizados.</span><span class="sxs-lookup"><span data-stu-id="4a1a8-133">Now, you can use your custom binding syntax to define custom templates.</span></span>

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a><span data-ttu-id="4a1a8-134">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4a1a8-134">Next steps</span></span>
- <span data-ttu-id="4a1a8-135">Confira este tutorial passo a passo sobre a [criação de um aplicativo angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span><span class="sxs-lookup"><span data-stu-id="4a1a8-135">Check out this step-by-step tutorial on [building an Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).</span></span>
- <span data-ttu-id="4a1a8-136">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="4a1a8-136">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="4a1a8-137">Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="4a1a8-137">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="4a1a8-138">Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="4a1a8-138">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>