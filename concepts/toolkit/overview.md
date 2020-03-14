---
title: 'Kit de ferramentas do Microsoft Graph: Web Components da plataforma Microsoft Graph'
description: O kit de ferramentas do Microsoft Graph é uma coleção de resuable, componentes da Web e auxiliares de estrutura independente para acessar e trabalhar com o Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 348e08212010f66fdde5ee3b752fe901699fbaa9
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639546"
---
# <a name="microsoft-graph-toolkit-web-components-powered-by-microsoft-graph"></a><span data-ttu-id="ddc8a-103">Kit de ferramentas do Microsoft Graph: Web Components da plataforma Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ddc8a-103">Microsoft Graph Toolkit: Web Components powered by Microsoft Graph</span></span>

<span data-ttu-id="ddc8a-104">O kit de ferramentas do Microsoft Graph é uma coleção de componentes da Web e auxiliares reutilizáveis da estrutura, que podem acessar e trabalhar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="ddc8a-105">Os componentes são totalmente funcionais à direita da caixa, com provedores internos que autenticam e buscam dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="ddc8a-106">O Microsoft Graph Toolkit torna fácil usar o Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="ddc8a-107">No exemplo abaixo, Confira como um usuário conectado e seus eventos de calendário são exibidos com apenas duas linhas de código usando os componentes de [login](./components/login.md) e [agenda](./components/agenda.md) .</span><span class="sxs-lookup"><span data-stu-id="ddc8a-107">In the example below, see how a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="ddc8a-108">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="ddc8a-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ddc8a-109">O que há no Microsoft Graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="ddc8a-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="ddc8a-110">Componentes</span><span class="sxs-lookup"><span data-stu-id="ddc8a-110">Components</span></span>

<span data-ttu-id="ddc8a-111">O kit de ferramentas do Microsoft Graph inclui uma coleção de componentes Web para as experiências mais compiladas com as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span>

|<span data-ttu-id="ddc8a-112">Componente</span><span class="sxs-lookup"><span data-stu-id="ddc8a-112">Component</span></span>|<span data-ttu-id="ddc8a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddc8a-113">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="ddc8a-114">Logon</span><span class="sxs-lookup"><span data-stu-id="ddc8a-114">Login</span></span>](./components/login.md)|<span data-ttu-id="ddc8a-115">Um botão e um controle de submenu para autenticar um usuário com a plataforma de identidade da Microsoft e exibir as informações de perfil do usuário em entrar.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-115">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="ddc8a-116">Pessoa</span><span class="sxs-lookup"><span data-stu-id="ddc8a-116">Person</span></span>](./components/person.md)|<span data-ttu-id="ddc8a-117">Exibe uma pessoa ou contato por sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-117">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="ddc8a-118">Pessoas</span><span class="sxs-lookup"><span data-stu-id="ddc8a-118">People</span></span>](./components/people.md)|<span data-ttu-id="ddc8a-119">Exibe um grupo de pessoas ou contatos por suas fotos ou iniciais.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-119">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="ddc8a-120">Agenda</span><span class="sxs-lookup"><span data-stu-id="ddc8a-120">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="ddc8a-121">Exibe eventos no calendário de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-121">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="ddc8a-122">Tarefas</span><span class="sxs-lookup"><span data-stu-id="ddc8a-122">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="ddc8a-123">Exibe e permite adicionar, remover, concluir ou editar tarefas do Microsoft Planner ou do Microsoft to-do.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-123">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To-Do.</span></span>|
|[<span data-ttu-id="ddc8a-124">Seletor de pessoas</span><span class="sxs-lookup"><span data-stu-id="ddc8a-124">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="ddc8a-125">Fornece a capacidade de Pesquisar pessoas e renderizar a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-125">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="ddc8a-126">Cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="ddc8a-126">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="ddc8a-127">Um submenu usado no componente Person para exibir mais informações de perfil sobre um usuário.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-127">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="ddc8a-128">Get</span><span class="sxs-lookup"><span data-stu-id="ddc8a-128">Get</span></span>](./components/get.md)|<span data-ttu-id="ddc8a-129">Faça uma consulta GET para qualquer API do Microsoft Graph diretamente no HTML.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-129">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|

### <a name="providers"></a><span data-ttu-id="ddc8a-130">Provedores</span><span class="sxs-lookup"><span data-stu-id="ddc8a-130">Providers</span></span>

<span data-ttu-id="ddc8a-131">Os componentes funcionam melhor quando usados com um [provedor](/providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="ddc8a-131">The components work best when used with a [provider](/providers/providers.md).</span></span> <span data-ttu-id="ddc8a-132">Os provedores habilitam a autenticação e fornecem a implementação para adquirir os tokens de acesso para chamar as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-132">Providers enable authentication and provide the implementation for acquiring the access tokens for calling the Microsoft Graph APIs.</span></span>

|<span data-ttu-id="ddc8a-133">Provedores</span><span class="sxs-lookup"><span data-stu-id="ddc8a-133">Providers</span></span>|<span data-ttu-id="ddc8a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddc8a-134">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="ddc8a-135">MSAL</span><span class="sxs-lookup"><span data-stu-id="ddc8a-135">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="ddc8a-136">Usa MSAL. js para entrar em usuários e adquirir tokens para uso com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-136">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="ddc8a-137">SharePoint</span><span class="sxs-lookup"><span data-stu-id="ddc8a-137">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="ddc8a-138">Autentica e fornece acesso do Microsoft Graph aos componentes dentro de Web Parts do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-138">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="ddc8a-139">Teams</span><span class="sxs-lookup"><span data-stu-id="ddc8a-139">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="ddc8a-140">Autentica e fornece acesso do Microsoft Graph aos componentes dentro das guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-140">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="ddc8a-141">Acionista</span><span class="sxs-lookup"><span data-stu-id="ddc8a-141">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="ddc8a-142">Permite o uso da autenticação de backend ao rotear todas as chamadas para o Microsoft Graph por meio do seu back-end.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-142">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="ddc8a-143">Personalizados</span><span class="sxs-lookup"><span data-stu-id="ddc8a-143">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="ddc8a-144">Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-144">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="ddc8a-145">Por que usar o kit de ferramentas do Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="ddc8a-145">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="ddc8a-146">O kit de ferramentas do Microsoft Graph disponibiliza a integração de experiências comuns que o Microsoft Graph em seu próprio aplicativo rápido e fácil.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-146">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="ddc8a-147">**Tempo de desenvolvimento reduzido**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-147">**Cut Development Time**</span></span>

    <span data-ttu-id="ddc8a-148">O trabalho para se conectar às APIs do Microsoft Graph e renderizar os dados em uma interface do usuário que parece uma experiência de Microsoft365 é feita para você, sem a necessidade de personalização.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-148">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="ddc8a-149">**Funciona em qualquer lugar**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-149">**Works Everywhere**</span></span>

    <span data-ttu-id="ddc8a-150">Todos os componentes são baseados nos padrões da Web e funcionam de forma perfeita com qualquer navegador e Web Framework modernos (reagir, angulares, Vue, etc.).</span><span class="sxs-lookup"><span data-stu-id="ddc8a-150">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="ddc8a-151">**Linda, mas flexível**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-151">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="ddc8a-152">Os componentes foram projetados para serem parecidos com as experiências do Microsoft365, mas também podem ser personalizáveis usando [as propriedades personalizadas](./style.md) e [Templating](./templates.md)de CSS.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-152">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./style.md) and [templating](./templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="ddc8a-153">Quem deve usá-lo?</span><span class="sxs-lookup"><span data-stu-id="ddc8a-153">Who should use it?</span></span>

<span data-ttu-id="ddc8a-154">O Microsoft Graph Toolkit é excelente para desenvolvedores de todos os níveis de experiência que procuram desenvolver um aplicativo Web, guia do Microsoft Teams ou Web Part do SharePoint que se conecta e acessa os dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-154">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop a web application, Microsoft Teams tab, or SharePoint web part that connects to and accesses data from Microsoft Graph.</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="ddc8a-155">Onde posso usá-lo?</span><span class="sxs-lookup"><span data-stu-id="ddc8a-155">Where can I use it?</span></span>

<span data-ttu-id="ddc8a-156">O kit de ferramentas do Microsoft Graph é suportado nos seguintes navegadores.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-156">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Borda](images/edgeIcon.png)|![Internet Explorer 11](images/internetExplorerIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="ddc8a-164">**Borda**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-164">**Edge**</span></span>|<span data-ttu-id="ddc8a-165">**IE 11**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-165">**IE 11**</span></span>|<span data-ttu-id="ddc8a-166">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-166">**Firefox**</span></span>|<span data-ttu-id="ddc8a-167">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-167">**Chrome**</span></span>|<span data-ttu-id="ddc8a-168">**Safari**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-168">**Safari**</span></span>|<span data-ttu-id="ddc8a-169">**Opera**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-169">**Opera**</span></span>|<span data-ttu-id="ddc8a-170">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="ddc8a-170">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="ddc8a-171">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="ddc8a-171">Next steps</span></span>

- <span data-ttu-id="ddc8a-172">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="ddc8a-172">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="ddc8a-173">[Introdução](get-started.md) ao Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="ddc8a-173">[Get started](get-started.md) with the Microsoft Graph Toolkit.</span></span>
