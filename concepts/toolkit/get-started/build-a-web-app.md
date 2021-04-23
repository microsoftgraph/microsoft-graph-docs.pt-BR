---
title: Criar um aplicativo Web com o Microsoft Graph Toolkit
description: Começar a criar um aplicativo Web usando o microsoft graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 974f6351bdce985089d93f607210c8eb47b902ba
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961349"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Criar um aplicativo Web com o Microsoft Graph Toolkit

Este tópico descreve como começar a usar o microsoft graph Toolkit em um aplicativo Web escrito em JavaScript de baunilha. Para obter um tutorial passo a passo, experimente o [módulo Introdução ao Microsoft Graph Toolkit .](/learn/modules/msgraph-toolkit-intro/) Se você quiser aprender a usar o Toolkit com uma estrutura da Web, consulte [Build a Web app (React)](./use-toolkit-with-react.md) ou Build a Web app [(Angular)](./use-toolkit-with-angular.md).

Começar a trabalhar com o Microsoft Graph Toolkit as seguintes etapas:
1. Adicione o Microsoft Graph Toolkit ao seu projeto.
2. Inicializar o Provedor MSAL.
3. Adicione componentes.
4. Teste seu aplicativo.

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>Adicionar o microsoft graph Toolkit ao seu projeto
Você pode usar o microsoft graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (por meio de unpkg) ou instalando o pacote npm.

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

## <a name="initialize-the-msal-provider"></a>Inicializar o provedor MSAL
Os provedores Toolkit Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). O [Provedor MSAL](../providers/msal.md) usa MSAL.js para entrar em usuários e adquirir tokens. Você pode inicializar o provedor MSAL em seu HTML ou JavaScript.

Se você quiser usar sua própria autenticação de back-end, use o [Provedor de Proxy](../providers/proxy.md) no lugar do provedor MSAL.

Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript. 

# <a name="html"></a>[HTML](#tab/HTML)
Adicione o `mgt-msal-provider` componente à sua página HTML e desmarcar o para o seu aplicativo `client-id` client-id.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[js](#tab/JavaScript)
Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao seu aplicativo:

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais. Para ver a lista completa, consulte [Msal Provider](../providers/msal.md).

### <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente
Para obter uma ID do cliente, você precisa registrar [seu aplicativo](./add-aad-app-registration.md) no Azure AD. 
>**Observação**: O MSAL só dá suporte ao Fluxo Implícito para OAuth. Certifique-se de habilitar o Fluxo Implícito em seu aplicativo no Portal do Azure (ele não está habilitado por padrão). Em **Autenticação**, encontre a seção **Concessão implícita** e selecione as caixas de seleção para **tokens de Acesso** e **tokens de ID**. 

## <a name="add-components"></a>Adicionar componentes
Depois de inicializar o provedor MSAL, você pode começar a usar qualquer um dos componentes Toolkit de dados.

# <a name="html"></a>[HTML](#tab/HTML)
Veja a seguir um exemplo de trabalho completo usando mgt-loader, o Provedor MSAL inicializado em HTML e o componente logon:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

Este é um exemplo usando os módulos ES6, o Provedor MSAL inicializado em HTML e o componente logon:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[js](#tab/JavaScript)
Este é um exemplo usando os módulos ES6, o Provedor MSAL inicializado em JavaScript e o componente logon:

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
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

Se você estiver apenas começando e quiser brincar, pode usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no código Visual Studio ou em qualquer servidor de desenvolvimento leve semelhante. Baixe a extensão e abra seu arquivo HTML usando o servidor ao vivo. 
> **Observação:** Certifique-se **de que o URI de** redirecionamento no registro do aplicativo está definido para a porta localhost em que seu aplicativo está hospedado. Vá para o registro do aplicativo no [portal do Azure,](https://portal.azure.com)clique em **Autenticação** em gerenciar e adicione o **URI de redirecionamento correto.**

## <a name="next-steps"></a>Próximas Etapas
- Confira o [tutorial Introdução ao Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) passo a passo.
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).
- Relatar bugs ou deixar uma solicitação de recurso [no GitHub](https://aka.ms/mgt).
