---
title: Criar um aplicativo Web com o microsoft Graph Toolkit
description: Introdução criar um aplicativo Web usando o microsoft Graph Toolkit.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: e464f822f6c08c51443ac24b482c99081954acf7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589006"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Criar um aplicativo Web com o microsoft Graph Toolkit

Este tópico descreve como começar a usar o microsoft Graph Toolkit em um aplicativo Web escrito em JavaScript de baunilha. Para um tutorial passo a passo, experimente o Introdução [com o módulo Graph Toolkit Microsoft](/learn/modules/msgraph-toolkit-intro/). Se você quiser aprender a usar o Toolkit com uma estrutura da Web, consulte [Build a web app (React)](./use-toolkit-with-react.md) ou [Build a Web app (Angular)](./use-toolkit-with-angular.md).

Começar com o microsoft Graph Toolkit envolve as seguintes etapas:
1. Adicione o Microsoft Graph Toolkit ao seu projeto.
2. Inicializar o Provedor MSAL2.
3. Adicione os componentes.
4. Teste seu aplicativo.

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>Adicionar o Microsoft Graph Toolkit ao seu projeto
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

## <a name="initialize-the-msal2-provider"></a>Inicializar o provedor MSAL2
Os provedores do Kit de ferramentas do Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). O [Provedor MSAL2](../providers/msal2.md) usa o msal-browser para entrar nos usuários e adquirir tokens. Você pode inicializar esse provedor em seu HTML ou JavaScript.

> **Observação**: se você estiver usando o Provedor MSAL no momento e quiser atualizar para o Provedor MSAL2, siga as etapas [listadas aqui](../providers/msal2.md#migrating-from-msal-provider-to-msal2-provider).
Se você quiser usar sua própria autenticação de back-end, use o [Provedor de Proxy](../providers/proxy.md) no lugar do Provedor MSAL2.

Você pode optar por inicializar o provedor em seu HTML ou no código JavaScript. 

# <a name="html"></a>[HTML](#tab/HTML)
Adicione o `mgt-msal2-provider` componente à sua página HTML e desmarcar o `client-id` para o seu aplicativo client-id.

```html
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
```
# <a name="javascript"></a>[JavaScript](#tab/JavaScript)
Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao seu aplicativo:

```javascript
import { Providers, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});
```

---

A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais. Para ver a lista completa, consulte [Provedor MSAL2](../providers/msal2.md).

### <a name="creating-an-appclient-id"></a>Criando uma ID de aplicativo/cliente
Para obter uma ID do cliente, você precisa registrar [seu aplicativo](./add-aad-app-registration.md) no Azure AD.

## <a name="add-components"></a>Adicionar os componentes
Depois de inicializar o provedor MSAL2, você pode começar a usar qualquer um dos componentes Toolkit.

# <a name="html"></a>[HTML](#tab/HTML)
Veja a seguir um exemplo de trabalho completo usando mgt-loader, o Provedor MSAL2 inicializado em HTML e o componente logon:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

Este é um exemplo usando os módulos ES6, o Provedor MSAL2 inicializado em HTML e o componente logon:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>
<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)
Este é um exemplo usando os módulos ES6, o Provedor MSAL2 inicializado em JavaScript e o componente logon:

```javascript
import { Providers, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});

function component() {
  const element = document.createElement('div');
  element.innerHTML = '<mgt-login></mgt-login>';
  return element;
}

document.body.appendChild(component());
```

---

## <a name="test-your-app"></a>Testar seu aplicativo

Para testar seu aplicativo, o MSAL exige que a página seja hospedada em um servidor Web para os redirecionamentos de autenticação. 

Se você estiver apenas começando e quiser brincar, poderá usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) em Visual Studio Code ou em qualquer servidor de desenvolvimento leve semelhante. Baixe a extensão e abra seu arquivo HTML usando o servidor ao vivo.
> **Observação:** Certifique-se **de que o URI de** redirecionamento no registro do aplicativo está definido para a porta localhost em que seu aplicativo está hospedado. Vá para o registro do aplicativo no [portal do Azure](https://portal.azure.com), clique em **Autenticação** em gerenciar e adicione o **URI de redirecionamento correto**.

## <a name="track-a-users-sign-in-state"></a>Rastrear o estado de login de um usuário

Você pode detectar quando um usuário se inscreveu com êxito e exibiu componentes específicos de acordo. Por exemplo, exibe o componente de agenda se o usuário tiver se assinado. Caso contrário, exibe a interface de login.

Para inspecionar corretamente o estado de login do usuário, adicione um manipulador de eventos ao `providerUpdated` evento usando a `Providers.onProviderUpdated` função. No manipulador, verifique o estado do provedor armazenado na `Providers.globalProvider.state` propriedade.

# <a name="html"></a>[HTML](#tab/HTML)

Se você estiver usando a biblioteca `mgt-loader` , poderá acessar e `Provider` `ProviderState` a partir da propriedade global `mgt` .

```html
<!DOCTYPE html>
<html>
<head>
  <script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
</head>
<body>
  <mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
  <div id="main">
    <mgt-login></mgt-login>
  </div>
  <script>
    const loadAgenda = () => {
      if (mgt.Providers.globalProvider.state === mgt.ProviderState.SignedIn) {
        document.getElementById('main').innerHTML = '<mgt-agenda></mgt-agenda>';
      }
    }
    mgt.Providers.onProviderUpdated(loadAgenda);
  </script>
</body>
</html>
```

# <a name="javascript"></a>[JavaScript](#tab/JavaScript)

Se você estiver usando o kit de ferramentas por meio dos pacotes npm, poderá importar o `Provider` e `ProviderState` de `@microsoft/mgt`.

```javascript
import { Providers, ProviderState, Msal2Provider } from '@microsoft/mgt';

Providers.globalProvider = new Msal2Provider({
  clientId: "<YOUR_CLIENT_ID>"
});

const loadAgenda = () => {
  if (Providers.globalProvider.state === ProviderState.SignedIn) {
    document.getElementById('main').innerHTML = '<mgt-agenda></mgt-agenda>';
  }
};

Providers.onProviderUpdated(loadAgenda);
```

---

## <a name="next-steps"></a>Próximas etapas

- Confira o tutorial [Introdução com o Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/) passo a passo.
- Experimente os componentes do [playground](https://mgt.dev).
- Faça uma pergunta no [Stack Overflow](https://aka.ms/mgt-question).
- Relate bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).
