---
title: Criar uma web part SharePoint com o microsoft Graph Toolkit
description: Começar a usar o microsoft Graph Toolkit para criar uma web part SharePoint web part.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: c1f4be864c9e762e164980bc20abb4195df5c9f7
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629130"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>Criar uma web part SharePoint com o microsoft Graph Toolkit

Este tópico aborda como usar os componentes do Microsoft Graph Toolkit em uma [web part SharePoint do lado do cliente.](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts) Começar envolve as seguintes etapas:

1. Configurar seu ambiente de desenvolvimento e criar uma Web Part.
1. Adicione o pacote microsoft Graph Toolkit Estrutura do SharePoint.
1. Adicione o SharePoint Provedor.
1. Adicione componentes.
1. Configurar permissões.
1. Implante o pacote microsoft Graph Toolkit Estrutura do SharePoint.
1. Crie e implante sua Web Part.
1. Teste sua Web Part.

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>Configurar seu ambiente de Estrutura do SharePoint de desenvolvimento e criar uma nova Web Part

Siga as etapas para Configurar seu ambiente de [Estrutura do SharePoint de desenvolvimento](/sharepoint/dev/spfx/set-up-your-development-environment) e, em seguida, criar uma nova Web [Part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>Adicionar o pacote microsoft Graph Toolkit Estrutura do SharePoint

Para impedir que vários componentes Estrutura do SharePoint registrem seu próprio conjunto de componentes do Microsoft Graph Toolkit na página, você deve implantar o pacote do Microsoft Graph Toolkit Estrutura do SharePoint para seu locatário e fazer referência aos componentes do Microsoft Graph Toolkit que você usa em sua solução a partir deste pacote.

O pacote Graph Toolkit Estrutura do SharePoint microsoft contém uma biblioteca Estrutura do SharePoint que registra uma única instância de componentes do Microsoft Graph Toolkit no SharePoint.

Instale o pacote npm do Microsoft Graph Toolkit Estrutura do SharePoint usando o seguinte comando:

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a>Adicionar o provedor SharePoint

Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). SharePoint web parts sempre existem em um contexto autenticado porque o usuário já precisou entrar para acessar a página que hospeda sua Web Part. Use este contexto para inicializar o [provedor SharePoint .](../providers/sharepoint.md)

Primeiro, adicione o provedor à web part. Localize o arquivo em sua pasta de projeto e adicione a seguinte linha à parte superior do arquivo, logo `src\webparts\<your-project>\<your-web-part>.ts` abaixo das instruções `import` existentes:

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

Em seguida, você precisa inicializar o provedor com o contexto autenticado dentro do `onInit()` método da web part. No mesmo arquivo, adicione o seguinte código antes da `public render(): void {` linha:

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a>Adicionar componentes

Agora, você pode começar a adicionar componentes à web part. Basta adicionar os componentes ao HTML dentro do método e os componentes usarão o contexto SharePoint para acessar o `render()` Microsoft Graph. Por exemplo, para adicionar o [componente Person](../components/person.md), seu código terá a aparência:

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> Se você estiver criando uma Web Part usando React, consulte os documentos [@microsoft/mgt-spfx](./mgt-spfx.md#react) para saber como usar `@microsoft/mgt-react` .

## <a name="configure-permissions"></a>Configurar permissões

Para chamar o Microsoft Graph de seu aplicativo Estrutura do SharePoint, você precisa solicitar as permissões necessárias no pacote de soluções e um administrador Microsoft 365 locatário precisa aprovar as permissões solicitadas.

Para adicionar as permissões ao pacote de solução, localize e abra o `config\package-solution.json` arquivo e desmarcar:

```json
"isDomainIsolated": false,
```

Logo abaixo dessa linha, adicione o seguinte:

```json
"webApiPermissionRequests":[],
```

Determine quais permissões de API do Microsoft Graph você precisa, dependendo dos componentes que você está usando. A página de documentação de cada componente fornece uma lista das permissões que o componente exige. Você precisará adicionar cada permissão necessária a `webApiPermissionRequests` . Por exemplo, se você estiver usando o componente Person e o componente Agenda, pode `webApiPermissionRequests` ter a aparência:

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>Implantar o pacote microsoft Graph Toolkit Estrutura do SharePoint

Antes de implantar seu pacote Estrutura do SharePoint no seu locatário, você precisará implantar o pacote microsoft Graph Toolkit Estrutura do SharePoint para seu locatário. Você pode baixar o pacote correspondente à versão do Microsoft Graph Toolkit que você usou em seu projeto, na seção [Versões](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) no GitHub.

>[!IMPORTANT]
>Como apenas uma versão da biblioteca Estrutura do SharePoint do Microsoft Graph Toolkit pode ser instalada no locatário, antes de usar o Microsoft Graph Toolkit em sua solução, determine se sua organização ou cliente já tem uma versão da biblioteca Estrutura do SharePoint implantada e use a mesma versão.

Depois de baixar o pacote .sppkg do Microsoft Graph Toolkit Estrutura do SharePoint, carregue-o no catálogo de aplicativos SharePoint Online. Vá para a [página Mais recursos do seu SharePoint de administração.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true) Selecione **Abrir** em **Aplicativos,** clique em **Catálogo de Aplicativos** e **Distribuir aplicativos para SharePoint**. Upload seu `.sppkg` arquivo e clique em **Implantar**.

## <a name="build-and-deploy-your-web-part"></a>Criar e implantar sua Web Part

Agora, você criará seu aplicativo e o implantará SharePoint. Crie seu aplicativo executando os seguintes comandos:

```bash
gulp build
gulp bundle
gulp package-solution
```

Na `sharepoint/solution` pasta, haverá um novo `.sppkg` arquivo. Você precisará carregar esse arquivo no catálogo de aplicativos SharePoint Online. Vá para a [página Mais recursos do seu SharePoint de administração.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true) Selecione **Abrir** em **Aplicativos,** clique em **Catálogo de Aplicativos** e **Distribuir aplicativos para SharePoint**. Upload seu `.sppkg` arquivo e clique em **Implantar**.

Em seguida, você precisa aprovar as permissões como administrador.

Vá para o centro **de administração SharePoint.** Na navegação à esquerda, selecione **Avançado** e, em seguida, **Acesso à API**. Você deve ver solicitações pendentes para cada uma das permissões adicionadas em seu `config\package-solution.json` arquivo. Selecione e aprove cada permissão.

## <a name="test-your-web-part"></a>Testar sua Web Part

Agora você está pronto para adicionar sua Web Part a uma SharePoint e testá-la. Você precisará usar o workbench hospedado para testar web parts que usam o microsoft Graph Toolkit porque os componentes precisam do contexto autenticado para chamar o Microsoft Graph. Você pode encontrar seu workbench hospedado **em https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.

Abra o `config\serve.json` arquivo em seu projeto e substitua o valor de pela URL do seu `initialPage` workbench hospedado:
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
Salve o arquivo e execute o seguinte comando no console para criar e visualizar sua Web Part:

```bash
gulp serve
```

Seu workbench hospedado será aberto automaticamente no navegador. Adicione sua Web Part à página e você deverá ver sua Web Part com os componentes Graph Toolkit Microsoft em ação! Enquanto o comando gulp serve ainda está em execução no console, você pode continuar a fazer edições para seu código e, em seguida, apenas atualizar seu navegador para ver suas alterações.

## <a name="next-steps"></a>Próximas etapas
- Confira este tutorial passo a passo sobre [como criar uma web part SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).
- Experimente os componentes no [playground](https://mgt.dev).
- Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).
- Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).
