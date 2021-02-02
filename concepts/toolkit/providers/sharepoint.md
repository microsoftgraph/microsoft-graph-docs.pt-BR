---
title: Provedor do SharePoint
description: Use o provedor do SharePoint dentro de suas Web Parts do SharePoint para a energia dos componentes com o acesso ao Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 2dc020dbe02a5b3018c1bfb343b7582f8a6110e5
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072342"
---
# <a name="sharepoint-provider"></a>Provedor do SharePoint

Use o provedor do SharePoint dentro de suas Web Parts do SharePoint para a energia dos componentes com o acesso ao Microsoft Graph.

Para saber mais sobre provedores de autenticação, consulte [Provedores.](./providers.md)

## <a name="get-started"></a>Introdução

Inicialize o provedor dentro `onInit()` do método da Web Part.

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

Agora você pode adicionar qualquer componente em seu `render()` método e ele usará o contexto do SharePoint para acessar o Microsoft Graph.

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

>**Observação:** O Microsoft Graph Toolkit requer o Typescript 3.x. Certifique-se de que você está usando uma versão com suporte do Typescript [instalando o compilador correto.](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)

## <a name="sample"></a>Amostra

Para obter detalhes sobre como inicializar o provedor do SharePoint, consulte o guia de iniciação da Web Part do [SharePoint.](../get-started/build-a-sharepoint-web-part.md)

Para ver um exemplo pré-criado que mostra como usar os vários componentes em suas Web Parts do [SharePoint,](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) confira o exemplo de Web Part do SharePoint no repositório do Microsoft Graph Toolkit.

## <a name="test-in-the-workbench"></a>Testar no workbench

Se você estiver apenas começando a usar as Web Parts do SharePoint, siga as orientações de Criar [sua primeira Web](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) Part.

Depois de criar uma Web Part e estar pronto para usar os componentes, você precisará garantir que sua Web Part tenha as permissões corretas para acessar o Microsoft Graph. Para obter detalhes, [consulte Consumir o Microsoft Graph na Estrutura do SharePoint.](/sharepoint/dev/spfx/use-aad-tutorial)

Em resumo, é importante adicionar a permissão certa ao seu `package-solution.json` . Você precisará carregar um pacote da Web Part para o SharePoint e pedir para um administrador aprovar as permissões solicitadas.

>[!TIP]
>O [guia de iniciação da Web Part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) criar uma Web Part do SharePoint fornece instruções passo a passo para configurar e aprovar permissões.

>**Observação:** se você não tiver certeza de quais permissões adicionar, a documentação de cada componente incluirá todas as permissões de que precisa.

## <a name="polyfills"></a>Polyfills

Se você planeja dar suporte ao IE11 em suas webparts SPFx, deve usar polyfills.

Para saber mais, consulte [Getting started with Microsoft Graph Toolkit](../get-started/overview.md#polyfills).
