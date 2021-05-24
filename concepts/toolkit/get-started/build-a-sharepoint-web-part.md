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
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="42204-103">Criar uma web part SharePoint com o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="42204-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="42204-104">Este tópico aborda como usar os componentes do Microsoft Graph Toolkit em uma [web part SharePoint do lado do cliente.](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)</span><span class="sxs-lookup"><span data-stu-id="42204-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="42204-105">Começar envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="42204-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="42204-106">Configurar seu ambiente de desenvolvimento e criar uma Web Part.</span><span class="sxs-lookup"><span data-stu-id="42204-106">Set up your development environment and create a web part.</span></span>
1. <span data-ttu-id="42204-107">Adicione o pacote microsoft Graph Toolkit Estrutura do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="42204-107">Add the Microsoft Graph Toolkit SharePoint Framework package.</span></span>
1. <span data-ttu-id="42204-108">Adicione o SharePoint Provedor.</span><span class="sxs-lookup"><span data-stu-id="42204-108">Add the SharePoint Provider.</span></span>
1. <span data-ttu-id="42204-109">Adicione componentes.</span><span class="sxs-lookup"><span data-stu-id="42204-109">Add components.</span></span>
1. <span data-ttu-id="42204-110">Configurar permissões.</span><span class="sxs-lookup"><span data-stu-id="42204-110">Configure permissions.</span></span>
1. <span data-ttu-id="42204-111">Implante o pacote microsoft Graph Toolkit Estrutura do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="42204-111">Deploy the Microsoft Graph Toolkit SharePoint Framework package.</span></span>
1. <span data-ttu-id="42204-112">Crie e implante sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="42204-112">Build and deploy your web part.</span></span>
1. <span data-ttu-id="42204-113">Teste sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="42204-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="42204-114">Configurar seu ambiente de Estrutura do SharePoint de desenvolvimento e criar uma nova Web Part</span><span class="sxs-lookup"><span data-stu-id="42204-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="42204-115">Siga as etapas para Configurar seu ambiente de [Estrutura do SharePoint de desenvolvimento](/sharepoint/dev/spfx/set-up-your-development-environment) e, em seguida, criar uma nova Web [Part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span><span class="sxs-lookup"><span data-stu-id="42204-115">Follow the steps to [Set up your SharePoint Framework development environment](/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a><span data-ttu-id="42204-116">Adicionar o pacote microsoft Graph Toolkit Estrutura do SharePoint</span><span class="sxs-lookup"><span data-stu-id="42204-116">Add the Microsoft Graph Toolkit SharePoint Framework package</span></span>

<span data-ttu-id="42204-117">Para impedir que vários componentes Estrutura do SharePoint registrem seu próprio conjunto de componentes do Microsoft Graph Toolkit na página, você deve implantar o pacote do Microsoft Graph Toolkit Estrutura do SharePoint para seu locatário e fazer referência aos componentes do Microsoft Graph Toolkit que você usa em sua solução a partir deste pacote.</span><span class="sxs-lookup"><span data-stu-id="42204-117">To prevent multiple SharePoint Framework components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy the Microsoft Graph Toolkit SharePoint Framework package to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this package.</span></span>

<span data-ttu-id="42204-118">O pacote Graph Toolkit Estrutura do SharePoint microsoft contém uma biblioteca Estrutura do SharePoint que registra uma única instância de componentes do Microsoft Graph Toolkit no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="42204-118">The Microsoft Graph Toolkit SharePoint Framework package contains a SharePoint Framework library that registers a single instance of Microsoft Graph Toolkit components in SharePoint.</span></span>

<span data-ttu-id="42204-119">Instale o pacote npm do Microsoft Graph Toolkit Estrutura do SharePoint usando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="42204-119">Install the Microsoft Graph Toolkit SharePoint Framework npm package using the following command:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="42204-120">Adicionar o provedor SharePoint</span><span class="sxs-lookup"><span data-stu-id="42204-120">Add the SharePoint Provider</span></span>

<span data-ttu-id="42204-121">Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="42204-121">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="42204-122">Para saber mais, confira [Usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="42204-122">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="42204-123">SharePoint web parts sempre existem em um contexto autenticado porque o usuário já precisou entrar para acessar a página que hospeda sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="42204-123">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="42204-124">Use este contexto para inicializar o [provedor SharePoint .](../providers/sharepoint.md)</span><span class="sxs-lookup"><span data-stu-id="42204-124">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="42204-125">Primeiro, adicione o provedor à web part.</span><span class="sxs-lookup"><span data-stu-id="42204-125">First, add the provider to your web part.</span></span> <span data-ttu-id="42204-126">Localize o arquivo em sua pasta de projeto e adicione a seguinte linha à parte superior do arquivo, logo `src\webparts\<your-project>\<your-web-part>.ts` abaixo das instruções `import` existentes:</span><span class="sxs-lookup"><span data-stu-id="42204-126">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

<span data-ttu-id="42204-127">Em seguida, você precisa inicializar o provedor com o contexto autenticado dentro do `onInit()` método da web part.</span><span class="sxs-lookup"><span data-stu-id="42204-127">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="42204-128">No mesmo arquivo, adicione o seguinte código antes da `public render(): void {` linha:</span><span class="sxs-lookup"><span data-stu-id="42204-128">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a><span data-ttu-id="42204-129">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="42204-129">Add components</span></span>

<span data-ttu-id="42204-130">Agora, você pode começar a adicionar componentes à web part.</span><span class="sxs-lookup"><span data-stu-id="42204-130">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="42204-131">Basta adicionar os componentes ao HTML dentro do método e os componentes usarão o contexto SharePoint para acessar o `render()` Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="42204-131">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="42204-132">Por exemplo, para adicionar o [componente Person](../components/person.md), seu código terá a aparência:</span><span class="sxs-lookup"><span data-stu-id="42204-132">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

>[!NOTE]
> <span data-ttu-id="42204-133">Se você estiver criando uma Web Part usando React, consulte os documentos [@microsoft/mgt-spfx](./mgt-spfx.md#react) para saber como usar `@microsoft/mgt-react` .</span><span class="sxs-lookup"><span data-stu-id="42204-133">If you're building a web part using React, see the [@microsoft/mgt-spfx docs](./mgt-spfx.md#react) to learn how to use `@microsoft/mgt-react`.</span></span>

## <a name="configure-permissions"></a><span data-ttu-id="42204-134">Configurar permissões</span><span class="sxs-lookup"><span data-stu-id="42204-134">Configure permissions</span></span>

<span data-ttu-id="42204-135">Para chamar o Microsoft Graph de seu aplicativo Estrutura do SharePoint, você precisa solicitar as permissões necessárias no pacote de soluções e um administrador Microsoft 365 locatário precisa aprovar as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="42204-135">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="42204-136">Para adicionar as permissões ao pacote de solução, localize e abra o `config\package-solution.json` arquivo e desmarcar:</span><span class="sxs-lookup"><span data-stu-id="42204-136">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="42204-137">Logo abaixo dessa linha, adicione o seguinte:</span><span class="sxs-lookup"><span data-stu-id="42204-137">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="42204-138">Determine quais permissões de API do Microsoft Graph você precisa, dependendo dos componentes que você está usando.</span><span class="sxs-lookup"><span data-stu-id="42204-138">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="42204-139">A página de documentação de cada componente fornece uma lista das permissões que o componente exige.</span><span class="sxs-lookup"><span data-stu-id="42204-139">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="42204-140">Você precisará adicionar cada permissão necessária a `webApiPermissionRequests` .</span><span class="sxs-lookup"><span data-stu-id="42204-140">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="42204-141">Por exemplo, se você estiver usando o componente Person e o componente Agenda, pode `webApiPermissionRequests` ter a aparência:</span><span class="sxs-lookup"><span data-stu-id="42204-141">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a><span data-ttu-id="42204-142">Implantar o pacote microsoft Graph Toolkit Estrutura do SharePoint</span><span class="sxs-lookup"><span data-stu-id="42204-142">Deploy the Microsoft Graph Toolkit SharePoint Framework package</span></span>

<span data-ttu-id="42204-143">Antes de implantar seu pacote Estrutura do SharePoint no seu locatário, você precisará implantar o pacote microsoft Graph Toolkit Estrutura do SharePoint para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="42204-143">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the Microsoft Graph Toolkit SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="42204-144">Você pode baixar o pacote correspondente à versão do Microsoft Graph Toolkit que você usou em seu projeto, na seção [Versões](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="42204-144">You can download the package corresponding to the version of Microsoft Graph Toolkit that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="42204-145">Como apenas uma versão da biblioteca Estrutura do SharePoint do Microsoft Graph Toolkit pode ser instalada no locatário, antes de usar o Microsoft Graph Toolkit em sua solução, determine se sua organização ou cliente já tem uma versão da biblioteca Estrutura do SharePoint implantada e use a mesma versão.</span><span class="sxs-lookup"><span data-stu-id="42204-145">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

<span data-ttu-id="42204-146">Depois de baixar o pacote .sppkg do Microsoft Graph Toolkit Estrutura do SharePoint, carregue-o no catálogo de aplicativos SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="42204-146">After downloading the Microsoft Graph Toolkit SharePoint Framework .sppkg package, upload it to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="42204-147">Vá para a [página Mais recursos do seu SharePoint de administração.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)</span><span class="sxs-lookup"><span data-stu-id="42204-147">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="42204-148">Selecione **Abrir** em **Aplicativos,** clique em **Catálogo de Aplicativos** e **Distribuir aplicativos para SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="42204-148">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="42204-149">Upload seu `.sppkg` arquivo e clique em **Implantar**.</span><span class="sxs-lookup"><span data-stu-id="42204-149">Upload your `.sppkg` file, and click **Deploy**.</span></span>

## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="42204-150">Criar e implantar sua Web Part</span><span class="sxs-lookup"><span data-stu-id="42204-150">Build and deploy your web part</span></span>

<span data-ttu-id="42204-151">Agora, você criará seu aplicativo e o implantará SharePoint.</span><span class="sxs-lookup"><span data-stu-id="42204-151">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="42204-152">Crie seu aplicativo executando os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="42204-152">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="42204-153">Na `sharepoint/solution` pasta, haverá um novo `.sppkg` arquivo.</span><span class="sxs-lookup"><span data-stu-id="42204-153">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="42204-154">Você precisará carregar esse arquivo no catálogo de aplicativos SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="42204-154">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="42204-155">Vá para a [página Mais recursos do seu SharePoint de administração.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)</span><span class="sxs-lookup"><span data-stu-id="42204-155">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="42204-156">Selecione **Abrir** em **Aplicativos,** clique em **Catálogo de Aplicativos** e **Distribuir aplicativos para SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="42204-156">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="42204-157">Upload seu `.sppkg` arquivo e clique em **Implantar**.</span><span class="sxs-lookup"><span data-stu-id="42204-157">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="42204-158">Em seguida, você precisa aprovar as permissões como administrador.</span><span class="sxs-lookup"><span data-stu-id="42204-158">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="42204-159">Vá para o centro **de administração SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="42204-159">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="42204-160">Na navegação à esquerda, selecione **Avançado** e, em seguida, **Acesso à API**.</span><span class="sxs-lookup"><span data-stu-id="42204-160">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="42204-161">Você deve ver solicitações pendentes para cada uma das permissões adicionadas em seu `config\package-solution.json` arquivo.</span><span class="sxs-lookup"><span data-stu-id="42204-161">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="42204-162">Selecione e aprove cada permissão.</span><span class="sxs-lookup"><span data-stu-id="42204-162">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="42204-163">Testar sua Web Part</span><span class="sxs-lookup"><span data-stu-id="42204-163">Test your web part</span></span>

<span data-ttu-id="42204-164">Agora você está pronto para adicionar sua Web Part a uma SharePoint e testá-la. Você precisará usar o workbench hospedado para testar web parts que usam o microsoft Graph Toolkit porque os componentes precisam do contexto autenticado para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="42204-164">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="42204-165">Você pode encontrar seu workbench hospedado **em https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span><span class="sxs-lookup"><span data-stu-id="42204-165">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="42204-166">Abra o `config\serve.json` arquivo em seu projeto e substitua o valor de pela URL do seu `initialPage` workbench hospedado:</span><span class="sxs-lookup"><span data-stu-id="42204-166">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="42204-167">Salve o arquivo e execute o seguinte comando no console para criar e visualizar sua Web Part:</span><span class="sxs-lookup"><span data-stu-id="42204-167">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="42204-168">Seu workbench hospedado será aberto automaticamente no navegador.</span><span class="sxs-lookup"><span data-stu-id="42204-168">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="42204-169">Adicione sua Web Part à página e você deverá ver sua Web Part com os componentes Graph Toolkit Microsoft em ação!</span><span class="sxs-lookup"><span data-stu-id="42204-169">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="42204-170">Enquanto o comando gulp serve ainda está em execução no console, você pode continuar a fazer edições para seu código e, em seguida, apenas atualizar seu navegador para ver suas alterações.</span><span class="sxs-lookup"><span data-stu-id="42204-170">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="42204-171">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="42204-171">Next Steps</span></span>
- <span data-ttu-id="42204-172">Confira este tutorial passo a passo sobre [como criar uma web part SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span><span class="sxs-lookup"><span data-stu-id="42204-172">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="42204-173">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="42204-173">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="42204-174">Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="42204-174">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="42204-175">Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="42204-175">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
