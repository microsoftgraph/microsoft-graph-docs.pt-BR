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
# <a name="sharepoint-provider"></a><span data-ttu-id="73811-103">Provedor do SharePoint</span><span class="sxs-lookup"><span data-stu-id="73811-103">SharePoint provider</span></span>

<span data-ttu-id="73811-104">Use o provedor do SharePoint dentro de suas Web Parts do SharePoint para poder alimentar os componentes com o acesso ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="73811-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="73811-105">Para saber mais sobre provedores de autenticação, consulte [Providers](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="73811-105">To learn more about authentication providers, see [Providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="73811-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="73811-106">Get started</span></span>

<span data-ttu-id="73811-107">Inicialize o provedor dentro do `onInit()` método de sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="73811-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="73811-108">Agora você pode adicionar qualquer componente no seu `render()` método e usará o contexto do SharePoint para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="73811-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

><span data-ttu-id="73811-109">**Observação:** O Microsoft Graph Toolkit requer o typescript 3. x.</span><span class="sxs-lookup"><span data-stu-id="73811-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="73811-110">Verifique se você está usando uma versão com suporte do typescript, [instalando o compilador certo](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="73811-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="73811-111">Amostra</span><span class="sxs-lookup"><span data-stu-id="73811-111">Sample</span></span>

<span data-ttu-id="73811-112">Para obter detalhes sobre como initalize o provedor do SharePoint, consulte o guia de introdução à [Web Part do SharePoint](../get-started/build-a-sharepoint-web-part.md) .</span><span class="sxs-lookup"><span data-stu-id="73811-112">For details about how to initalize the SharePoint provider, see the [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md) getting started guide.</span></span>

<span data-ttu-id="73811-113">Para obter um exemplo predefinido que mostra como usar os vários componentes em suas Web Parts do SharePoint, confira o [exemplo de Web Part do SharePoint](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) no repositório do Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="73811-113">For a pre-built example that shows you how to use the various components in your SharePoint web parts, see the [SharePoint web part sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/sp-webpart) in the Microsoft Graph Toolkit repository.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="73811-114">Teste no Workbench</span><span class="sxs-lookup"><span data-stu-id="73811-114">Test in the workbench</span></span>

<span data-ttu-id="73811-115">Se você estiver apenas começando a usar as Web Parts do SharePoint, poderá seguir as orientações [Compilar sua primeira Web Part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) .</span><span class="sxs-lookup"><span data-stu-id="73811-115">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="73811-116">Depois de criar uma Web Part e estiver pronto para usar os componentes, você precisará certificar-se de que sua Web Part tem as permissões corretas para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="73811-116">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="73811-117">Para obter detalhes, consulte [consuma Microsoft Graph na estrutura do SharePoint](/sharepoint/dev/spfx/use-aad-tutorial).</span><span class="sxs-lookup"><span data-stu-id="73811-117">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="73811-118">Em suma, é importante adicionar a permissão certa ao seu `package-solution.json` .</span><span class="sxs-lookup"><span data-stu-id="73811-118">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="73811-119">Você precisará carregar um pacote de sua Web Part para o SharePoint e fazer com que um administrador aprove as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="73811-119">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

>[!TIP]
><span data-ttu-id="73811-120">O guia de introdução de [Web Parts do SharePoint](../get-started/build-a-sharepoint-web-part.md#configure-permissions) fornece instruções passo a passo para configurar e aprovar permissões.</span><span class="sxs-lookup"><span data-stu-id="73811-120">The [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) getting started guide provides step-by-step instructions for configuring and approving permissions.</span></span>

><span data-ttu-id="73811-121">**Observação:** se você não tiver certeza de quais permissões adicionar, a documentação de cada componente inclui todas as permissões necessárias.</span><span class="sxs-lookup"><span data-stu-id="73811-121">**Note:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>

## <a name="polyfills"></a><span data-ttu-id="73811-122">Polyfills</span><span class="sxs-lookup"><span data-stu-id="73811-122">Polyfills</span></span>

<span data-ttu-id="73811-123">Se você planeja suportar o IE11 em suas Web Parts do SPFx, você deve usar polipreenchimentos.</span><span class="sxs-lookup"><span data-stu-id="73811-123">If you plan to support IE11 in your SPFx webparts, you must use polyfills.</span></span>

<span data-ttu-id="73811-124">Para saber mais, confira [introdução ao Microsoft Graph Toolkit](../get-started/overview.md#polyfills).</span><span class="sxs-lookup"><span data-stu-id="73811-124">To learn more, see [Getting started with Microsoft Graph Toolkit](../get-started/overview.md#polyfills).</span></span>
