---
title: Criar um aplicativo Web com o microsoft Graph Toolkit
description: Começar a criar um aplicativo Web usando o microsoft Graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 5eed45974428a2c6daf47d02144741d937e12c91
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579897"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Criar um aplicativo Web com o microsoft Graph Toolkit

Este tópico descreve como começar a usar o microsoft Graph Toolkit em um aplicativo Web escrito em JavaScript de baunilha. Para obter um tutorial passo a passo, experimente o [módulo Introdução ao microsoft Graph Toolkit .](/learn/modules/msgraph-toolkit-intro/) Se você quiser aprender a usar o Toolkit com uma estrutura da Web, consulte [Build a web app (React) ou](./use-toolkit-with-react.md) Build a Web app [(Angular)](./use-toolkit-with-angular.md).

Começar com o microsoft Graph Toolkit envolve as seguintes etapas:
1. Adicione o Microsoft Graph Toolkit ao seu projeto.
2. Inicializar o Provedor MSAL 2.0.
3. Adicione componentes.
4. Teste seu aplicativo.

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>Adicionar o microsoft Graph Toolkit ao seu projeto
Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[npm](#tab/npm)
Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo. Para usar os módulos ES6, adicione o pacote npm ao seu projeto:

```cmd
npm install @microsoft/mgt
```

---


> **Observação**: se você estiver direcionando um navegador como o IE11 que não dá suporte a componentes web na verdade, talvez seja necessário incluir [polífilos](./overview.md#polyfills).

## <a name="initialize-the-msal-20-provider"></a>Inicializar o Provedor MSAL 2.0
Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). O [Provedor MSAL 2.0](../providers/msal2.md) usa o msal-browser para entrar nos usuários e adquirir tokens. Você pode inicializar esse provedor em seu HTML ou JavaScript.

> **Observação**: se você estiver usando o Provedor MSAL no momento e quiser atualizar para o Provedor MSAL 2.0, siga as etapas listadas [aqui](../providers/msal2.md#migrating-from-msal-provider-to-msal-2-provider).
Se você quiser usar sua própria autenticação de back-end, use o [Provedor de Proxy](../providers/proxy.md) no lugar do provedor MSAL 2.0.

Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript. 

# <a name="html"></a>[HTML](#tab/HTML)
Adicione o `mgt-msal2-provider` componente à sua página HTML e desmarcar o para o seu aplicativo `client-id` client-id.

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID"></mgt-msal2-provider>
```
# <a name="js"></a>[js](#tab/JavaScript)
Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao seu aplicativo:

```js
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais. Para ver a lista completa, consulte [Msal 2.0 Provider](../providers/msal2.md).

### <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente
Para obter uma ID do cliente, você precisa registrar [seu aplicativo](./add-aad-app-registration.md) no Azure AD. 

## <a name="add-components"></a>Adicionar componentes
Depois de inicializar o provedor MSAL 2.0, você pode começar a usar qualquer um dos Toolkit componentes.

# <a name="html"></a>[HTML](#tab/HTML)
Veja a seguir um exemplo de trabalho completo usando mgt-loader, o Provedor MSAL inicializado em HTML e o componente logon:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

Este é um exemplo usando os módulos ES6, o Provedor MSAL 2.0 inicializado em HTML e o componente logon:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[js](#tab/JavaScript)
Este é um exemplo usando os módulos ES6, o Provedor MSAL 2.0 inicializado em JavaScript e o componente logon:

```js
import {Providers, Msal2Provider} from '@microsoft/mgt'

Providers.globalProvider = new Msal2Provider({
    clientId: "<YOUR_CLIENT_ID>"
})

function component() {
    const element = document.createElement('div');
    element.innerHTML = '<mgt-login></mgt-login>'
    return element;
}

document.body.appendChild((component()));
```

---


## <a name="test-your-app"></a>Testar seu aplicativo

Para testar seu aplicativo, o MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação. 

Se você estiver apenas começando e quiser brincar, poderá usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Visual Studio Code ou qualquer servidor de desenvolvimento leve semelhante. Baixe a extensão e abra seu arquivo HTML usando o servidor ao vivo. 
> **Observação:** Certifique-se **de que o URI de** redirecionamento no registro do aplicativo está definido para a porta localhost em que seu aplicativo está hospedado. Vá para o registro do aplicativo no [portal do Azure,](https://portal.azure.com)clique em **Autenticação** em gerenciar e adicione o **URI de redirecionamento correto.**

## <a name="next-steps"></a>Próximas etapas
- Confira o [tutorial Introdução ao Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) passo a passo.
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).
- Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).
