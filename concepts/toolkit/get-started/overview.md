---
title: Começando com o Graph Toolkit da Microsoft
description: Comece a usar o Graph Toolkit microsoft em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e84350a7835cac7914f5238110f74b3383047e13
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579589"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Começando com o Graph Toolkit da Microsoft

Os componentes Graph Toolkit da Microsoft podem ser facilmente adicionados ao seu aplicativo web, SharePoint parte da Web ou Microsoft Teams guias. Os componentes são baseados em padrões da Web e podem ser usados em projetos JavaScript simples ou com estruturas web populares, como Reach, Angular, Vue.js e muito mais.

Você pode assistir a este vídeo curto para ver como é rápido e fácil começar com o Toolkit.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

Para um tutorial passo a passo, consulte o [módulo Get started with Microsoft Graph Toolkit](/learn/modules/msgraph-toolkit-intro/). 

## <a name="set-up-your-microsoft-365-tenant"></a>Configure o locatário do Microsoft 365.
Para se desenvolver com o Toolkit, você precisa ter acesso a um inquilino Microsoft 365. Se você não tiver uma, você pode obter uma assinatura gratuita de Microsoft 365 [desenvolvedores, aderindo ao programa de desenvolvedores Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program). Para obter detalhes sobre como configurar sua assinatura, consulte [Configurar uma assinatura de desenvolvedor Microsoft 365](/office/developer-program/microsoft-365-developer-program-get-started).

## <a name="set-up-your-development-environment"></a>Defina seu ambiente de desenvolvimento
Para se desenvolver com o Toolkit, você precisará de um editor de texto ou IDE. Você pode usar o editor ou IDE de sua escolha ou instalar e usar [Visual Studio Code](https://code.visualstudio.com/download) gratuitamente. Você também precisará de um navegador moderno como Microsoft Edge, Google Chrome ou Firefox. Você também precisará de uma versão LTS de Node.js, que você pode instalar a partir de [nodejs.org](https://nodejs.org).

## <a name="using-the-microsoft-graph-toolkit"></a>Usando o Graph Toolkit da Microsoft
Você pode usar o Microsoft Graph Toolkit em seu aplicativo fazendo referência diretamente ao carregador (via unpkg) ou instalando o pacote npm.

# <a name="unpkg"></a>[unpkg](#tab/html)
Para usar o Toolkit via mgt-loader, adicione a referência em um script ao seu código:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal2-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal2-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
O uso do Toolkit através de módulos ES6 lhe dará controle total do processo de agrupamento e permitirá que você empacota apenas o código necessário para o seu aplicativo. Para usar os módulos ES6, adicione o pacote npm ao seu projeto:

```cmd
npm install @microsoft/mgt
```
Agora você pode referenciar todos os componentes da página que você está usando:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a>Pacotes NPM

O Microsoft Graph Toolkit é composto por vários pacotes NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.

<b>@microsoft/mgt-elemento</b>

O `@microsoft/mgt-element` pacote principal que contém apenas as classes base usadas para a construção de componentes e provedores. Este pacote expõe todas as classes e interfaces necessárias para construir seus próprios componentes e exporta a [interface IProvider e a classe SimpleProvider](../providers/custom.md) para a construção de provedores personalizados.

<b>@microsoft/mgt-componentes</b>

O `@microsoft/mgt-components` pacote contém todos os componentes da Microsoft Graph conectados da Web, como , e muito `Person` `PeoplePicker` mais. 

**Provedores**

Os provedores estão disponíveis através de um único pacote e podem ser instalados conforme necessário. Os seguintes pacotes de provedores estão disponíveis:

- <b>@micosoft/mgt-msal-provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` `mgt-msal-provider` componente e o componente. O provedor MSAL usa msal.js para autenticar em aplicativos web e Aplicativos Web Progressivos (PWAs).

- <b>@micosoft/mgt-msal2-provider</b>

    [`@micosoft/mgt-msal2-provider`](../providers/msal2.md) contém o `Msal2Provider` `mgt-msal2-provider` componente e o componente. O provedor MSAL usa o navegador MSAL para autenticar em aplicativos web e PWAs.

-  <b>@microsoft/mgt-teams-provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` `mgt-teams-provider` componente e o componente. O provedor de Microsoft Teams permite a autenticação no aplicativo de guia Microsoft Teams.

- <b>@microsoft/mgt-sharepoint-provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md)contém o `SharePointProvider` para autenticar em um ambiente SharePoint. 

- <b>@microsoft/mgt-proxy-provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md)contém o `ProxyProvider` aplicativo para que o proxy Graph chamadas através de um serviço backend. 

<b>@microsoft/mgt</b>

O `@microsoft/mgt` pacote principal que inclui todos os pacotes acima e re-exporta-los para que eles estejam disponíveis através de um único pacote que você pode instalar. 

<b>@microsoft/mgt-react</b>

O [`@microsoft/mgt-react`](./mgt-react.md) pacote contém todos os componentes React gerados automaticamente e requer dependência do `@microsoft/mgt` pacote.

<b>@microsoft/mgt-spfx</b>

O [`@microsoft/mgt-spfx`](./mgt-spfx.md) pacote contém uma biblioteca Estrutura do SharePoint necessária para usar o Microsoft Graph Toolkit em soluções Estrutura do SharePoint.

## <a name="polyfills"></a>Polifilis

Se você estiver usando os módulos ES6 do pacote npm e estiver [mirando um navegador como o IE11](https://caniuse.com/#search=components) que não suporta componentes da Web nativamente, você precisará incluir polifildos em seu projeto, pois eles não estão automaticamente incluídos. Os polyfills ajudam a preencher os recursos ausentes do navegador em navegadores que ainda estão em processo de atualização para suportar os padrões do Web Component. Para obter instruções e saber mais, consulte [a documentação de polifilis](https://www.webcomponents.org/polyfills). 

Os polifilis já estão incluídos se você estiver usando o Toolkit através do script mgt-loader.

## <a name="next-steps"></a>Próximas etapas
Agora você está pronto para começar a desenvolver com o microsoft Graph Toolkit! Os seguintes guias estão disponíveis para ajudá-lo a começar:

- [Registrar um aplicativo no Azure Active Directory](./add-aad-app-registration.md)
- [Construa um aplicativo web (JavaScript)](./build-a-web-app.md) (baunilha JavaScript)
- [Criar um aplicativo web (React)](./use-toolkit-with-react.md)
- [Criar um aplicativo web (Angular)](./use-toolkit-with-angular.md)
- [Criar uma web part do Microsoft Office SharePoint Online](./build-a-sharepoint-web-part.md)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
