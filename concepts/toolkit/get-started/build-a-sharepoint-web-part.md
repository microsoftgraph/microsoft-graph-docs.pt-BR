---
title: Criar uma Web Part do SharePoint com o kit de ferramentas do Microsoft Graph
description: Introdução ao uso do kit de ferramentas do Microsoft Graph para criar uma Web Part do SharePoint.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: d07a597c69ae998c75e3d4698cb0513cff056e56
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659747"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>Criar uma Web Part do SharePoint com o kit de ferramentas do Microsoft Graph

Este tópico aborda como usar os componentes do Microsoft Graph Toolkit em uma [Web Part do lado do cliente do SharePoint](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts). Introdução envolve as seguintes etapas:

1. Configurar seu ambiente de desenvolvimento e criar uma Web Part.
2. Atualize o TypeScript em seu projeto.
3. Adicione o Microsoft Graph Toolkit.
4. Adicione o provedor do SharePoint.
5. Adicionar componentes.
6. Configurar permissões.
7. Criar e implantar sua Web Part.
8. Testar sua Web Part.

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>Configurar seu ambiente de desenvolvimento da estrutura do SharePoint e criar uma nova Web Part

Siga as etapas para [configurar seu ambiente de desenvolvimento da estrutura do SharePoint](/sharepoint/dev/spfx/set-up-your-development-environment) e, em seguida, [criar uma nova Web Part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).

## <a name="update-typescript-in-your-project"></a>Atualizar TypeScript em seu projeto

O Microsoft Graph Toolkit requer o typescript 3. x. Antes de adicionar o kit de ferramentas ao seu projeto, verifique se você está usando uma [versão com suporte do typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x). Por exemplo, para adicionar o typescript 3,7, use o seguinte comando:

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
Em seguida, localize o `tsconfig.json` arquivo na pasta do projeto, abra o arquivo e procure esta linha:

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
Substitua a linha por:

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a>Adicionar o Microsoft Graph Toolkit

Instale o pacote NPM do Microsoft Graph Toolkit e os metapreenchimentos com o seguinte comando:

```bash
npm install @microsoft/mgt
```
Se você planeja suportar o IE11 em suas Web Parts, será necessário seguir etapas adicionais para garantir a compatibilidade entre navegadores:

1. Instale os seguintes pacotes:
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. Adicione o seguinte código ao `gulpfile.js` , imediatamente acima `build.initialize(gulp)` :
```ts
build.configureWebpack.mergeConfig({
  additionalConfiguration: (generatedConfiguration) => {
    generatedConfiguration.module.rules.push(
      {
        test: /\.m?js$/, use:
        {
          loader: "babel-loader",
          options:
          {
            presets: [["@babel/preset-env",
              {
                targets: {
                  "ie": "11"
                }
              }]]
          }
        }
      }
    );

    return generatedConfiguration;
  }
});
```
3. No `src\webparts\<your-project>\<your-web-part>.ts` arquivo, importe os seguintes metapreenchimentos antes do provedor do SharePoint na próxima etapa.

```ts
import 'regenerator-runtime/runtime';
import 'core-js/es/number';
import 'core-js/es/math';
import 'core-js/es/string';
import 'core-js/es/date';
import 'core-js/es/array';
import 'core-js/es/regexp';
import '@webcomponents/webcomponentsjs/webcomponents-bundle.js';
```

## <a name="add-the-sharepoint-provider"></a>Adicionar o provedor do SharePoint

Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para os componentes. Para saber mais, consulte [usando os provedores](../providers/providers.md). Web Parts do SharePoint sempre existem em um contexto autenticado porque o usuário já teve que entrar para acessar a página que hospeda sua Web Part. Use este contexto para inicializar o [provedor do SharePoint](../providers/sharepoint.md).

Primeiro, adicione o provedor à Web Part. Localize o `src\webparts\<your-project>\<your-web-part>.ts` arquivo na pasta do projeto e adicione a seguinte linha na parte superior do arquivo, logo abaixo das `import` instruções existentes:

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

Em seguida, você precisa inicializar o provedor com o contexto autenticado dentro do `onInit()` método de sua Web Part. No mesmo arquivo, adicione o seguinte código imediatamente antes da `public render(): void {` linha:

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a>Adicionar componentes

Agora, você pode começar a adicionar componentes à sua Web Part. Basta adicionar os componentes ao HTML dentro do `render()` método e os componentes usarão o contexto do SharePoint para acessar o Microsoft Graph. Por exemplo, para adicionar o [componente pessoa](../components/person.md), seu código terá a seguinte aparência:

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a>Configurar permissões

Para chamar o Microsoft Graph a partir do seu aplicativo da estrutura do SharePoint, você precisa solicitar as permissões necessárias no pacote de solução e um administrador de locatários do Microsoft 365 precisa aprovar as permissões solicitadas.

Para adicionar as permissões ao seu pacote de solução, localize e abra o `config\package-solution.json` arquivo e defina:

```json
"isDomainIsolated": false,
```

Logo abaixo dessa linha, adicione o seguinte:

```json
"webApiPermissionRequests":[],
```

Determine quais permissões de API do Microsoft Graph você precisa dependendo dos componentes que você está usando. A página de documentação de cada componente fornece uma lista das permissões exigidas pelo componente. Será necessário adicionar cada permissão necessária para o `webApiPermissionRequests` . Por exemplo, se você estiver usando o componente Person e o componente de agenda, você `webApiPermissionRequests` pode ter a seguinte aparência:

```json
"webApiPermissionRequests": [
  {
    "resource": "Microsoft Graph",
    "scope": "User.Read"
  },
  {
    "resource": "Microsoft Graph",
    "scope": "Calendars.Read"
  }
]
```
## <a name="build-and-deploy-your-web-part"></a>Criar e implantar sua Web Part

Agora, você irá criar seu aplicativo e implantá-lo no SharePoint. Crie seu aplicativo executando os seguintes comandos:

```bash
gulp build
gulp bundle
gulp package-solution
```

Na `sharepoint/solution` pasta, haverá um novo `.sppkg` arquivo. Você precisará carregar esse arquivo no catálogo de aplicativos do SharePoint Online. Vá para a [página mais recursos do seu centro de administração do SharePoint](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true). Selecione **abrir** em **aplicativos**, clique em **Catálogo de aplicativos** e **distribua aplicativos para SharePoint**. Carregue o `.sppkg` arquivo e clique em **implantar**.

Em seguida, você precisa aprovar as permissões como um administrador.

Vá para o **centro de administração do SharePoint**. Na navegação à esquerda, selecione **avançado** e, em seguida, **acesso à API**. Você deve ver as solicitações pendentes para cada uma das permissões adicionadas ao `config\package-solution.json` arquivo. Selecione e aprove cada permissão.

## <a name="test-your-web-part"></a>Testar sua Web Part

Agora você está pronto para adicionar a Web Part a uma página do SharePoint e testá-la. Você precisará usar o Workbench hospedado para testar Web Parts que usam o Microsoft Graph Toolkit porque os componentes precisam do contexto autenticado para chamar o Microsoft Graph. Você pode encontrar o Workbench hospedado em **https://<YOUR_TENANT>. SharePoint.com/_layouts/15/Workbench.aspx**.

Abra o `config\serve.json` arquivo no seu projeto e substitua o valor de `initialPage` pela URL do seu Workbench hospedado:
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
Salve o arquivo e, em seguida, execute o seguinte comando no console para compilar e visualizar sua Web Part:

```bash
gulp serve
```

O Workbench hospedado será aberto automaticamente no navegador. Adicione sua Web Part à página e você deverá ver sua Web Part com os componentes do Microsoft Graph Toolkit em ação! Contanto que o comando Gulp sirva ainda esteja em execução no seu console, você pode continuar a fazer edições no seu código e, em seguida, apenas atualizar seu navegador para ver suas alterações.

## <a name="next-steps"></a>Próximas etapas
- Confira este tutorial passo a passo sobre a [criação de uma Web Part do SharePoint](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).
- Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).