---
title: Provedor de proxy
description: O provedor de proxy permite que você use sua própria autenticação do lado do servidor com o Microsoft Graph Toolkit.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c62718471c361cd9537bc8ee098c33e7b65830ec
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092250"
---
# <a name="proxy-provider"></a>Provedor de proxy

Ao usar o provedor de proxy, você pode usar sua autenticação de back-end (como o fluxo On-Behalf-Of da Auth2.0) para ligar o Microsoft Graph Toolkit roteamento de todas as chamadas para o Microsoft Graph por meio de seu próprio back-end.

Seu serviço back-end deve expor uma API que será chamada para cada chamada ao Microsoft Graph. Por exemplo, quando um componente tenta obter um recurso, o ProxyProvider chama sua API base e anexa esse recurso.

<pre>https://graph.microsoft.com/v1.0/me => https://myurl.com/api/GraphProxy/v1.0/me</pre> 

A implementação da API deve chamar o Microsoft Graph em nome do usuário e retornar os resultados para o componente.

Para um exemplo de implementação, consulte o [exemplo ASP.NET MVC.](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/proxy-provider-asp-net-mvc) 

Para saber mais sobre provedores de autenticação, consulte [provedores.](./providers.md)

## <a name="get-started"></a>Introdução

Você pode inicializar o provedor de proxy em HTML ou JavaScript. Você deve fazer isso apenas uma vez por página.

### <a name="initialize-in-your-html-page"></a>Inicializar em sua página HTML

Inicializar o provedor de proxy em HTML é a maneira mais simples de definir sua própria rota para autenticação personalizada do lado do servidor. Use o `mgt-proxy-provider` componente para definir o **graph-proxy-url**. Isso definirá o provedor de proxy definido como o provedor global.

```html
<mgt-proxy-provider graph-proxy-url="https://myurl.com/api/GraphProxy"></mgt-proxy-provider>
```

| Atributo | Descrição |
| --- | --- |
| graph-proxy-url  | URL base para a API de proxy. |


### <a name="initialize-in-javascript"></a>Inicializar em JavaScript

Você pode fornecer mais opções inicializando o provedor em JavaScript.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy");
```

Opcionalmente, você pode enviar outros headers com cada solicitação para sua api de proxy usando uma função opcional como o segundo parâmetro no construtor.

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

Providers.globalProvider = new ProxyProvider("https://myurl.com/api/GraphProxy", async () => {
  return {
    header: 'value',
    header2: 'value2'
  };
);
```

Isso é útil quando você precisa passar tokens ou outros headers para seu back-end.

Se você for usar o `mgt-login` componente, também deverá especificar as `login` funções e `logout` o provedor:

```ts
import {Providers, ProxyProvider} from '@microsoft/mgt';

let provider = new ProxyProvider("https://myurl.com/api/GraphProxy");
provider.login = () => { /* will be called when "Sign In" is clicked */ };
provider.logout = () => { /* will be called when "Sign Out" is called */ };

Providers.globalProvider = provider;
```

