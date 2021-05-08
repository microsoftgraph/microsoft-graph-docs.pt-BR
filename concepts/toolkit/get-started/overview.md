---
title: Iniciando o microsoft graph Toolkit
description: Começar a usar o microsoft graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 15d3e4721ae43146496b1a54ec12bc7906bfda5b
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266868"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Iniciando o microsoft graph Toolkit

Os componentes Toolkit do Microsoft Graph podem ser facilmente adicionados ao aplicativo Web, à Web Part do SharePoint ou às guias do Microsoft Teams. Os componentes são baseados em padrões web e podem ser usados em projetos JavaScript simples ou com estruturas da Web populares, como Reach, Angular, Vue.js e muito mais.

Você pode assistir a este vídeo curto para ver como é rápido e fácil começar com o Toolkit.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Para obter um tutorial passo a passo, consulte o [módulo Introdução ao Microsoft Graph Toolkit .](/learn/modules/msgraph-toolkit-intro/) 

## <a name="set-up-your-microsoft-365-tenant"></a>Configure o locatário do Microsoft 365.
Para desenvolver com o Toolkit, você precisa acessar um locatário do Microsoft 365. Se você não tiver um, poderá obter uma assinatura gratuita de desenvolvedor do Microsoft 365 ins juntando-se ao Programa de Desenvolvedores do [Microsoft 365.](https://developer.microsoft.com/microsoft-365/dev-program) Para obter detalhes sobre como configurar sua assinatura, consulte Configurar uma assinatura de [desenvolvedor do Microsoft 365](/office/developer-program/microsoft-365-developer-program-get-started).

## <a name="set-up-your-development-environment"></a>Defina seu ambiente de desenvolvimento
Para desenvolver com o Toolkit, você precisará de um editor de texto ou IDE. Você pode usar o editor ou o IDE de sua escolha ou instalar e usar [Visual Studio Código](https://code.visualstudio.com/download) gratuitamente. Você também precisará de um navegador da Web moderno, como o Microsoft Edge, o Google Chrome ou o Firefox. Você também precisará de uma versão LTS do Node.js, que pode ser instalada [nodejs.org](https://nodejs.org).

## <a name="using-the-microsoft-graph-toolkit"></a>Usando o microsoft graph Toolkit
Você pode usar o microsoft graph Toolkit em seu aplicativo fazendo referência ao carregador diretamente (por meio de unpkg) ou instalando o pacote npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
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

O microsoft graph Toolkit é feito de vários pacotes NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.

<b>@microsoft/mgt-element</b>

O `@microsoft/mgt-element` é o pacote principal que contém apenas as classes base usadas para criar componentes e provedores. Este pacote expõe todas as classes e interfaces necessárias necessárias para criar seus próprios componentes e exporta a interface IProvider e a [classe SimpleProvider](../providers/custom.md) para a criação de provedores personalizados.

<b>@microsoft/mgt-components</b>

O `@microsoft/mgt-components` pacote contém todos os componentes web conectados do Microsoft Graph, como `Person` , e muito `PeoplePicker` mais. 

**Provedores**

Os provedores estão disponíveis por meio de um único pacote e podem ser instalados conforme necessário. Os seguintes pacotes de provedor estão disponíveis:

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` componente `mgt-msal-provider` e. O provedor msal aproveita o msal.js para autenticação em aplicativos Web e PWAs.

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` componente `mgt-teams-provider` e. O provedor do Microsoft Teams habilita a autenticação no aplicativo de guia do Microsoft Teams.

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contém o `SharePointProvider` para autenticação em um ambiente do SharePoint. 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contém o `ProxyProvider` aplicativo para o que o Proxy Graph chama por meio de um serviço de back-end. 

<b>@microsoft/mgt</b>

O é o pacote principal que inclui todos os pacotes acima e os reexporta para que eles sejam disponibilizados por meio de um `@microsoft/mgt` único pacote que você pode instalar. 

<b>@microsoft/mgt-react</b>

O pacote contém todos os componentes do React gerados automaticamente [`@microsoft/mgt-react`](./mgt-react.md) e tem dependência do `@microsoft/mgt` pacote.

## <a name="polyfills"></a>Polyfills

Se você estiver usando os módulos ES6 do pacote npm e estiver direcionando um navegador, como [o IE11,](https://caniuse.com/#search=components) que não dá suporte a componentes web de forma nativa, você precisará incluir polyfills em seu projeto, pois eles não são incluídos automaticamente. Polyfills ajudam a preencher os recursos ausentes do navegador em navegadores que ainda estão em processo de atualização para dar suporte aos padrões do Componente Web. Para obter instruções e saber mais, consulte [polyfills documentation](https://www.webcomponents.org/polyfills). 

Os polyfills já estão incluídos se você estiver usando o Toolkit por meio do script mgt-loader.

## <a name="next-steps"></a>Próximas Etapas
Agora você está pronto para começar a desenvolver com o microsoft graph Toolkit! Os guias a seguir estão disponíveis para ajudá-lo a começar:

- [Registrar um aplicativo no Azure Active Directory](./add-aad-app-registration.md)
- [Criar um aplicativo Web (JavaScript)](./build-a-web-app.md) (javascript de baunilha)
- [Criar um aplicativo web (React)](./use-toolkit-with-react.md)
- [Criar um aplicativo web (Angular)](./use-toolkit-with-angular.md)
- [Criar uma web part do Microsoft Office SharePoint Online](./build-a-sharepoint-web-part.md)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
