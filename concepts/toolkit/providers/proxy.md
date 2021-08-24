---
title: Provedor de proxy
description: O provedor de proxy permite que você use sua própria autenticação do lado do servidor com o microsoft Graph Toolkit.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9ce4a1def59a6bfa5dc8031f7ae1bcfd93c593ab
ms.sourcegitcommit: c6f7a931a8d83ac54f577b7bec08237fd17ce51a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2021
ms.locfileid: "58490389"
---
# <a name="proxy-provider"></a>Provedor de proxy

Ao usar o provedor de proxy, você pode usar sua autenticação back-end (como fluxo Auth2.0 On-Behalf-Of) para ligar o Microsoft Graph Toolkit roteamento de todas as chamadas para o Microsoft Graph por meio de seu próprio back-end.

Seu serviço back-end deve expor uma API que será chamada para todas as chamadas para o Microsoft Graph. Por exemplo, quando um componente tenta obter um recurso, o ProxyProvider chamará sua API base e anexará esse recurso.

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

Sua implementação de API deve chamar a Microsoft Graph em nome do usuário e retornar os resultados para o componente.

Para um exemplo de implementação, consulte o [exemplo ASP.NET MVC](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc). 

Para saber mais sobre provedores de autenticação, consulte [provedores](./providers.md).

## <a name="get-started"></a>Introdução

Você pode inicializar o provedor proxy em HTML ou JavaScript. Você deve fazer isso apenas uma vez por página.

### <a name="initialize-in-your-html-page"></a>Inicializar em sua página HTML

Inicializar o provedor proxy em HTML é a maneira mais simples de definir sua própria rota para autenticação personalizada do lado do servidor. Use o `mgt-proxy-provider` componente para definir o **graph-proxy-url**. Isso definirá o provedor de proxy definido como o provedor global.

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| Atributo | Descrição |
| --- | --- |
| graph-proxy-url  | URL base para a API proxy. |


### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Você pode fornecer mais opções inicializando o provedor em JavaScript.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

Opcionalmente, você pode enviar headers adicionais com cada solicitação para sua api proxy usando uma função opcional como o segundo parâmetro no construtor.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
});
```

Isso é útil quando você precisa passar tokens ou outros headers para seu back-end.

Se você estiver usando o componente, também deverá especificar `mgt-login` as funções e para o `login` `logout` provedor:

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

