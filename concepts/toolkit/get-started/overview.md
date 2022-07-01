---
title: Introdução ao Kit de ferramentas do Microsoft Graph
description: Saiba como configurar seu ambiente de desenvolvimento e locatário do Microsoft 365 para usar o Kit de Ferramentas do Microsoft Graph. Instale pacotes NPM para componentes e provedores.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 3e4711003808dfc97536b648fbd02a1ee40b78b2
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577711"
---
# <a name="get-started-with-microsoft-graph-toolkit"></a>Introdução ao Kit de Ferramentas do Microsoft Graph

Os componentes do Kit de Ferramentas do Microsoft Graph podem ser facilmente adicionados ao seu aplicativo Web, à Web Part do SharePoint ou às guias do Microsoft Teams. Os componentes são baseados em padrões da Web e podem ser usados em projetos JavaScript simples ou com estruturas da Web populares, como Reach, Angular e Vue.js.

Assista a este breve vídeo para começar a usar o kit de ferramentas.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Para obter um tutorial passo a passo, consulte o [módulo Introdução ao Kit de Ferramentas do Microsoft Graph](/learn/modules/msgraph-toolkit-intro/) . 

## <a name="set-up-your-microsoft-365-tenant"></a>Configure o locatário do Microsoft 365.

Para usar o Kit de Ferramentas do Microsoft Graph para desenvolver um aplicativo, você precisa acessar um locatário do Microsoft 365. Se você não tiver uma, poderá obter uma assinatura gratuita de desenvolvedor do Microsoft 365 ingressando no Programa para Desenvolvedores do [Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program). Para obter detalhes sobre como configurar sua assinatura, consulte [Configurar uma assinatura de desenvolvedor do Microsoft 365](/office/developer-program/microsoft-365-developer-program-get-started).

## <a name="set-up-your-development-environment"></a>Defina seu ambiente de desenvolvimento

Para desenvolver com o kit de ferramentas, você precisa do seguinte:

- Um editor de texto ou IDE. Você pode usar o editor ou o IDE de sua escolha ou pode instalar [e usar Visual Studio Code](https://code.visualstudio.com/download) gratuitamente.
- Um navegador da Web moderno, como Microsoft Edge, Google Chrome ou Firefox.
- Uma versão LTS do Node.js, que você pode instalar do [nodejs.org](https://nodejs.org).

## <a name="use-microsoft-graph-toolkit"></a>Usar o Kit de Ferramentas do Microsoft Graph

Você pode usar o Kit de Ferramentas do Microsoft Graph em seu aplicativo referenciando o carregador diretamente (via `unpkg`) ou instalando o `npm` pacote.

# <a name="unpkg"></a>[unpkg](#tab/html)
Para usar o kit de ferramentas, `mgt-loader`adicione a referência em um script ao código:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
O uso do kit de ferramentas por meio de módulos ES6 oferece controle total do processo de agrupamento e permite que você empacote apenas o código necessário para seu aplicativo. Para usar os módulos ES6, adicione o pacote `npm` ao seu projeto:

```cmd
npm install @microsoft/mgt
```
Agora você pode referenciar todos os componentes na página que está usando:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


### <a name="npm-packages"></a>Pacotes NPM

O Kit de Ferramentas do Microsoft Graph é composto por vários pacotes NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.

<b>@microsoft/mgt-element</b>

É `@microsoft/mgt-element` o pacote principal que contém apenas as classes base usadas para criar componentes e provedores. Esse pacote expõe todas as classes e interfaces necessárias que você precisa para criar seus próprios componentes e exporta a [interface IProvider e a classe SimpleProvider](../providers/custom.md) para criar provedores personalizados.

<b>@microsoft/mgt-components</b>

O `@microsoft/mgt-components` pacote contém todos os componentes da Web conectados ao Microsoft Graph, como `Person`, `PeoplePicker`e muito mais. 

**Provedores**

Os provedores estão disponíveis por meio de um único pacote e podem ser instalados conforme necessário. Os seguintes pacotes de provedor estão disponíveis:

- <b>@microsoft/mgt-msal-provider</b>

    <code>[@microsoft/mgt-msal-provider](../providers/msal.md)</code> contém o `MsalProvider` componente `mgt-msal-provider` e o componente. O provedor MSAL usa msal.js autenticação em aplicativos Web e PWAs (Aplicativos Web Progressivo).

- <b>@microsoft/mgt-msal2-provider</b>

    <code>[@microsoft/mgt-msal2-provider](../providers/msal2.md)</code> contém o `Msal2Provider` componente `mgt-msal2-provider` e o componente. O provedor MSAL2 usa msal-browser para autenticação em aplicativos Web e PWAs.

-  <b>@microsoft/mgt-teams-provider</b>

    <code>[@microsoft/mgt-teams-provider](../providers/teams.md)</code> contém o `TeamsProvider` componente `mgt-teams-provider` e o componente. O provedor do Microsoft Teams habilita a autenticação no aplicativo de guia do Microsoft Teams.

-  <b>@microsoft/mgt-teams-msal2-provider</b>

    <code>[@microsoft/mgt-teams-msal2-provider](../providers/teams.md)</code> contém o `TeamsMsal2Provider` componente `mgt-teams-msal2-provider` e o componente. O provedor MSAL2 do Microsoft Teams habilita a autenticação no aplicativo de guia do Microsoft Teams.

- <b>@microsoft/mgt-sharepoint-provider</b>

    <code>[@microsoft/mgt-sharepoint-provider](../providers/sharepoint.md)</code> contém a `SharePointProvider` autenticação em um ambiente do SharePoint. 

- <b>@microsoft/mgt-proxy-provider</b>

    <code>[@microsoft/mgt-proxy-provider](../providers/proxy.md)</code> contém o para `ProxyProvider` um aplicativo que o Proxy Graph chama por meio de um serviço de back-end. 

<b>@microsoft/mgt</b>

O `@microsoft/mgt` pacote é o pacote principal que inclui todos os pacotes anteriores e os exporta novamente para que eles estejam disponíveis por meio de um único pacote que você pode instalar. 

<b>@microsoft/mgt-react</b>

O <code>[@microsoft/mgt-react](./mgt-react.md)</code> pacote contém todos os componentes de React gerados automaticamente e assume a dependência do `@microsoft/mgt` pacote.

<b>@microsoft/mgt-spfx</b>

O <code>[@microsoft/mgt-spfx](./mgt-spfx.md)</code> pacote contém uma Estrutura do SharePoint que é necessária para usar o Kit de Ferramentas do Microsoft Graph em Estrutura do SharePoint soluções.

## <a name="next-steps"></a>Próximos passos

Agora você está pronto para começar a desenvolver com o Kit de Ferramentas do Microsoft Graph! Os guias a seguir estão disponíveis para ajudá-lo a começar:

- [Registrar um aplicativo do Azure Active Directory (Azure AD)](./add-aad-app-registration.md)
- [Criar um aplicativo Web (JavaScript)](./build-a-web-app.md) (JavaScript de vanilla)
- [Criar um aplicativo web (React)](./use-toolkit-with-react.md)
- [Criar um aplicativo web (Angular)](./use-toolkit-with-angular.md)
- [Criar uma web part do Microsoft Office SharePoint Online](./build-a-sharepoint-web-part.md)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Criar uma guia de SSO do Microsoft Teams](./build-a-microsoft-teams-sso-tab.md)
- [Criar um aplicativo Electron](./build-an-electron-app.md)
