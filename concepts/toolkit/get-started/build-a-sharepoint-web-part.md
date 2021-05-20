---
title: Criar uma web part SharePoint com o microsoft Graph Toolkit
description: Começar a usar o microsoft Graph Toolkit para criar uma web part SharePoint web part.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 4c5443e05a57aade5c09d04f337c6a8bb67584c6
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579911"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="fb4f0-103">Criar uma web part SharePoint com o microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="fb4f0-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="fb4f0-104">Este tópico aborda como usar os componentes do Microsoft Graph Toolkit em uma [web part SharePoint do lado do cliente.](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts)</span><span class="sxs-lookup"><span data-stu-id="fb4f0-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="fb4f0-105">Começar envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="fb4f0-106">Configurar seu ambiente de desenvolvimento e criar uma Web Part.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-106">Set up your development environment and create a web part.</span></span>
1. <span data-ttu-id="fb4f0-107">Adicione o pacote microsoft Graph Toolkit Estrutura do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-107">Add the Microsoft Graph Toolkit SharePoint Framework package.</span></span>
1. <span data-ttu-id="fb4f0-108">Adicione o SharePoint Provedor.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-108">Add the SharePoint Provider.</span></span>
1. <span data-ttu-id="fb4f0-109">Adicione componentes.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-109">Add components.</span></span>
1. <span data-ttu-id="fb4f0-110">Configurar permissões.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-110">Configure permissions.</span></span>
1. <span data-ttu-id="fb4f0-111">Implante o pacote microsoft Graph Toolkit Estrutura do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-111">Deploy the Microsoft Graph Toolkit SharePoint Framework package.</span></span>
1. <span data-ttu-id="fb4f0-112">Crie e implante sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-112">Build and deploy your web part.</span></span>
1. <span data-ttu-id="fb4f0-113">Teste sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="fb4f0-114">Configurar seu ambiente de Estrutura do SharePoint de desenvolvimento e criar uma nova Web Part</span><span class="sxs-lookup"><span data-stu-id="fb4f0-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="fb4f0-115">Siga as etapas para Configurar seu ambiente de [Estrutura do SharePoint de desenvolvimento](/sharepoint/dev/spfx/set-up-your-development-environment) e, em seguida, criar uma nova Web [Part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span><span class="sxs-lookup"><span data-stu-id="fb4f0-115">Follow the steps to [Set up your SharePoint Framework development environment](/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="add-the-microsoft-graph-toolkit-sharepoint-framework-package"></a><span data-ttu-id="fb4f0-116">Adicionar o pacote microsoft Graph Toolkit Estrutura do SharePoint</span><span class="sxs-lookup"><span data-stu-id="fb4f0-116">Add the Microsoft Graph Toolkit SharePoint Framework package</span></span>

<span data-ttu-id="fb4f0-117">Para impedir que vários componentes Estrutura do SharePoint registrem seu próprio conjunto de componentes do Microsoft Graph Toolkit na página, você deve implantar o pacote do Microsoft Graph Toolkit Estrutura do SharePoint para seu locatário e fazer referência aos componentes do Microsoft Graph Toolkit que você usa em sua solução a partir deste pacote.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-117">To prevent multiple SharePoint Framework components from registering their own set of Microsoft Graph Toolkit components on the page, you should deploy the Microsoft Graph Toolkit SharePoint Framework package to your tenant and reference Microsoft Graph Toolkit components that you use in your solution from this package.</span></span>

<span data-ttu-id="fb4f0-118">O pacote Graph Toolkit Estrutura do SharePoint microsoft contém uma biblioteca Estrutura do SharePoint que registra uma única instância de componentes do Microsoft Graph Toolkit no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-118">The Microsoft Graph Toolkit SharePoint Framework package contains a SharePoint Framework library that registers a single instance of Microsoft Graph Toolkit components in SharePoint.</span></span>

<span data-ttu-id="fb4f0-119">Instale o pacote npm do Microsoft Graph Toolkit Estrutura do SharePoint usando o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-119">Install the Microsoft Graph Toolkit SharePoint Framework npm package using the following command:</span></span>

```bash
npm install @microsoft/mgt-spfx
```

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="fb4f0-120">Adicionar o provedor SharePoint</span><span class="sxs-lookup"><span data-stu-id="fb4f0-120">Add the SharePoint Provider</span></span>

<span data-ttu-id="fb4f0-121">Os provedores Graph Toolkit Microsoft habilitam a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-121">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="fb4f0-122">Para saber mais, confira [Usando os provedores](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="fb4f0-122">To learn more, see [Using the providers](../providers/providers.md).</span></span> <span data-ttu-id="fb4f0-123">SharePoint web parts sempre existem em um contexto autenticado porque o usuário já precisou entrar para acessar a página que hospeda sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-123">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="fb4f0-124">Use este contexto para inicializar o [provedor SharePoint .](../providers/sharepoint.md)</span><span class="sxs-lookup"><span data-stu-id="fb4f0-124">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="fb4f0-125">Primeiro, adicione o provedor à web part.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-125">First, add the provider to your web part.</span></span> <span data-ttu-id="fb4f0-126">Localize o arquivo em sua pasta de projeto e adicione a seguinte linha à parte superior do arquivo, logo `src\webparts\<your-project>\<your-web-part>.ts` abaixo das instruções `import` existentes:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-126">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt-spfx';
```

<span data-ttu-id="fb4f0-127">Em seguida, você precisa inicializar o provedor com o contexto autenticado dentro do `onInit()` método da web part.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-127">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="fb4f0-128">No mesmo arquivo, adicione o seguinte código antes da `public render(): void {` linha:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-128">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
  if (!Providers.globalProvider) {
    Providers.globalProvider = new SharePointProvider(this.context);
  }
}
```

## <a name="add-components"></a><span data-ttu-id="fb4f0-129">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="fb4f0-129">Add components</span></span>

<span data-ttu-id="fb4f0-130">Agora, você pode começar a adicionar componentes à web part.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-130">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="fb4f0-131">Basta adicionar os componentes ao HTML dentro do método e os componentes usarão o contexto SharePoint para acessar o `render()` Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-131">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="fb4f0-132">Por exemplo, para adicionar o [componente Person](../components/person.md), seu código terá a aparência:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-132">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"></mgt-person>
    `;
}
```

## <a name="configure-permissions"></a><span data-ttu-id="fb4f0-133">Configurar permissões</span><span class="sxs-lookup"><span data-stu-id="fb4f0-133">Configure permissions</span></span>

<span data-ttu-id="fb4f0-134">Para chamar o Microsoft Graph de seu aplicativo Estrutura do SharePoint, você precisa solicitar as permissões necessárias no pacote de soluções e um administrador Microsoft 365 locatário precisa aprovar as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-134">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="fb4f0-135">Para adicionar as permissões ao pacote de solução, localize e abra o `config\package-solution.json` arquivo e desmarcar:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-135">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="fb4f0-136">Logo abaixo dessa linha, adicione o seguinte:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-136">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="fb4f0-137">Determine quais permissões de API do Microsoft Graph você precisa, dependendo dos componentes que você está usando.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-137">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="fb4f0-138">A página de documentação de cada componente fornece uma lista das permissões que o componente exige.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-138">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="fb4f0-139">Você precisará adicionar cada permissão necessária a `webApiPermissionRequests` .</span><span class="sxs-lookup"><span data-stu-id="fb4f0-139">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="fb4f0-140">Por exemplo, se você estiver usando o componente Person e o componente Agenda, pode `webApiPermissionRequests` ter a aparência:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-140">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

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

## <a name="deploy-the-microsoft-graph-toolkit-sharepoint-framework-package"></a><span data-ttu-id="fb4f0-141">Implantar o pacote microsoft Graph Toolkit Estrutura do SharePoint</span><span class="sxs-lookup"><span data-stu-id="fb4f0-141">Deploy the Microsoft Graph Toolkit SharePoint Framework package</span></span>

<span data-ttu-id="fb4f0-142">Antes de implantar seu pacote Estrutura do SharePoint no seu locatário, você precisará implantar o pacote microsoft Graph Toolkit Estrutura do SharePoint para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-142">Before deploying your SharePoint Framework package to your tenant, you will need to deploy the Microsoft Graph Toolkit SharePoint Framework package to your tenant.</span></span> <span data-ttu-id="fb4f0-143">Você pode baixar o pacote correspondente à versão do Microsoft Graph Toolkit que você usou em seu projeto, na seção [Versões](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-143">You can download the package corresponding to the version of Microsoft Graph Toolkit that you used in your project, from the [Releases](https://github.com/microsoftgraph/microsoft-graph-toolkit/releases) section on GitHub.</span></span>

>[!IMPORTANT]
><span data-ttu-id="fb4f0-144">Como apenas uma versão da biblioteca Estrutura do SharePoint do Microsoft Graph Toolkit pode ser instalada no locatário, antes de usar o Microsoft Graph Toolkit em sua solução, determine se sua organização ou cliente já tem uma versão da biblioteca Estrutura do SharePoint implantada e use a mesma versão.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-144">Because only one version of the SharePoint Framework library for Microsoft Graph Toolkit can be installed in the tenant, before you use the Microsoft Graph Toolkit in your solution, determine whether your organization or customer already has a version of the SharePoint Framework library deployed and use the same version.</span></span>

<span data-ttu-id="fb4f0-145">Depois de baixar o pacote .sppkg do Microsoft Graph Toolkit Estrutura do SharePoint, carregue-o no catálogo de aplicativos SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-145">After downloading the Microsoft Graph Toolkit SharePoint Framework .sppkg package, upload it to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="fb4f0-146">Vá para a [página Mais recursos do seu SharePoint de administração.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)</span><span class="sxs-lookup"><span data-stu-id="fb4f0-146">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="fb4f0-147">Selecione **Abrir** em **Aplicativos,** clique em **Catálogo de Aplicativos** e **Distribuir aplicativos para SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-147">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="fb4f0-148">Upload seu `.sppkg` arquivo e clique em **Implantar**.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-148">Upload your `.sppkg` file, and click **Deploy**.</span></span>

## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="fb4f0-149">Criar e implantar sua Web Part</span><span class="sxs-lookup"><span data-stu-id="fb4f0-149">Build and deploy your web part</span></span>

<span data-ttu-id="fb4f0-150">Agora, você criará seu aplicativo e o implantará SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-150">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="fb4f0-151">Crie seu aplicativo executando os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-151">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="fb4f0-152">Na `sharepoint/solution` pasta, haverá um novo `.sppkg` arquivo.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-152">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="fb4f0-153">Você precisará carregar esse arquivo no catálogo de aplicativos SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-153">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="fb4f0-154">Vá para a [página Mais recursos do seu SharePoint de administração.](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true)</span><span class="sxs-lookup"><span data-stu-id="fb4f0-154">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="fb4f0-155">Selecione **Abrir** em **Aplicativos,** clique em **Catálogo de Aplicativos** e **Distribuir aplicativos para SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-155">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="fb4f0-156">Upload seu `.sppkg` arquivo e clique em **Implantar**.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-156">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="fb4f0-157">Em seguida, você precisa aprovar as permissões como administrador.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-157">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="fb4f0-158">Vá para o centro **de administração SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="fb4f0-158">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="fb4f0-159">Na navegação à esquerda, selecione **Avançado** e, em seguida, **Acesso à API**.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-159">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="fb4f0-160">Você deve ver solicitações pendentes para cada uma das permissões adicionadas em seu `config\package-solution.json` arquivo.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-160">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="fb4f0-161">Selecione e aprove cada permissão.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-161">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="fb4f0-162">Testar sua Web Part</span><span class="sxs-lookup"><span data-stu-id="fb4f0-162">Test your web part</span></span>

<span data-ttu-id="fb4f0-163">Agora você está pronto para adicionar sua Web Part a uma SharePoint e testá-la. Você precisará usar o workbench hospedado para testar web parts que usam o microsoft Graph Toolkit porque os componentes precisam do contexto autenticado para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-163">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="fb4f0-164">Você pode encontrar seu workbench hospedado **em https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-164">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="fb4f0-165">Abra o `config\serve.json` arquivo em seu projeto e substitua o valor de pela URL do seu `initialPage` workbench hospedado:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-165">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="fb4f0-166">Salve o arquivo e execute o seguinte comando no console para criar e visualizar sua Web Part:</span><span class="sxs-lookup"><span data-stu-id="fb4f0-166">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="fb4f0-167">Seu workbench hospedado será aberto automaticamente no navegador.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-167">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="fb4f0-168">Adicione sua Web Part à página e você deverá ver sua Web Part com os componentes Graph Toolkit Microsoft em ação!</span><span class="sxs-lookup"><span data-stu-id="fb4f0-168">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="fb4f0-169">Enquanto o comando gulp serve ainda está em execução no console, você pode continuar a fazer edições para seu código e, em seguida, apenas atualizar seu navegador para ver suas alterações.</span><span class="sxs-lookup"><span data-stu-id="fb4f0-169">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fb4f0-170">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="fb4f0-170">Next Steps</span></span>
- <span data-ttu-id="fb4f0-171">Confira este tutorial passo a passo sobre [como criar uma web part SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span><span class="sxs-lookup"><span data-stu-id="fb4f0-171">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="fb4f0-172">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="fb4f0-172">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="fb4f0-173">Faça uma pergunta sobre [Stack Overflow](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="fb4f0-173">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="fb4f0-174">Relatar bugs ou deixar uma solicitação de recurso [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="fb4f0-174">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>
