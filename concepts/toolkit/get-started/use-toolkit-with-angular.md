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
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>Usar o kit de ferramentas do Microsoft Graph com angular

Os componentes do kit de ferramentas do Microsoft Graph funcionam bem com estruturas da Web como angulares, além de JavaScript e HTML. Este tópico descreve como usar o kit de ferramentas do Microsoft Graph com angular. Para obter instruções passo a passo que descrevem como criar um novo aplicativo angular e usar o Microsoft Graph Toolkit, consulte [usando o Microsoft Graph Toolkit com angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o Microsoft Graph Toolkit

Primeiro, você precisa habilitar elementos personalizados no seu aplicativo angular adicionando o `CUSTOM_ELEMENT_SCHEMA` ao `@NgModule() decorator` `app.module.ts` . O exemplo a seguir mostra como fazer isso:
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
Em seguida, adicione o Microsoft Graph Toolkit ao seu projeto instalando o pacote do NPM com:
```bash
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>Inicializar um provedor

Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para os componentes. Para saber mais, consulte [usando os provedores](../providers/providers.md). O provedor que você usa depende do contexto no qual a solução será usada.

O exemplo a seguir mostra como adicionar o [provedor MSAL](../providers/msal.md), mas você pode seguir o mesmo modelo com qualquer um dos provedores. Importe o provedor e defina-o para ser inicializado quando o aplicativo for inicializado. Substitua `<YOUR-CLIENT-ID>` pela ID do cliente para seu aplicativo.

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
### <a name="create-an-appclient-id"></a>Criar uma ID de aplicativo/cliente
Para obter uma ID de cliente, você precisa [registrar seu aplicativo](../../auth-register-app-v2.md) no Azure AD. 
>**Observação**: o MSAL só dá suporte ao fluxo implícito do OAuth. Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão). Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**.

## <a name="add-components"></a>Adicionar componentes

Agora, você pode usar qualquer um dos componentes do Microsoft Graph Toolkit como faria normalmente em seus modelos HTML. Por exemplo, para adicionar o [componente pessoa](../components/person.md), adicione o seguinte ao modelo:

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>Personalizando componentes com o angular

Todos os componentes do Microsoft Graph Toolkit dão suporte a [modelos personalizados](../customize-components/templates.md), que permitem modificar o conteúdo de um componente. A sintaxe padrão para personalizar os componentes é usar chaves duplas para se referir aos dados de propriedade de cada um dos itens retornados, conforme mostrado:

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

No angular, no entanto, chaves duplas são usadas para associação de dados e o compilador angular apresentará um erro se você tentar usar a sintaxe de chave dupla.

Você pode evitar esses erros alterando os caracteres padrão usados pelo kit de ferramentas para algo diferente de chaves duplas usando o `TemplateHelper` . É melhor fazer isso no seu componente de aplicativo de nível superior para que se aplique globalmente.

Importe o `TemplateHelper` e use o `.setBindingSyntax()` método para definir sua sintaxe de associação personalizada.

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
Agora, você pode usar a sintaxe de associação personalizada para definir modelos personalizados.

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a>Próximas etapas
- Confira este tutorial passo a passo sobre a [criação de um aplicativo angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).
- Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).