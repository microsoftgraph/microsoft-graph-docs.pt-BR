---
title: Criar uma Web Part do SharePoint com o kit de ferramentas do Microsoft Graph
description: Introdução ao uso do kit de ferramentas do Microsoft Graph para criar uma Web Part do SharePoint.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: b2ae71a8fb37e088c0497716fdf4d1cdc42f41ef
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288522"
---
# <a name="build-a-sharepoint-web-part-with-the-microsoft-graph-toolkit"></a><span data-ttu-id="bad91-103">Criar uma Web Part do SharePoint com o kit de ferramentas do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bad91-103">Build a SharePoint web part with the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bad91-104">Este tópico aborda como usar os componentes do Microsoft Graph Toolkit em uma [Web Part do lado do cliente do SharePoint](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span><span class="sxs-lookup"><span data-stu-id="bad91-104">This topic covers how to use Microsoft Graph Toolkit components in a [SharePoint client-side web part](/sharepoint/dev/spfx/web-parts/overview-client-side-web-parts).</span></span> <span data-ttu-id="bad91-105">Introdução envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="bad91-105">Getting started involves the following steps:</span></span>

1. <span data-ttu-id="bad91-106">Configurar seu ambiente de desenvolvimento e criar uma Web Part.</span><span class="sxs-lookup"><span data-stu-id="bad91-106">Set up your development environment and create a web part.</span></span>
2. <span data-ttu-id="bad91-107">Atualize o TypeScript em seu projeto.</span><span class="sxs-lookup"><span data-stu-id="bad91-107">Update TypeScript in your project.</span></span>
3. <span data-ttu-id="bad91-108">Adicione o Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="bad91-108">Add the Microsoft Graph Toolkit.</span></span>
4. <span data-ttu-id="bad91-109">Adicione o provedor do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bad91-109">Add the SharePoint Provider.</span></span>
5. <span data-ttu-id="bad91-110">Adicionar componentes.</span><span class="sxs-lookup"><span data-stu-id="bad91-110">Add components.</span></span>
6. <span data-ttu-id="bad91-111">Configurar permissões.</span><span class="sxs-lookup"><span data-stu-id="bad91-111">Configure permissions.</span></span>
7. <span data-ttu-id="bad91-112">Criar e implantar sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="bad91-112">Build and deploy your web part.</span></span>
8. <span data-ttu-id="bad91-113">Testar sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="bad91-113">Test your web part.</span></span>

## <a name="set-up-your-sharepoint-framework-development-environment-and-create-a-new-web-part"></a><span data-ttu-id="bad91-114">Configurar seu ambiente de desenvolvimento da estrutura do SharePoint e criar uma nova Web Part</span><span class="sxs-lookup"><span data-stu-id="bad91-114">Set up your SharePoint Framework development environment and create a new web part</span></span>

<span data-ttu-id="bad91-115">Siga as etapas para [configurar seu ambiente de desenvolvimento da estrutura do SharePoint](/sharepoint/dev/spfx/set-up-your-development-environment) e, em seguida, [criar uma nova Web Part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span><span class="sxs-lookup"><span data-stu-id="bad91-115">Follow the steps to [Set up your SharePoint Framework development environment](/sharepoint/dev/spfx/set-up-your-development-environment) and then [create a new web part](/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part).</span></span>

## <a name="update-typescript-in-your-project"></a><span data-ttu-id="bad91-116">Atualizar TypeScript em seu projeto</span><span class="sxs-lookup"><span data-stu-id="bad91-116">Update TypeScript in your project</span></span>

<span data-ttu-id="bad91-117">O Microsoft Graph Toolkit requer o typescript 3. x.</span><span class="sxs-lookup"><span data-stu-id="bad91-117">The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="bad91-118">Antes de adicionar o kit de ferramentas ao seu projeto, verifique se você está usando uma [versão com suporte do typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span><span class="sxs-lookup"><span data-stu-id="bad91-118">Before adding the Toolkit to your project, make sure you're using a [supported version of Typescript](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span> <span data-ttu-id="bad91-119">Por exemplo, para adicionar o typescript 3,7, use o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="bad91-119">For example, to add Typescript 3.7, use the following command:</span></span>

```bash
npm install @microsoft/rush-stack-compiler-3.7 --save-dev
```
<span data-ttu-id="bad91-120">Em seguida, localize o `tsconfig.json` arquivo na pasta do projeto, abra o arquivo e procure esta linha:</span><span class="sxs-lookup"><span data-stu-id="bad91-120">Then, locate the `tsconfig.json` file in your project folder, open the file, and look for this line:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.3/includes/tsconfig-web.json",
```
<span data-ttu-id="bad91-121">Substitua a linha por:</span><span class="sxs-lookup"><span data-stu-id="bad91-121">Replace the line with:</span></span>

```json
"extends": "./node_modules/@microsoft/rush-stack-compiler-3.7/includes/tsconfig-web.json",
```

## <a name="add-the-microsoft-graph-toolkit"></a><span data-ttu-id="bad91-122">Adicionar o Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="bad91-122">Add the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="bad91-123">Instale o pacote NPM do Microsoft Graph Toolkit e os metapreenchimentos com o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="bad91-123">Install the Microsoft Graph Toolkit npm package and polyfills with the following command:</span></span>

```bash
npm install @microsoft/mgt
```
<span data-ttu-id="bad91-124">Se você planeja suportar o IE11 em suas Web Parts, será necessário seguir etapas adicionais para garantir a compatibilidade entre navegadores:</span><span class="sxs-lookup"><span data-stu-id="bad91-124">If you plan to support IE11 in your web parts, you'll need to follow additional steps to ensure cross-browser compatibility:</span></span>

1. <span data-ttu-id="bad91-125">Instale os seguintes pacotes:</span><span class="sxs-lookup"><span data-stu-id="bad91-125">Install the following packages:</span></span>
```bash
npm install -D babel-loader @babel/core @babel/preset-env webpack
npm install -D @webcomponents/webcomponentsjs regenerator-runtime core-js
```

2. <span data-ttu-id="bad91-126">Adicione o seguinte código ao `gulpfile.js` , imediatamente acima `build.initialize(gulp)` :</span><span class="sxs-lookup"><span data-stu-id="bad91-126">Add the following code to `gulpfile.js`, right above `build.initialize(gulp)`:</span></span>
```ts
build.configureWebpack.mergeConfig({
  additionalConfiguration: (generatedConfiguration) => {
    generatedConfiguration.module.rules.push(
      {
        test: /\.m?js$/, use:
        {
          loader: "babel-loader",
          options:
          {
            presets: [["@babel/preset-env",
              {
                targets: {
                  "ie": "11"
                }
              }]]
          }
        }
      }
    );

    return generatedConfiguration;
  }
});
```
3. <span data-ttu-id="bad91-127">No `src\webparts\<your-project>\<your-web-part>.ts` arquivo, importe os seguintes metapreenchimentos antes do provedor do SharePoint na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="bad91-127">In your `src\webparts\<your-project>\<your-web-part>.ts` file, import the following polyfills before the SharePoint provider in the next step.</span></span>

```ts
import 'regenerator-runtime/runtime';
import 'core-js/es/number';
import 'core-js/es/math';
import 'core-js/es/string';
import 'core-js/es/date';
import 'core-js/es/array';
import 'core-js/es/regexp';
import '@webcomponents/webcomponentsjs/webcomponents-bundle.js';
```

## <a name="add-the-sharepoint-provider"></a><span data-ttu-id="bad91-128">Adicionar o provedor do SharePoint</span><span class="sxs-lookup"><span data-stu-id="bad91-128">Add the SharePoint Provider</span></span>

<span data-ttu-id="bad91-129">Os provedores do Microsoft Graph Toolkit permitem a autenticação e o acesso ao Microsoft Graph para os componentes.</span><span class="sxs-lookup"><span data-stu-id="bad91-129">The Microsoft Graph Toolkit providers enable authentication and access to Microsoft Graph for the components.</span></span> <span data-ttu-id="bad91-130">Para saber mais, consulte [usando os provedores](../providers.md).</span><span class="sxs-lookup"><span data-stu-id="bad91-130">To learn more, see [Using the providers](../providers.md).</span></span> <span data-ttu-id="bad91-131">Web Parts do SharePoint sempre existem em um contexto autenticado porque o usuário já teve que entrar para acessar a página que hospeda sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="bad91-131">SharePoint web parts always exist in an authenticated context because the user has already had to sign in in order to get to the page that hosts your web part.</span></span> <span data-ttu-id="bad91-132">Use este contexto para inicializar o [provedor do SharePoint](../providers/sharepoint.md).</span><span class="sxs-lookup"><span data-stu-id="bad91-132">Use this context to initialize the [SharePoint provider](../providers/sharepoint.md).</span></span>

<span data-ttu-id="bad91-133">Primeiro, adicione o provedor à Web Part.</span><span class="sxs-lookup"><span data-stu-id="bad91-133">First, add the provider to your web part.</span></span> <span data-ttu-id="bad91-134">Localize o `src\webparts\<your-project>\<your-web-part>.ts` arquivo na pasta do projeto e adicione a seguinte linha na parte superior do arquivo, logo abaixo das `import` instruções existentes:</span><span class="sxs-lookup"><span data-stu-id="bad91-134">Locate the `src\webparts\<your-project>\<your-web-part>.ts` file in your project folder, and add the following line to the top of your file, right below the existing `import` statements:</span></span>

```ts
import { Providers, SharePointProvider } from '@microsoft/mgt';
```

<span data-ttu-id="bad91-135">Em seguida, você precisa inicializar o provedor com o contexto autenticado dentro do `onInit()` método de sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="bad91-135">Next, you need to initialize the provider with the authenticated context inside the `onInit()` method of your web part.</span></span> <span data-ttu-id="bad91-136">No mesmo arquivo, adicione o seguinte código imediatamente antes da `public render(): void {` linha:</span><span class="sxs-lookup"><span data-stu-id="bad91-136">In the same file, add the following code right before the `public render(): void {` line:</span></span>

```ts
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context)
}
```

## <a name="add-components"></a><span data-ttu-id="bad91-137">Adicionar componentes</span><span class="sxs-lookup"><span data-stu-id="bad91-137">Add components</span></span>

<span data-ttu-id="bad91-138">Agora, você pode começar a adicionar componentes à sua Web Part.</span><span class="sxs-lookup"><span data-stu-id="bad91-138">Now, you can start adding components to your web part.</span></span> <span data-ttu-id="bad91-139">Basta adicionar os componentes ao HTML dentro do `render()` método e os componentes usarão o contexto do SharePoint para acessar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bad91-139">Simply add the components to the HTML inside of the `render()` method, and the components will use the SharePoint context to access Microsoft Graph.</span></span> <span data-ttu-id="bad91-140">Por exemplo, para adicionar o [componente pessoa](../components/person.md), seu código terá a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="bad91-140">For example, to add the [Person component](../components/person.md), your code will look like:</span></span>

```ts
public render(): void {
    this.domElement.innerHTML = `
      <mgt-person person-query="me" view="twolines"><mgt-person>
    `;
}
```

## <a name="configure-permissions"></a><span data-ttu-id="bad91-141">Configurar permissões</span><span class="sxs-lookup"><span data-stu-id="bad91-141">Configure permissions</span></span>

<span data-ttu-id="bad91-142">Para chamar o Microsoft Graph a partir do seu aplicativo da estrutura do SharePoint, você precisa solicitar as permissões necessárias no pacote de solução e um administrador de locatários do Microsoft 365 precisa aprovar as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="bad91-142">To call Microsoft Graph from your SharePoint Framework application, you need to request the needed permissions in your solution package and a Microsoft 365 tenant administrator needs to approve the requested permissions.</span></span>

<span data-ttu-id="bad91-143">Para adicionar as permissões ao seu pacote de solução, localize e abra o `config\package-solution.json` arquivo e defina:</span><span class="sxs-lookup"><span data-stu-id="bad91-143">To add the permissions to your solution package, locate and open the `config\package-solution.json` file and set:</span></span>

```json
"isDomainIsolated": false,
```

<span data-ttu-id="bad91-144">Logo abaixo dessa linha, adicione o seguinte:</span><span class="sxs-lookup"><span data-stu-id="bad91-144">Just below that line, add the following:</span></span>

```json
"webApiPermissionRequests":[],
```

<span data-ttu-id="bad91-145">Determine quais permissões de API do Microsoft Graph você precisa dependendo dos componentes que você está usando.</span><span class="sxs-lookup"><span data-stu-id="bad91-145">Determine which Microsoft Graph API permissions you need depending on the components you're using.</span></span> <span data-ttu-id="bad91-146">A página de documentação de cada componente fornece uma lista das permissões exigidas pelo componente.</span><span class="sxs-lookup"><span data-stu-id="bad91-146">Each component's documentation page provides a list of the permissions that component requires.</span></span> <span data-ttu-id="bad91-147">Será necessário adicionar cada permissão necessária para o `webApiPermissionRequests` .</span><span class="sxs-lookup"><span data-stu-id="bad91-147">You will need to add each permission required to `webApiPermissionRequests`.</span></span> <span data-ttu-id="bad91-148">Por exemplo, se você estiver usando o componente Person e o componente de agenda, você `webApiPermissionRequests` pode ter a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="bad91-148">For example, if you're using the Person component and the Agenda component, your `webApiPermissionRequests` might look like:</span></span>

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
## <a name="build-and-deploy-your-web-part"></a><span data-ttu-id="bad91-149">Criar e implantar sua Web Part</span><span class="sxs-lookup"><span data-stu-id="bad91-149">Build and deploy your web part</span></span>

<span data-ttu-id="bad91-150">Agora, você irá criar seu aplicativo e implantá-lo no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bad91-150">Now, you will build your application and deploy it to SharePoint.</span></span> <span data-ttu-id="bad91-151">Crie seu aplicativo executando os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="bad91-151">Build your application by running the following commands:</span></span>

```bash
gulp build
gulp bundle
gulp package-solution
```

<span data-ttu-id="bad91-152">Na `sharepoint/solution` pasta, haverá um novo `.sppkg` arquivo.</span><span class="sxs-lookup"><span data-stu-id="bad91-152">In the `sharepoint/solution` folder, there will be a new `.sppkg` file.</span></span> <span data-ttu-id="bad91-153">Você precisará carregar esse arquivo no catálogo de aplicativos do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="bad91-153">You will need to upload this file to your SharePoint Online App Catalog.</span></span> <span data-ttu-id="bad91-154">Vá para a [página mais recursos do seu centro de administração do SharePoint](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span><span class="sxs-lookup"><span data-stu-id="bad91-154">Go to the [More features page of your SharePoint admin center](https://admin.microsoft.com/sharepoint?page=classicfeatures&modern=true).</span></span> <span data-ttu-id="bad91-155">Selecione **abrir** em **aplicativos**, clique em **Catálogo de aplicativos**e **distribua aplicativos para SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="bad91-155">Select **Open** under **Apps**, then click **App Catalog**, and **Distribute apps for SharePoint**.</span></span> <span data-ttu-id="bad91-156">Carregue o `.sppkg` arquivo e clique em **implantar**.</span><span class="sxs-lookup"><span data-stu-id="bad91-156">Upload your `.sppkg` file, and click **Deploy**.</span></span>

<span data-ttu-id="bad91-157">Em seguida, você precisa aprovar as permissões como um administrador.</span><span class="sxs-lookup"><span data-stu-id="bad91-157">Next, you need to approve the permissions as an administrator.</span></span>

<span data-ttu-id="bad91-158">Vá para o **centro de administração do SharePoint**.</span><span class="sxs-lookup"><span data-stu-id="bad91-158">Go to your **SharePoint Admin center**.</span></span> <span data-ttu-id="bad91-159">Na navegação à esquerda, selecione **avançado** e, em seguida, **acesso à API**.</span><span class="sxs-lookup"><span data-stu-id="bad91-159">In the left-hand navigation, select **Advanced** and then **API Access**.</span></span> <span data-ttu-id="bad91-160">Você deve ver as solicitações pendentes para cada uma das permissões adicionadas ao `config\package-solution.json` arquivo.</span><span class="sxs-lookup"><span data-stu-id="bad91-160">You should see pending requests for each of the permissions you added in your `config\package-solution.json` file.</span></span> <span data-ttu-id="bad91-161">Selecione e aprove cada permissão.</span><span class="sxs-lookup"><span data-stu-id="bad91-161">Select and approve each permission.</span></span>

## <a name="test-your-web-part"></a><span data-ttu-id="bad91-162">Testar sua Web Part</span><span class="sxs-lookup"><span data-stu-id="bad91-162">Test your web part</span></span>

<span data-ttu-id="bad91-163">Agora você está pronto para adicionar a Web Part a uma página do SharePoint e testá-la. Você precisará usar o Workbench hospedado para testar Web Parts que usam o Microsoft Graph Toolkit porque os componentes precisam do contexto autenticado para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bad91-163">You're now ready to add your web part to a SharePoint page and test it out. You will need to use the hosted workbench to test web parts that use the Microsoft Graph Toolkit because the components need the authenticated context in order to call Microsoft Graph.</span></span> <span data-ttu-id="bad91-164">Você pode encontrar o Workbench hospedado em **https://<YOUR_TENANT>. SharePoint.com/_layouts/15/Workbench.aspx**.</span><span class="sxs-lookup"><span data-stu-id="bad91-164">You can find your hosted workbench at **https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx**.</span></span>

<span data-ttu-id="bad91-165">Abra o `config\serve.json` arquivo no seu projeto e substitua o valor de `initialPage` pela URL do seu Workbench hospedado:</span><span class="sxs-lookup"><span data-stu-id="bad91-165">Open the `config\serve.json` file in your project and replace the  value of `initialPage` with the url for your hosted workbench:</span></span>
```json
"initialPage": "https://<YOUR_TENANT>.sharepoint.com/_layouts/15/workbench.aspx",
```
<span data-ttu-id="bad91-166">Salve o arquivo e, em seguida, execute o seguinte comando no console para compilar e visualizar sua Web Part:</span><span class="sxs-lookup"><span data-stu-id="bad91-166">Save the file and then run the following command in the console to build and preview your web part:</span></span>

```bash
gulp serve
```

<span data-ttu-id="bad91-167">O Workbench hospedado será aberto automaticamente no navegador.</span><span class="sxs-lookup"><span data-stu-id="bad91-167">Your hosted workbench will automatically open in your browser.</span></span> <span data-ttu-id="bad91-168">Adicione sua Web Part à página e você deverá ver sua Web Part com os componentes do Microsoft Graph Toolkit em ação!</span><span class="sxs-lookup"><span data-stu-id="bad91-168">Add your web part to the page and you should see your web part with the Microsoft Graph Toolkit components in action!</span></span> <span data-ttu-id="bad91-169">Contanto que o comando Gulp sirva ainda esteja em execução no seu console, você pode continuar a fazer edições no seu código e, em seguida, apenas atualizar seu navegador para ver suas alterações.</span><span class="sxs-lookup"><span data-stu-id="bad91-169">As long as the gulp serve command is still running in your console, you can continue to make edits to your code and then just refresh your browser to see your changes.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bad91-170">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="bad91-170">Next Steps</span></span>
- <span data-ttu-id="bad91-171">Confira este tutorial passo a passo sobre a [criação de uma Web Part do SharePoint](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span><span class="sxs-lookup"><span data-stu-id="bad91-171">Check out this step-by-step tutorial on [building a SharePoint web part](https://developer.microsoft.com/graph/blogs/a-lap-around-microsoft-graph-toolkit-day-9-microsoft-graph-toolkit-sharepoint-provider/).</span></span>
- <span data-ttu-id="bad91-172">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="bad91-172">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="bad91-173">Faça uma pergunta sobre o [estouro de pilha](https://aka.ms/mgt-question).</span><span class="sxs-lookup"><span data-stu-id="bad91-173">Ask a question on [Stack Overflow](https://aka.ms/mgt-question).</span></span>
- <span data-ttu-id="bad91-174">Informe bugs ou deixe uma solicitação de recurso no [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="bad91-174">Report bugs or leave a feature request on [GitHub](https://aka.ms/mgt).</span></span>