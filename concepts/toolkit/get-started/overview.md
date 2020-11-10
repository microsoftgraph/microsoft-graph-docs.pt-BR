---
title: Introdução ao Microsoft Graph Toolkit
description: Introdução ao uso do Microsoft Graph Toolkit em seu aplicativo.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: e3739bb6180e19569ae40e873d3a018bbb541833
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977132"
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

### <a name="use-via-mgt-loader"></a>Usar via gerenciamento-carregador
Para usar o kit de ferramentas via gerenciamento-Loader, adicione a referência em um script ao seu código:

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

### <a name="use-via-npm-es6-modules"></a>Usar via NPM (módulos ES6)
O uso do kit de ferramentas por meio de módulos ES6 fornecerá controle total do processo de agrupamento e permitirá que você reúna apenas o código necessário para o aplicativo. Para usar os módulos ES6, adicione o pacote NPM ao seu projeto:

```bash
npm install @microsoft/mgt
```
Agora, você pode fazer referência a todos os componentes na página que você está usando:

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

Ou, apenas faça referência ao componente de que você precisa e Evite carregar tudo o mais:
```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

#### <a name="polyfills"></a>Polyfills

Se você estiver usando os módulos ES6 do pacote do NPM e estiver [direcionando um navegador como o IE11](https://caniuse.com/#search=components) que não ofereça suporte a componentes Web nativamente, será necessário incluir os metapreenchimentos no seu projeto, pois eles não serão incluídos automaticamente. Os metapreenchimentos ajudam a preencher os recursos de navegador ausentes em navegadores que ainda estejam no processo de atualização para suportar os padrões do webcComponent. Para obter instruções e saber mais, confira [documentação dos metaabastecimentos](https://www.webcomponents.org/polyfills). 

Os metapreenchimentos já estão incluídos se você estiver usando o kit de ferramentas através do script de gerenciamento de Complementos.

## <a name="next-steps"></a>Próximas Etapas
Agora você está pronto para começar a desenvolver com o Microsoft Graph Toolkit! Os seguintes guias estão disponíveis para ajudá-lo a começar:

- [Criar um aplicativo do Azure Active Directory](./add-aad-app-registration.md)
- [Criar um aplicativo Web](./build-a-web-app.md) (JavaScript de baunilha)
- [Criar uma web part do Microsoft Office SharePoint Online](./build-a-sharepoint-web-part.md)
- [Criar uma guia do Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Usar o kit de ferramentas reagir](./use-toolkit-with-react.md)
- [Usar o kit de ferramentas com angular](./use-toolkit-with-angular.md)
