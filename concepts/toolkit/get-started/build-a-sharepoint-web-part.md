---
title: Criar uma web part do Microsoft Office SharePoint Online com o Kit de ferramentas do Microsoft Graph
description: Comece a usar o Kit de ferramentas do Microsoft Graph para construir uma web part do Microsoft Office SharePoint Online.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 74d13b37bf5de08540b938b55566ee16fbb269f1b84f736f8ef0e804edb10082
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54221058"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a>Criar uma web part do Microsoft Office SharePoint Online com o Kit de ferramentas do Microsoft Graph

Este tópico aborda como usar os componentes do o Kit de ferramentas do Microsoft Graph em uma [web part do lado do cliente do Microsoft Office SharePoint Online](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts). Os primeiros passos envolvem as seguintes etapas:

1. Configure seu ambiente de desenvolvimento e crie uma web part.
1. Adicione o pacote da Estrutura do SharePoint do Kit de ferramentas do Microsoft Graph.
1. Adicione o provedor do Microsoft Office SharePoint Online.
1. Adicione os componentes.
1. Configure as permissões.
1. Implante o pacote de Estrutura do SharePoint do Kit de ferramentas do Microsoft Graph.
1. Crie e implante sua web part.
1. Teste sua web part.

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a>Configure seu ambiente de desenvolvimento da Estrutura do SharePoint e crie uma nova web part

Siga as etapas para [Configurar seu ambiente de desenvolvimento da Estrutura do SharePoint](/sharepoint/dev/spfx/set-up-your-development-environment) e, em seguida, [criar uma nova web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>Adicione o pacote da Estrutura do SharePoint do Kit de ferramentas do Microsoft Graph

Para evitar que vários componentes da Estrutura do SharePoint registrem seu próprio conjunto de componentes do Kit de ferramentas do Microsoft Graph na página, você deve implantar o pacote de Estrutura do SharePoint do Kit de ferramentas do Microsoft Graph para o seu locatário e fazer referência aos componentes do kit de ferramentas do Microsoft Graph usados em sua solução deste pacote.

O pacote de Estrutura do SharePoint do Kit de ferramentas do Microsoft Graph contém uma biblioteca de Estrutura SharePoint que registra uma única instância dos componentes do Kit de ferramentas do Microsoft Graph no Microsoft Office SharePoint Online.

Instale o pacote npm do Kit de ferramentas do Microsoft Graph da Estrutura do SharePoint usando o seguinte comando:

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a>Adicionar o Provedor do Microsoft Office SharePoint Online

Os provedores do Kit de ferramentas do Microsoft Graph permitem autenticação e acesso ao Microsoft Graph para os componentes. Para saber mais, confira [Usando os provedores](../providers/providers.md). As web parts do Microsoft Office SharePoint Online sempre existem em um contexto autenticado porque o usuário já teve que entrar para acessar a página que hospeda sua web part. Use este contexto para inicializar o [provedor do Microsoft Office SharePoint Online](../providers/sharepoint.md).

Primeiro, adicione o provedor à sua web part. Localize o arquivo `src\webparts\<your-project>\<your-web-part>.ts` na pasta do projeto e adicione a seguinte linha no início do arquivo, logo abaixo das instruções `import` existentes:

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

Em seguida, você precisa inicializar o provedor com o contexto autenticado dentro do método `onInit()` de sua web part. No mesmo arquivo, adicione o seguinte código antes da linha `public render(): void {`:

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a>Adicionar os componentes

Agora, você pode começar a adicionar componentes à sua web part. Basta adicionar os componentes ao HTML dentro do método `render()` e os componentes usarão o contexto do Microsoft Office SharePoint Online para acessar o Microsoft Graph. Por exemplo, para adicionar o [componente Person](../components/person.md), seu código se parecerá com:

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> Se você estiver criando uma web part usando o React, confira a [documentação do @microsoft/mgt-spfx](./mgt-spfx.md#react) para saber como usá-la`@microsoft/mgt-react`.

## <a name="configure-permissions"></a>Configurar as permissões

Para chamar o Microsoft Graph de seu aplicativo da Estrutura do SharePoint, você precisa solicitar as permissões necessárias em seu pacote de solução e um administrador de locatário do Microsoft 365 precisa aprovar as permissões solicitadas.

Para adicionar as permissões ao seu pacote de solução, localize e abra o arquivo `config\package-solution.json` e defina:

```json
"isDomainIsolated": false,
```

Logo abaixo dessa linha, adicione o seguinte:

```json
"webApiPermissionRequests":[],
```

Determine quais permissões da API do Microsoft Graph você precisa, dependendo dos componentes que está usando. A página de documentação de cada componente fornece uma lista das permissões que o componente requer. Você precisará adicionar cada permissão necessária para `webApiPermissionRequests`. Por exemplo, se você estiver usando o componente Person e o componente Agenda, seu `webApiPermissionRequests` pode ser parecido com:

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a>Implantar o pacote do Kit de ferramentas do Microsoft Graph da Estrutura do SharePoint

Antes de implantar o pacote da Estrutura do SharePoint para o seu locatário, você precisará implantar o pacote do Kit de ferramentas do Microsoft Graph da Estrutura do SharePoint para o seu locatário. Você pode baixar o pacote correspondente à versão do Kit de ferramentas do Microsoft Graph que você usou em seu projeto, na seção [Lançamentos](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) no GitHub.

>[!IMPORTANT]
>Como apenas uma versão da biblioteca da Estrutura do SharePoint para o Kit de ferramentas do Microsoft Graph pode ser instalada no locatário, antes de usar o Kit de ferramentas do Microsoft Graph em sua solução, determine se sua organização ou cliente já possui uma versão da biblioteca da Estrutura do SharePoint implantada e use o mesma versão.

Depois de baixar o pacote .sppkg do Kit de ferramentas do Microsoft Graph da Estrutura do SharePoint, carregue-o no Catálogo de aplicativos do Microsoft Office SharePoint Online. Vá para a [ página Mais recursos do Centro de Administração do SharePoint Online](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true). Selecione **Abrir** em **Aplicativos**, clique em **Catálogo de Aplicativos** e **Distribuir aplicativos para Microsoft Office SharePoint Online**. Faça upload do seu arquivo `.sppkg` e clique em **Implementar**.

## <a name="build-and-deploy-your-web-part"></a>Construir e implantar sua web part

Agora, você irá construir seu aplicativo e implantá-lo no Microsoft Office SharePoint Online. Crie seu aplicativo executando os seguintes comandos:

```bash
gulp build
gulp bundle
gulp package-solution
```

Na pasta `sharepoint/solution`, haverá um novo arquivo `.sppkg`. Você precisará carregar este arquivo no seu Catálogo de Aplicativos Online do Microsoft Office SharePoint Online. Vá para a [ página Mais recursos do Centro de Administração do SharePoint Online](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true). Selecione **Abrir** em **Aplicativos**, clique em **Catálogo de Aplicativos** e **Distribuir aplicativos para Microsoft Office SharePoint Online**. Faça upload do seu arquivo `.sppkg` e clique em **Implementar**.

Em seguida, você precisa aprovar as permissões como um administrador.

Vá para o seu **Centro de administração do SharePoint Online**. Na navegação à esquerda, selecione **Avançado** e depois **Acesso à API**. Você deve ver as solicitações pendentes para cada uma das permissões adicionadas ao seu arquivo`config\package-solution.json`. Selecione e aprove cada permissão.

## <a name="test-your-web-part"></a>Testar sua web part

Agora você está pronto para adicionar sua web part a uma página do Microsoft Office SharePoint Online e testá-la. Você precisará usar o ambiente de trabalho hospedado para testar as web parts que usam o Kit de ferramentas do Microsoft Graph porque os componentes precisam do contexto autenticado para chamar o Microsoft Graph. Você pode localizar seu workbench hospedado em **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.

Abra o arquivo `config\serve.json` em seu projeto e substitua o valor  de `initialPage` pelo url de sua bancada hospedada:
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
Salve o arquivo e execute o seguinte comando no console para criar e visualizar sua web part:

```bash
gulp serve
```

Sua bancada de trabalho hospedada será aberta automaticamente em seu navegador. Adicione sua web part à página e você deverá vê-la com os componentes do Kit de ferramentas do Microsoft Graph em ação! Contanto que o comando gulp serve ainda esteja em execução em seu console, você pode continuar a fazer edições em seu código e, em seguida, apenas atualizar seu navegador para ver as alterações.

## <a name="next-steps"></a>Próximos passos
- Confira este tutorial passo a passo sobre [como criar uma web part SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).
- Experimente os componentes do [playground](https://mgt.dev).
- Faça uma pergunta no [Stack Overflow](https://aka.ms/mgt-question).
- Relate bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).
