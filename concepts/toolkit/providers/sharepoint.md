---
title: Provedor do SharePoint
description: Use o provedor do SharePoint dentro de suas Web Parts do SharePoint para poder alimentar os componentes com o acesso ao Microsoft Graph.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e2088c41ce8f0cc3e55d269fc5f55c3c95633fbd
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37553898"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="1a57b-103">Provedor do SharePoint</span><span class="sxs-lookup"><span data-stu-id="1a57b-103">SharePoint provider</span></span>

<span data-ttu-id="1a57b-104">Use o provedor do SharePoint dentro de suas Web Parts do SharePoint para poder alimentar os componentes com o acesso ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a57b-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="1a57b-105">Para saber mais, veja [Providers](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="1a57b-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="1a57b-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="1a57b-106">Get started</span></span>

<span data-ttu-id="1a57b-107">Inicialize o provedor dentro do `onInit()` método de sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="1a57b-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt/dist/commonjs';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="1a57b-108">Agora você pode adicionar qualquer componente no seu `render()` método e usará o contexto do SharePoint para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a57b-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

><span data-ttu-id="1a57b-109">**Observação:** O Microsoft Graph Toolkit requer o typescript 3. x.</span><span class="sxs-lookup"><span data-stu-id="1a57b-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="1a57b-110">Verifique se você está usando uma versão com suporte do typescript, [instalando o compilador certo](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="1a57b-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="1a57b-111">Teste no Workbench</span><span class="sxs-lookup"><span data-stu-id="1a57b-111">Test in the workbench</span></span>

<span data-ttu-id="1a57b-112">Se você estiver apenas começando a usar as Web Parts do SharePoint, poderá seguir as orientações [Compilar sua primeira Web Part](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) .</span><span class="sxs-lookup"><span data-stu-id="1a57b-112">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="1a57b-113">Depois de criar uma Web Part e estiver pronto para usar os componentes, você precisará certificar-se de que sua Web Part tem as permissões corretas para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a57b-113">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="1a57b-114">Para obter detalhes, consulte [consuma Microsoft Graph na estrutura do SharePoint](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/use-aad-tutorial).</span><span class="sxs-lookup"><span data-stu-id="1a57b-114">For details, see [Consume Microsoft Graph in the SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="1a57b-115">Em suma, é importante adicionar a permissão certa ao seu `package-solution.json`.</span><span class="sxs-lookup"><span data-stu-id="1a57b-115">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="1a57b-116">Você precisará carregar um pacote de sua Web Part para o SharePoint e fazer com que um administrador aprove as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="1a57b-116">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

><span data-ttu-id="1a57b-117">**Dica:** se você não tiver certeza de quais permissões adicionar, a documentação de cada componente inclui todas as permissões necessárias.</span><span class="sxs-lookup"><span data-stu-id="1a57b-117">**Tip:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>
