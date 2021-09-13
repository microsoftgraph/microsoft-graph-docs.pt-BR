---
title: Provedor do SharePoint
description: Use o provedor SharePoint seu SharePoint web parts para dar energia aos componentes com o microsoft Graph acesso.
ms.localizationpriority: medium
author: nmetulev
ms.openlocfilehash: f1906598eaa0218a9adb7749ecf9276b105f437b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126531"
---
# <a name="sharepoint-provider"></a>Provedor do SharePoint

Use o provedor SharePoint seu SharePoint web parts para dar energia aos componentes com o microsoft Graph acesso.

Para saber mais sobre provedores de autenticação, consulte [Provedores](./providers.md).

## <a name="get-started"></a>Introdução

Inicializar o provedor dentro `onInit()` do método da web part. Este exemplo usa o [ `@microsoft/mgt-spfx` pacote](../get-started/mgt-spfx.md).

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt-spfx';

// add the onInit() method if not already there in your web part class
protected async onInit() {
  Providers.globalProvider = new SharePointProvider(this.context);
}
```

Agora você pode adicionar qualquer componente em seu método e ele usará o contexto `render()` SharePoint para acessar o Microsoft Graph.

```ts
public render(): void {
  this.domElement.innerHTML = `
    <mgt-agenda></mgt-agenda>
    `;
}
```

>**Observação:** O microsoft Graph Toolkit requer Typescript 3.7 ou mais novo. Certifique-se de que você está usando uma versão com suporte do Typescript [instalando o compilador correto](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).

## <a name="sample"></a>Amostra

Para obter detalhes sobre como inicializar o provedor SharePoint, consulte o [guia Criar uma web part SharePoint](../get-started/build-a-sharepoint-web-part.md) de início.

## <a name="test-in-the-workbench"></a>Teste no workbench

Se você estiver apenas começando a usar SharePoint Web Parts, siga as diretrizes [Criar sua primeira Web Part.](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)

Depois de criar uma Web Part e estiver pronto para usar os componentes, você precisará garantir que sua Web Part tenha as permissões certas para acessar o Microsoft Graph. Para obter detalhes, [consulte Consume Microsoft Graph in the Estrutura do SharePoint](/sharepoint/dev/spfx/use-aad-tutorial).

Em resumo, é importante adicionar a permissão certa ao `package-solution.json` seu . Você precisará carregar um pacote da web part para SharePoint e fazer com que um administrador aprove as permissões solicitadas.

>[!TIP]
>O [guia Criar uma SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) de início fornece instruções passo a passo para configurar e aprovar permissões.

>**Observação:** se você não tiver certeza de quais permissões adicionar, a documentação de cada componente incluirá todas as permissões de que ele precisa.
