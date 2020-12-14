---
title: Introdução ao Microsoft Graph Toolkit
description: Introdução ao uso do Microsoft Graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: f1451213822e2489f04bb454c355125ed95b1aed
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664125"
---
# <a name="getting-started-with-the-microsoft-graph-toolkit"></a>Introdução ao Microsoft Graph Toolkit

Os componentes do Microsoft Graph Toolkit podem ser adicionados facilmente ao aplicativo Web, à Web Part do SharePoint ou às guias do Microsoft Teams. Os componentes são baseados em padrões da Web e podem ser usados em projetos de JavaScript simples ou com estruturas da Web populares, como REACH, angular, Vue.js e muito mais.

Você pode assistir a esse pequeno vídeo para ver como é rápido e fácil começar a usar o kit de ferramentas.

> [!VIDEO https://www.youtube-nocookie.com/embed/oZCGb2MMxa0]

## <a name="set-up-your-microsoft-365-tenant"></a>Configurar seu locatário do Microsoft 365
Para desenvolver com o kit de ferramentas, você precisa acessar um Microsoft 365 locatário. Se você não tiver um, poderá obter uma assinatura gratuita do desenvolvedor do Microsoft 365, [participando do programa de desenvolvedor do microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program). Para obter detalhes sobre como configurar sua assinatura, consulte [set up a Microsoft 365 Developer Subscription](/office/developer-program/microsoft-365-developer-program-get-started).

## <a name="set-up-your-development-environment"></a>Defina seu ambiente de desenvolvimento
Para desenvolver com o kit de ferramentas, você precisará de um editor de texto ou IDE. Você pode usar o editor ou o IDE de sua escolha ou instalar e usar o [Visual Studio Code](https://code.visualstudio.com/download) gratuitamente. Você também precisará de um navegador da Web moderno, como o Microsoft Edge, Google Chrome ou Firefox. Você também precisará de uma versão do LTS do Node.js, que pode ser instalada no [NodeJS.org](https://nodejs.org).

## <a name="using-the-microsoft-graph-toolkit"></a>Usando o kit de ferramentas do Microsoft Graph
Você pode usar o Microsoft Graph Toolkit em seu aplicativo referenciando o carregador diretamente (via unpkg) ou instalando o pacote NPM.

# <a name="unpkg"></a>[unpkg](#tab/html)
Para usar o kit de ferramentas via gerenciamento-Loader, adicione a referência em um script ao seu código:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"></mgt-msal-provider>
<mgt-login></mgt-login>
```
# <a name="npm"></a>[npm](#tab/npm)
O uso do kit de ferramentas por meio de módulos ES6 fornecerá controle total do processo de agrupamento e permitirá que você reúna apenas o código necessário para o aplicativo. Para usar os módulos ES6, adicione o pacote NPM ao seu projeto:

```cmd
npm install @microsoft/mgt
```
Agora, você pode fazer referência a todos os componentes na página que você está usando:

```html
<script type="module" src="node_modules/@microsoft/mgt/dist/es6/index.js"></script>

<mgt-login></mgt-login>
<mgt-agenda></mgt-agenda>
```


---


## <a name="npm-packages"></a>Pacotes NPM

O Microsoft Graph Toolkit é composto por vários pacotes do NPM, permitindo que você inclua apenas o código necessário para seus aplicativos.

<b>@microsoft/MGT-Element</b>

O `@microsoft/mgt-element` é o pacote principal que contém apenas as classes base usadas para criar componentes e provedores. Este pacote expõe todas as classes e interfaces necessárias para criar seus próprios componentes e exporta a [interface IProvider e a classe simpleprovider](../providers/custom.md) para a criação de provedores personalizados.

<b>@microsoft/MGT-Components</b>

O `@microsoft/mgt-components` pacote contém todos os componentes da Web conectados ao Microsoft Graph, como `Person` , `PeoplePicker` e mais. 

**Provedores**

Os provedores estão disponíveis por meio de um único pacote e podem ser instalados conforme necessário. Os seguintes pacotes de provedor estão disponíveis:

- <b>@micosoft/MGT-MSAL-Provider</b>

    [`@micosoft/mgt-msal-provider`](../providers/msal.md) contém o `MsalProvider` `mgt-msal-provider` componente e. O provedor MSAL utiliza msal.js para autenticação em aplicativos Web e PWAs.

-  <b>@microsoft/MGT-Teams-Provider</b>

    [`@microsoft/mgt-teams-provider`](../providers/teams.md) contém o `TeamsProvider` `mgt-teams-provider` componente e. O provedor do Microsoft Teams habilita a autenticação no aplicativo de guia do Microsoft Teams.

- <b>@microsoft/MGT-SharePoint-Provider</b>

    [`@microsoft/mgt-sharepoint-provider`](../providers/sharepoint.md) contém o `SharePointProvider` para autenticação em um ambiente do SharePoint. 

- <b>@microsoft/MGT-proxy-Provider</b>

    [`@microsoft/mgt-proxy-provider`](../providers/proxy.md) contém o `ProxyProvider` aplicativo para o qual o proxy Graph chama por meio de um serviço de back-end. 

<b>@microsoft/MGT</b>

O `@microsoft/mgt` é o pacote principal que inclui todos os pacotes acima e os exporta novamente para que estejam disponíveis por meio de um único pacote que você possa instalar. 

<b>@microsoft/MGT-React</b>

O [`@microsoft/mgt-react`](./mgt-react.md) pacote contém todos os componentes de reagir gerados automaticamente e assume a dependência do `@microsoft/mgt` pacote.

## <a name="polyfills"></a>Polyfills

Se você estiver usando os módulos ES6 do pacote do NPM e estiver [direcionando um navegador como o IE11](https://caniuse.com/#search=components) que não ofereça suporte a componentes Web nativamente, será necessário incluir os metapreenchimentos no seu projeto, pois eles não serão incluídos automaticamente. Os metapreenchimentos ajudam a preencher os recursos de navegador ausentes em navegadores que ainda estejam no processo de atualização para suporte aos padrões de componente da Web. Para obter instruções e saber mais, confira [documentação dos metaabastecimentos](https://www.webcomponents.org/polyfills). 

Os metapreenchimentos já estão incluídos se você estiver usando o kit de ferramentas através do script de gerenciamento de Complementos.

## <a name="next-steps"></a>Próximas etapas
Agora você está pronto para começar a desenvolver com o Microsoft Graph Toolkit! Os seguintes guias estão disponíveis para ajudá-lo a começar:

- [Registrar um aplicativo no Azure Active Directory](./add-aad-app-registration.md)
- [Criar um aplicativo Web (JavaScript)](./build-a-web-app.md) (JavaScript de baunilha)
- [Criar um aplicativo web (React)](./use-toolkit-with-react.md)
- [Criar um aplicativo web (Angular)](./use-toolkit-with-angular.md)
- [Criar uma web part do Microsoft Office SharePoint Online](./build-a-sharepoint-web-part.md)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
