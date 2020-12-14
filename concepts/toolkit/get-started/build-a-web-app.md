---
title: Criar um aplicativo Web com o kit de ferramentas do Microsoft Graph
description: Introdução à criação de um aplicativo Web usando o Microsoft Graph Toolkit.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 73e61e9d2c1c453ec67e61dce1f088b5119d1e8d
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664013"
---
# <a name="build-a-web-application-with-the-microsoft-graph-toolkit"></a>Criar um aplicativo Web com o kit de ferramentas do Microsoft Graph

Este tópico descreve como começar a usar o kit de ferramentas do Microsoft Graph em um aplicativo Web escrito no JavaScript da baunilha. Se quiser saber como usar o kit de ferramentas com uma estrutura da Web, consulte [compilar um aplicativo Web (reagir)](./use-toolkit-with-react.md) ou [compilar um aplicativo Web (angular)](./use-toolkit-with-angular.md).

Introdução ao Microsoft Graph Toolkit envolve as seguintes etapas:
1. Adicione o Microsoft Graph Toolkit ao seu projeto.
2. Inicialize o provedor MSAL.
3. Adicionar componentes.
4. Teste seu aplicativo.

## <a name="add-the-microsoft-graph-toolkit-to-your-project"></a>Adicionar o Microsoft Graph Toolkit ao seu projeto
Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote NPM.

# <a name="unpkg"></a>[unpkg](#tab/html)
Para usar o kit de ferramentas via gerenciamento-Loader, adicione a referência em um script ao seu código:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```
# <a name="npm"></a>[npm](#tab/npm)
O uso do kit de ferramentas por meio de módulos ES6 fornecerá controle total do processo de agrupamento e permitirá que você reúna apenas o código necessário para o aplicativo. Para usar os módulos ES6, adicione o pacote NPM ao seu projeto:

```cmd
npm install @microsoft/mgt
```

---


> **Observação**: se você estiver direcionando um navegador como o IE11 que não ofereça suporte a componentes da Web nativamente, talvez seja necessário [incluir polipreenchimentos](./overview.md#polyfills).

## <a name="initialize-the-msal-provider"></a>Inicializar o provedor MSAL
Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para os componentes. Para saber mais, consulte [usando os provedores](../providers/providers.md). O [provedor MSAL](../providers/msal.md) usa MSAL.js para entrar em usuários e adquirir tokens. Você pode inicializar o provedor MSAL no HTML ou no JavaScript.

Se quiser usar sua própria autenticação de backend, use o provedor de [proxy](../providers/proxy.md) no lugar do provedor MSAL.

Você pode optar por inicializar o provedor em seu código HTML ou JavaScript. 

# <a name="html"></a>[formato](#tab/HTML)
Adicione o `mgt-msal-provider` componente à sua página HTML e defina o `client-id` como seu cliente de aplicativo-ID.

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID"></mgt-msal-provider>
```
# <a name="js"></a>[JS](#tab/JavaScript)
Para inicializar o provedor MSAL em seu JavaScript, adicione o seguinte código ao aplicativo:

```js
import {Providers, MsalProvider} from '@microsoft/mgt'

Providers.globalProvider = new MsalProvider({
    clientId: "<YOUR_CLIENT_ID>"
})
```

---


A ID do cliente é a única propriedade necessária para inicializar o provedor, mas você pode definir opções adicionais. Para obter a lista completa, consulte [MSAL Provider](../providers/msal.md).

### <a name="creating-an-appclient-id"></a>Criar uma ID de aplicativo/cliente
Para obter uma ID de cliente, você precisa [registrar seu aplicativo](./add-aad-app-registration.md) no Azure AD. 
>**Observação**: o MSAL só dá suporte ao fluxo implícito do OAuth. Certifique-se de habilitar o fluxo implícito em seu aplicativo no portal do Azure (não está habilitado por padrão). Em **autenticação**, encontre a seção **concessão implícita** e marque as caixas de seleção para **tokens de acesso** e **tokens de ID**. 

## <a name="add-components"></a>Adicionar componentes
Depois de inicializar o provedor do MSAL, você pode começar a usar qualquer um dos componentes do kit de ferramentas.

# <a name="html"></a>[formato](#tab/HTML)
Veja a seguir um exemplo de trabalho completo usando o adMSAL-Loader, o provedor do inicializado em HTML e o componente de logon:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```

Este é um exemplo usando os módulos ES6, o provedor MSAL inicializado em HTML e o componente de logon:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>

<mgt-login></mgt-login>
```
# <a name="js"></a>[JS](#tab/JavaScript)
Este é um exemplo usando os módulos ES6, o provedor MSAL inicializado no JavaScript e o componente de logon:

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

Se você está apenas começando e deseja jogar, é possível usar o [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no Visual Studio Code ou qualquer servidor de desenvolvimento leve semelhante. Baixe a extensão e abra o arquivo HTML usando o Live Server. 
> **Observação:** Certifique-se de que o **URI de redirecionamento** em seu registro de aplicativo está definido como a porta de localhost em que seu aplicativo está hospedado. Vá para o seu registro de aplicativo no [portal do Azure](https://portal.azure.com), clique em **autenticação** em gerenciar e adicione o **URI de redirecionamento** correto.

## <a name="next-steps"></a>Próximas etapas
- Confira este tutorial passo a passo sobre como [criar um aplicativo Web simples](https://developer.microsoft.com/microsoft-365/blogs/a-lap-around-microsoft-graph-toolkit-day-2-zero-to-hero/).
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).
- Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).