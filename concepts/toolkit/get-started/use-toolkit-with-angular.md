---
title: Use o microsoft Graph Toolkit com Angular
description: Introdução usando o microsoft Graph Toolkit em um Angular aplicativo.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 9131fa4a1e161c93983fea3d615ebd1fc78bf0b7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588754"
---
# <a name="use-the-microsoft-graph-toolkit-with-angular"></a>Use o microsoft Graph Toolkit com Angular

Os Graph Toolkit da Microsoft funcionam muito bem com estruturas da Web, como Angular além de JavaScript e HTML de baunilha. Este tópico descreve como usar o microsoft Graph Toolkit com Angular. Para um passo a passo passo que descreve como criar um novo aplicativo Angular e usar o Microsoft Graph Toolkit, consulte [Using Microsoft Graph Toolkit with Angular](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o microsoft Graph Toolkit

Primeiro, você precisa habilitar elementos personalizados em seu aplicativo Angular adicionando `CUSTOM_ELEMENT_SCHEMA` o ao `@NgModule() decorator` em `app.module.ts`. O exemplo a seguir mostra como fazer isso:
```TypeScript
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
Em seguida, adicione o microsoft Graph Toolkit ao seu projeto instalando o pacote npm com:
```Command Line
npm install @microsoft/mgt
```
## <a name="initialize-a-provider"></a>Inicializar um provedor

Os provedores do Kit de ferramentas do Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). O provedor usado depende do contexto no qual sua solução será usada.

O exemplo a seguir mostra como adicionar o [Provedor MSAL2](../providers/msal2.md), mas você pode seguir o mesmo modelo com qualquer um dos provedores.
>[!NOTE] 
>Se você estiver usando o Provedor MSAL no momento e quiser atualizar para o Provedor MSAL2, siga as etapas no artigo provedor [MSAL2](../providers/msal2.md#migrating-from-msal-provider-to-msal2-provider) .

Import the provider and set it to initialize when the application initializes. Substitua `<YOUR-CLIENT-ID>` pela ID do cliente para seu aplicativo.

```TypeScript
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
### <a name="create-an-appclient-id"></a>Criar uma ID de aplicativo/cliente
Para obter uma ID do cliente, você precisa registrar [seu aplicativo](../../auth-register-app-v2.md) no Azure AD. 

## <a name="add-components"></a>Adicionar os componentes

Agora, você pode usar qualquer um dos componentes do Microsoft Graph Toolkit como faria normalmente em seus modelos HTML. Por exemplo, para adicionar o [componente Person](../components/person.md), adicione o seguinte ao seu modelo:

```html
<mgt-person person-query="me" view="twolines"></mgt-person>
```

## <a name="customizing-components-with-angular"></a>Personalização de componentes com Angular

Todos os Graph Toolkit microsoft [suportam modelos personalizados](../customize-components/templates.md), que permitem modificar o conteúdo de um componente. A sintaxe padrão para personalizar os componentes é usar chaves duplas para se referir aos dados de propriedade de cada um dos itens retornados, conforme mostrado:

```html
<!-- Double braces are used for data binding in Angular. This will throw an error. -->
<mgt-agenda>
    <template data-type="event">
        <div>{{event.subject}}</div>
    </template>
</mgt-agenda>
```

No Angular, no entanto, chaves duplas são usadas para vinculação de dados e o compilador Angular lançará um erro se você tentar usar a sintaxe de chave dupla.

Você pode evitar esses erros alterando os caracteres padrão usados pela Toolkit para algo diferente de chaves duplas usando o `TemplateHelper`. É melhor fazer isso em seu componente de aplicativo de nível superior para que ele se aplique globalmente.

Importe e `TemplateHelper` use o método `.setBindingSyntax()` para definir sua sintaxe de associação personalizada.

```TypeScript
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
Agora, você pode usar sua sintaxe de associação personalizada para definir modelos personalizados.

```html
<mgt-agenda>
    <template data-type="event">
        <div>[[event.subject]]</div>
    </template>
</mgt-agenda>
```

## <a name="next-steps"></a>Próximas etapas
- Confira este tutorial passo a passo sobre como [criar um Angular app](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-14-using-microsoft-graph-toolkit-with-angular/).
- Experimente os componentes do [playground](https://mgt.dev).
- Faça uma pergunta no [Stack Overflow](https://aka.ms/mgt-question).
- Relate bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).
