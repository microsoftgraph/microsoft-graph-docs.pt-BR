---
title: Provedor de proxy
description: O provedor de proxy permite que você use sua própria autenticação do lado do servidor com o Microsoft Graph Toolkit.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ab52ed5c1d3af2cb0dfb99e086245a5b33aa9908
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657882"
---
# <a name="proxy-provider"></a>Provedor de proxy

Quando você usa o provedor de proxy, é possível usar a autenticação de backend (como o fluxo de autenticação em nome de 2.0) para alimentar o Microsoft Graph Toolkit encaminhando todas as chamadas para o Microsoft Graph através do seu próprio backend.

Seu serviço de back-end deve expor uma API que será chamada para cada chamada para o Microsoft Graph. Por exemplo, quando um componente tenta obter um recurso, o Proxyprovider chamará sua API base e acrescentará esse recurso.

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

A implementação da API deve chamar o Microsoft Graph em nome do usuário e retornar os resultados para o componente.

Para obter um exemplo de implementação, consulte o [exemplo MVC do ASP.net](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc). 

Para saber mais sobre provedores de autenticação, consulte [Providers](./providers.md).

## <a name="get-started"></a>Introdução

Você pode inicializar o provedor de proxy no HTML ou no JavaScript. Você deve fazer isso apenas uma vez por página.

### <a name="initialize-in-your-html-page"></a>Inicializar na página HTML

Inicializar o provedor de proxy em HTML é a maneira mais simples de definir sua própria rota para autenticação personalizada no servidor. Use o `mgt-proxy-provider` componente para definir o **gráfico-proxy-URL**. Isso definirá o provedor de proxy definido como o provedor global.

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| Atributo | Descrição |
| --- | --- |
| gráfico-proxy-URL  | URL base para a API de proxy. |


### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Você pode fornecer mais opções inicializando o provedor no JavaScript.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

Opcionalmente, você pode enviar cabeçalhos adicionais com cada solicitação para a API de proxy usando uma função opcional como o segundo parâmetro no construtor.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

Isso é útil quando você precisa passar tokens ou outros cabeçalhos para o back-end

Se você estiver usando o `mgt-login` componente, também deverá especificar as `login` `logout` funções e para o provedor:

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt'

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

