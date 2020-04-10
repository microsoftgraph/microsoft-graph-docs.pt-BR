---
title: 'Kit de ferramentas do Microsoft Graph: Web Components da plataforma Microsoft Graph'
description: O kit de ferramentas do Microsoft Graph é uma coleção de resuable, componentes da Web e auxiliares de estrutura independente para acessar e trabalhar com o Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 2ba11a66dcec1eaec276b3fe71427fcf356cbcde
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181613"
---
# <a name="microsoft-graph-toolkit-web-components-powered-by-microsoft-graph"></a><span data-ttu-id="af85f-103">Kit de ferramentas do Microsoft Graph: Web Components da plataforma Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="af85f-103">Microsoft Graph Toolkit: Web Components powered by Microsoft Graph</span></span>

<span data-ttu-id="af85f-104">O kit de ferramentas do Microsoft Graph é uma coleção de componentes da Web e auxiliares reutilizáveis da estrutura, que podem acessar e trabalhar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af85f-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="af85f-105">Os componentes são totalmente funcionais à direita da caixa, com provedores internos que autenticam e buscam dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af85f-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="af85f-106">O Microsoft Graph Toolkit torna fácil usar o Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af85f-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="af85f-107">No exemplo abaixo, Confira como um usuário conectado e seus eventos de calendário são exibidos com apenas duas linhas de código usando os componentes de [login](./components/login.md) e [agenda](./components/agenda.md) .</span><span class="sxs-lookup"><span data-stu-id="af85f-107">In the example below, see how a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="af85f-108">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="af85f-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="af85f-109">O que há no Microsoft Graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="af85f-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="af85f-110">Componentes</span><span class="sxs-lookup"><span data-stu-id="af85f-110">Components</span></span>

<span data-ttu-id="af85f-111">O kit de ferramentas do Microsoft Graph inclui uma coleção de componentes Web para as experiências mais compiladas com as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af85f-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span>

|<span data-ttu-id="af85f-112">Componente</span><span class="sxs-lookup"><span data-stu-id="af85f-112">Component</span></span>|<span data-ttu-id="af85f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="af85f-113">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="af85f-114">Logon</span><span class="sxs-lookup"><span data-stu-id="af85f-114">Login</span></span>](./components/login.md)|<span data-ttu-id="af85f-115">Um botão e um controle de submenu para autenticar um usuário com a plataforma de identidade da Microsoft e exibir as informações de perfil do usuário em entrar.</span><span class="sxs-lookup"><span data-stu-id="af85f-115">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="af85f-116">Pessoa</span><span class="sxs-lookup"><span data-stu-id="af85f-116">Person</span></span>](./components/person.md)|<span data-ttu-id="af85f-117">Exibe uma pessoa ou contato por sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="af85f-117">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="af85f-118">Pessoas</span><span class="sxs-lookup"><span data-stu-id="af85f-118">People</span></span>](./components/people.md)|<span data-ttu-id="af85f-119">Exibe um grupo de pessoas ou contatos por suas fotos ou iniciais.</span><span class="sxs-lookup"><span data-stu-id="af85f-119">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="af85f-120">Agenda</span><span class="sxs-lookup"><span data-stu-id="af85f-120">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="af85f-121">Exibe eventos no calendário de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="af85f-121">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="af85f-122">Tarefas</span><span class="sxs-lookup"><span data-stu-id="af85f-122">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="af85f-123">Exibe e permite adicionar, remover, concluir ou editar tarefas do Microsoft Planner ou do Microsoft to-do.</span><span class="sxs-lookup"><span data-stu-id="af85f-123">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To-Do.</span></span>|
|[<span data-ttu-id="af85f-124">Seletor de pessoas</span><span class="sxs-lookup"><span data-stu-id="af85f-124">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="af85f-125">Fornece a capacidade de Pesquisar pessoas e renderizar a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="af85f-125">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="af85f-126">Cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="af85f-126">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="af85f-127">Um submenu usado no componente Person para exibir mais informações de perfil sobre um usuário.</span><span class="sxs-lookup"><span data-stu-id="af85f-127">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="af85f-128">Get</span><span class="sxs-lookup"><span data-stu-id="af85f-128">Get</span></span>](./components/get.md)|<span data-ttu-id="af85f-129">Faça uma consulta GET para qualquer API do Microsoft Graph diretamente no HTML.</span><span class="sxs-lookup"><span data-stu-id="af85f-129">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="af85f-130">Seletor de canal</span><span class="sxs-lookup"><span data-stu-id="af85f-130">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="af85f-131">Fornece a capacidade de Pesquisar os canais do Microsoft Teams para selecionar um canal de uma lista de resultados renderizada.</span><span class="sxs-lookup"><span data-stu-id="af85f-131">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|

### <a name="providers"></a><span data-ttu-id="af85f-132">Provedores</span><span class="sxs-lookup"><span data-stu-id="af85f-132">Providers</span></span>

<span data-ttu-id="af85f-133">Os componentes funcionam melhor quando usados com um [provedor](/providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="af85f-133">The components work best when used with a [provider](/providers/providers.md).</span></span> <span data-ttu-id="af85f-134">Os provedores habilitam a autenticação e fornecem a implementação para adquirir os tokens de acesso para chamar as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af85f-134">Providers enable authentication and provide the implementation for acquiring the access tokens for calling the Microsoft Graph APIs.</span></span>

|<span data-ttu-id="af85f-135">Provedores</span><span class="sxs-lookup"><span data-stu-id="af85f-135">Providers</span></span>|<span data-ttu-id="af85f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="af85f-136">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="af85f-137">MSAL</span><span class="sxs-lookup"><span data-stu-id="af85f-137">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="af85f-138">Usa MSAL. js para entrar em usuários e adquirir tokens para uso com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af85f-138">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="af85f-139">SharePoint</span><span class="sxs-lookup"><span data-stu-id="af85f-139">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="af85f-140">Autentica e fornece acesso do Microsoft Graph aos componentes dentro de Web Parts do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="af85f-140">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="af85f-141">Teams</span><span class="sxs-lookup"><span data-stu-id="af85f-141">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="af85f-142">Autentica e fornece acesso do Microsoft Graph aos componentes dentro das guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="af85f-142">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="af85f-143">Acionista</span><span class="sxs-lookup"><span data-stu-id="af85f-143">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="af85f-144">Permite o uso da autenticação de backend ao rotear todas as chamadas para o Microsoft Graph por meio do seu back-end.</span><span class="sxs-lookup"><span data-stu-id="af85f-144">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="af85f-145">Personalizados</span><span class="sxs-lookup"><span data-stu-id="af85f-145">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="af85f-146">Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af85f-146">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="af85f-147">Por que usar o kit de ferramentas do Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="af85f-147">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="af85f-148">O kit de ferramentas do Microsoft Graph disponibiliza a integração de experiências comuns que o Microsoft Graph em seu próprio aplicativo rápido e fácil.</span><span class="sxs-lookup"><span data-stu-id="af85f-148">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="af85f-149">**Tempo de desenvolvimento reduzido**</span><span class="sxs-lookup"><span data-stu-id="af85f-149">**Cut Development Time**</span></span>

    <span data-ttu-id="af85f-150">O trabalho para se conectar às APIs do Microsoft Graph e renderizar os dados em uma interface do usuário que parece uma experiência de Microsoft365 é feita para você, sem a necessidade de personalização.</span><span class="sxs-lookup"><span data-stu-id="af85f-150">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="af85f-151">**Funciona em qualquer lugar**</span><span class="sxs-lookup"><span data-stu-id="af85f-151">**Works Everywhere**</span></span>

    <span data-ttu-id="af85f-152">Todos os componentes são baseados nos padrões da Web e funcionam de forma perfeita com qualquer navegador e Web Framework modernos (reagir, angulares, Vue, etc.).</span><span class="sxs-lookup"><span data-stu-id="af85f-152">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="af85f-153">**Linda, mas flexível**</span><span class="sxs-lookup"><span data-stu-id="af85f-153">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="af85f-154">Os componentes foram projetados para serem parecidos com as experiências do Microsoft365, mas também podem ser personalizáveis usando [as propriedades personalizadas](./style.md) e [Templating](./templates.md)de CSS.</span><span class="sxs-lookup"><span data-stu-id="af85f-154">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./style.md) and [templating](./templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="af85f-155">Quem deve usá-lo?</span><span class="sxs-lookup"><span data-stu-id="af85f-155">Who should use it?</span></span>

<span data-ttu-id="af85f-156">O Microsoft Graph Toolkit é excelente para desenvolvedores de todos os níveis de experiência que procuram desenvolver um aplicativo Web, guia do Microsoft Teams ou Web Part do SharePoint que se conecta e acessa os dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="af85f-156">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop a web application, Microsoft Teams tab, or SharePoint web part that connects to and accesses data from Microsoft Graph.</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="af85f-157">Onde posso usá-lo?</span><span class="sxs-lookup"><span data-stu-id="af85f-157">Where can I use it?</span></span>

<span data-ttu-id="af85f-158">O kit de ferramentas do Microsoft Graph é suportado nos seguintes navegadores.</span><span class="sxs-lookup"><span data-stu-id="af85f-158">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Borda](images/edgeIcon.png)|![Internet Explorer 11](images/internetExplorerIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="af85f-166">**Borda**</span><span class="sxs-lookup"><span data-stu-id="af85f-166">**Edge**</span></span>|<span data-ttu-id="af85f-167">**IE 11**</span><span class="sxs-lookup"><span data-stu-id="af85f-167">**IE 11**</span></span>|<span data-ttu-id="af85f-168">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="af85f-168">**Firefox**</span></span>|<span data-ttu-id="af85f-169">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="af85f-169">**Chrome**</span></span>|<span data-ttu-id="af85f-170">**Safari**</span><span class="sxs-lookup"><span data-stu-id="af85f-170">**Safari**</span></span>|<span data-ttu-id="af85f-171">**Opera**</span><span class="sxs-lookup"><span data-stu-id="af85f-171">**Opera**</span></span>|<span data-ttu-id="af85f-172">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="af85f-172">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="af85f-173">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="af85f-173">Next steps</span></span>

- <span data-ttu-id="af85f-174">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="af85f-174">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="af85f-175">[Introdução](get-started.md) ao Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="af85f-175">[Get started](get-started.md) with the Microsoft Graph Toolkit.</span></span>
