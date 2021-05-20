---
title: Iniciando o microsoft Graph Toolkit
description: Começar a usar o microsoft Graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e84350a7835cac7914f5238110f74b3383047e13
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579589"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Iniciando o microsoft Graph Toolkit

Os componentes Graph Toolkit microsoft podem ser facilmente adicionados ao seu aplicativo Web, SharePoint Web Part ou Microsoft Teams guias. Os componentes são baseados em padrões web e podem ser usados em projetos JavaScript simples ou com estruturas da Web populares, como Reach, Angular, Vue.js e muito mais.

Você pode assistir a este vídeo curto para ver como é rápido e fácil começar com o Toolkit.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Para obter um tutorial passo a passo, consulte o [módulo Introdução ao microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/). 

## <a name="set-up-your-microsoft-365-tenant"></a>Configure o locatário do Microsoft 365.
Para desenvolver com o Toolkit, você precisa de acesso a um locatário Microsoft 365 locatário. Se você não tiver um, poderá obter uma assinatura de desenvolvedor gratuita Microsoft 365 in [joining the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program). Para obter detalhes sobre como configurar sua assinatura, consulte [Configurar uma assinatura Microsoft 365 desenvolvedor.](/office/developer-program/microsoft-365-developer-program-get-started)

## <a name="set-up-your-development-environment"></a>Defina seu ambiente de desenvolvimento
Para desenvolver com o Toolkit, você precisará de um editor de texto ou IDE. Você pode usar o editor ou o IDE de sua escolha ou instalar e [usar](https://code.visualstudio.com/download) Visual Studio Code gratuitamente. Você também precisará de um navegador da Web moderno como Microsoft Edge, Google Chrome ou Firefox. Você também precisará de uma versão LTS do Node.js, que pode ser instalada [nodejs.org](https://nodejs.org).

## <a name="using-the-microsoft-graph-toolkit"></a>Usando o microsoft Graph Toolkit
Você pode usar o microsoft Graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (via unpkg) ou instalando o pacote npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
Usar o Toolkit por meio de módulos ES6 dará a você controle total do processo de empacotamento e permitirá que você empacote apenas o código necessário para seu aplicativo. Para usar os módulos ES6, adicione o pacote npm ao seu projeto:

```cmd
npm install @microsoft/mgt
```
Agora você pode fazer referência a todos os componentes na página que está usando:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a>Pacotes NPM

O microsoft Graph Toolkit é feito de vários pacotes NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.

<b>@microsoft/mgt-element</b>

O `@microsoft/mgt-element` é o pacote principal que contém apenas as classes base usadas para criar componentes e provedores. Este pacote expõe todas as classes e interfaces necessárias necessárias para criar seus próprios componentes e exporta a interface IProvider e a [classe SimpleProvider](../providers/custom.md) para a criação de provedores personalizados.

<b>@microsoft/mgt-components</b>

O `@microsoft/mgt-components` pacote contém todos os Graph Da Microsoft conectados, como , e muito `Person` `PeoplePicker` mais. 

**Provedores**

Os provedores estão disponíveis por meio de um único pacote e podem ser instalados conforme necessário. Os seguintes pacotes de provedor estão disponíveis:

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` componente `mgt-msal-provider` e. O provedor MSAL usa msal.js para autenticação em aplicativos Web e PWAs (Progressive Web Apps).

- <b>@micosoft/mgt-msal2-provider</b>

    [`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contém o `Msal2Provider` componente `mgt-msal2-provider` e. O provedor MSAL usa o msal-browser para autenticação em aplicativos Web e PWAs.

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` componente `mgt-teams-provider` e. O Microsoft Teams habilita a autenticação no Microsoft Teams guia.

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)contém a `SharePointProvider` para autenticação em um SharePoint ambiente. 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md)contém o `ProxyProvider` aplicativo para que o proxy Graph chamadas por meio de um serviço back-end. 

<b>@microsoft/mgt</b>

O é o pacote principal que inclui todos os pacotes acima e os reexporta para que eles sejam disponibilizados por meio de um `@microsoft/mgt` único pacote que você pode instalar. 

<b>@microsoft/mgt-react</b>

O pacote contém todos os componentes de React gerados automaticamente e tem [`@microsoft/mgt-react`](./mgt-react.md) dependência do `@microsoft/mgt` pacote.

<b>@microsoft/mgt-spfx</b>

O pacote contém uma Estrutura do SharePoint que é necessária para usar o [`@microsoft/mgt-spfx`](./mgt-spfx.md) Microsoft Graph Toolkit em Estrutura do SharePoint soluções.

## <a name="polyfills"></a>Polyfills

Se você estiver usando os módulos ES6 do pacote npm e estiver direcionando um navegador, como [o IE11,](https://caniuse.com/#search=components) que não dá suporte a componentes web de forma nativa, você precisará incluir polyfills em seu projeto, pois eles não são incluídos automaticamente. Polyfills ajudam a preencher os recursos ausentes do navegador em navegadores que ainda estão em processo de atualização para dar suporte aos padrões do Componente Web. Para obter instruções e saber mais, consulte [polyfills documentation](https://www.webcomponents.org/polyfills). 

Os polyfills já estão incluídos se você estiver usando o Toolkit por meio do script mgt-loader.

## <a name="next-steps"></a>Próximas etapas
Agora você está pronto para começar a desenvolver com o microsoft Graph Toolkit! Os guias a seguir estão disponíveis para ajudá-lo a começar:

- [Registrar um aplicativo no Azure Active Directory](./add-aad-app-registration.md)
- [Criar um aplicativo Web (JavaScript)](./build-a-web-app.md) (javascript de baunilha)
- [Criar um aplicativo web (React)](./use-toolkit-with-react.md)
- [Criar um aplicativo web (Angular)](./use-toolkit-with-angular.md)
- [Criar uma web part do Microsoft Office SharePoint Online](./build-a-sharepoint-web-part.md)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
