---
title: Provedor do SharePoint
description: Use o provedor SharePoint seu SharePoint web parts para dar energia aos componentes com o microsoft Graph acesso.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: eb5e5c5935e51fe7574c41feb57700f473567707
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629123"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="ce92d-103">Provedor do SharePoint</span><span class="sxs-lookup"><span data-stu-id="ce92d-103">SharePoint provider</span></span>

<span data-ttu-id="ce92d-104">Use o provedor SharePoint seu SharePoint web parts para dar energia aos componentes com o microsoft Graph acesso.</span><span class="sxs-lookup"><span data-stu-id="ce92d-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="ce92d-105">Para saber mais sobre provedores de autenticação, consulte [Provedores](./providers.md).</span><span class="sxs-lookup"><span data-stu-id="ce92d-105">To learn more about authentication providers, see [Providers](./providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="ce92d-106">Introdução</span><span class="sxs-lookup"><span data-stu-id="ce92d-106">Get started</span></span>

<span data-ttu-id="ce92d-107">Inicializar o provedor dentro `onInit()` do método da web part.</span><span class="sxs-lookup"><span data-stu-id="ce92d-107">Initialize the provider inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="ce92d-108">Este exemplo usa o [ `@microsoft/mgt-spfx` pacote](../get-started/mgt-spfx.md).</span><span class="sxs-lookup"><span data-stu-id="ce92d-108">This example uses the [`@microsoft/mgt-spfx` package](../get-started/mgt-spfx.md).</span></span>

```ts
// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt-spfx';

// add the onInit() method if not already there in your web part class
protected async onInit() {
  Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="ce92d-109">Agora você pode adicionar qualquer componente em seu método e ele usará o contexto `render()` SharePoint para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ce92d-109">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts
public render(): void {
  this.domElement.innerHTML = `
    <mgt-agenda></mgt-agenda>
    `;
}
```

><span data-ttu-id="ce92d-110">**Observação:** O microsoft Graph Toolkit requer Typescript 3.7 ou mais novo.</span><span class="sxs-lookup"><span data-stu-id="ce92d-110">**Note:** The Microsoft Graph Toolkit requires Typescript 3.7 or newer.</span></span> <span data-ttu-id="ce92d-111">Certifique-se de que você está usando uma versão com suporte do Typescript [instalando o compilador correto](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="ce92d-111">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="sample"></a><span data-ttu-id="ce92d-112">Amostra</span><span class="sxs-lookup"><span data-stu-id="ce92d-112">Sample</span></span>

<span data-ttu-id="ce92d-113">Para obter detalhes sobre como inicializar o provedor SharePoint, consulte o [guia Criar uma web part SharePoint](../get-started/build-a-sharepoint-web-part.md) de início.</span><span class="sxs-lookup"><span data-stu-id="ce92d-113">For details about how to initialize the SharePoint provider, see the [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md) getting started guide.</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="ce92d-114">Teste no workbench</span><span class="sxs-lookup"><span data-stu-id="ce92d-114">Test in the workbench</span></span>

<span data-ttu-id="ce92d-115">Se você estiver apenas começando a usar SharePoint Web Parts, siga as diretrizes [Criar sua primeira Web Part.](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)</span><span class="sxs-lookup"><span data-stu-id="ce92d-115">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="ce92d-116">Depois de criar uma Web Part e estiver pronto para usar os componentes, você precisará garantir que sua Web Part tenha as permissões certas para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ce92d-116">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="ce92d-117">Para obter detalhes, [consulte Consume Microsoft Graph in the Estrutura do SharePoint](/sharepoint/dev/spfx/use-aad-tutorial).</span><span class="sxs-lookup"><span data-stu-id="ce92d-117">For details, see [Consume Microsoft Graph in the SharePoint Framework](/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="ce92d-118">Em resumo, é importante adicionar a permissão certa ao `package-solution.json` seu .</span><span class="sxs-lookup"><span data-stu-id="ce92d-118">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="ce92d-119">Você precisará carregar um pacote da web part para SharePoint e fazer com que um administrador aprove as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="ce92d-119">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

>[!TIP]
><span data-ttu-id="ce92d-120">O [guia Criar uma SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) de início fornece instruções passo a passo para configurar e aprovar permissões.</span><span class="sxs-lookup"><span data-stu-id="ce92d-120">The [Build a SharePoint web part](../get-started/build-a-sharepoint-web-part.md#configure-permissions) getting started guide provides step-by-step instructions for configuring and approving permissions.</span></span>

><span data-ttu-id="ce92d-121">**Observação:** se você não tiver certeza de quais permissões adicionar, a documentação de cada componente incluirá todas as permissões de que ele precisa.</span><span class="sxs-lookup"><span data-stu-id="ce92d-121">**Note:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>