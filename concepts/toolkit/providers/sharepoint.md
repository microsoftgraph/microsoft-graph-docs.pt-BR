---
title: Provedor do SharePoint
description: Use o provedor do SharePoint dentro de suas Web Parts do SharePoint para poder alimentar os componentes com o acesso ao Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: bb657e8fb5d6d9a775fb41e5c5c9fa6bf4662926
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657293"
---
# <a name="sharepoint-provider"></a>Provedor do SharePoint

Use o provedor do SharePoint dentro de suas Web Parts do SharePoint para poder alimentar os componentes com o acesso ao Microsoft Graph.

Para saber mais sobre provedores de autenticação, consulte [Providers](./providers.md).

## <a name="get-started"></a>Introdução

Inicialize o provedor dentro do `onInit()` método de sua Web Part.

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

Agora você pode adicionar qualquer componente no seu `render()` método e usará o contexto do SharePoint para acessar o Microsoft Graph.

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

>**Observação:** O Microsoft Graph Toolkit requer o typescript 3. x. Verifique se você está usando uma versão com suporte do typescript, [instalando o compilador certo](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).

## <a name="sample"></a>Amostra

Para obter detalhes sobre como initalize o provedor do SharePoint, consulte o guia de introdução à [Web Part do SharePoint](../get-started/build-a-sharepoint-web-part.md) .

Para obter um exemplo predefinido que mostra como usar os vários componentes em suas Web Parts do SharePoint, confira o [exemplo de Web Part do SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) no repositório do Microsoft Graph Toolkit.

## <a name="test-in-the-workbench"></a>Teste no Workbench

Se você estiver apenas começando a usar as Web Parts do SharePoint, poderá seguir as orientações [Compilar sua primeira Web Part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) .

Depois de criar uma Web Part e estiver pronto para usar os componentes, você precisará certificar-se de que sua Web Part tem as permissões corretas para acessar o Microsoft Graph. Para obter detalhes, consulte [consuma Microsoft Graph na estrutura do SharePoint](/sharepoint/dev/spfx/use-aad-tutorial).

Em suma, é importante adicionar a permissão certa ao seu `package-solution.json` . Você precisará carregar um pacote de sua Web Part para o SharePoint e fazer com que um administrador aprove as permissões solicitadas.

>[!TIP]
>O guia de introdução de [Web Parts do SharePoint](../get-started/build-a-sharepoint-web-part.md#configure-permissions) fornece instruções passo a passo para configurar e aprovar permissões.

>**Observação:** se você não tiver certeza de quais permissões adicionar, a documentação de cada componente inclui todas as permissões necessárias.

## <a name="polyfills"></a>Polyfills

Se você planeja suportar o IE11 em suas Web Parts do SPFx, você deve usar polipreenchimentos.

Para saber mais, confira [introdução ao Microsoft Graph Toolkit](../get-started/overview.md#polyfills).
