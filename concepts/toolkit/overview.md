---
title: 'Kit de ferramentas do Microsoft Graph: componentes de interface do usuário e provedores de autenticação para o Microsoft Graph'
description: O kit de ferramentas do Microsoft Graph é uma coleção de provedores de autenticação e componentes Web reutilizáveis de estrutura independente para acessar e trabalhar com o Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: d2ed14c5862cbd081b7592a180cd15e2bfdb2548
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659260"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a><span data-ttu-id="2741d-103">Kit de ferramentas do Microsoft Graph: componentes de interface do usuário e provedores de autenticação para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2741d-103">Microsoft Graph Toolkit: UI Components and Authentication Providers for Microsoft Graph</span></span> 

<span data-ttu-id="2741d-104">O kit de ferramentas do Microsoft Graph é uma coleção de componentes e provedores de autenticação reutilizáveis e independentes de estrutura para acessar e trabalhar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2741d-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic components and authentication providers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="2741d-105">Os componentes são totalmente funcionais à direita da caixa, com provedores internos que autenticam e buscam dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2741d-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="2741d-106">O Microsoft Graph Toolkit torna fácil usar o Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2741d-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="2741d-107">No exemplo a seguir, um usuário conectado e seus eventos de calendário são exibidos com apenas duas linhas de código usando os componentes de [login](./components/login.md) e [agenda](./components/agenda.md) .</span><span class="sxs-lookup"><span data-stu-id="2741d-107">In the following example, a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="2741d-108">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="2741d-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="2741d-109">O que há no Microsoft Graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="2741d-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="2741d-110">Componentes</span><span class="sxs-lookup"><span data-stu-id="2741d-110">Components</span></span>

<span data-ttu-id="2741d-111">O kit de ferramentas do Microsoft Graph inclui uma coleção de componentes Web para as experiências mais compiladas com as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2741d-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span> 

<span data-ttu-id="2741d-112">Os componentes também estão disponíveis como [componentes de reagir](./get-started/mgt-react.md).</span><span class="sxs-lookup"><span data-stu-id="2741d-112">The components are also available as [React components](./get-started/mgt-react.md).</span></span>

|<span data-ttu-id="2741d-113">Componente</span><span class="sxs-lookup"><span data-stu-id="2741d-113">Component</span></span>|<span data-ttu-id="2741d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="2741d-114">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="2741d-115">Logon</span><span class="sxs-lookup"><span data-stu-id="2741d-115">Login</span></span>](./components/login.md)|<span data-ttu-id="2741d-116">Um botão e um controle de submenu para autenticar um usuário com a plataforma de identidade da Microsoft e exibir as informações de perfil do usuário em entrar.</span><span class="sxs-lookup"><span data-stu-id="2741d-116">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="2741d-117">Pessoa</span><span class="sxs-lookup"><span data-stu-id="2741d-117">Person</span></span>](./components/person.md)|<span data-ttu-id="2741d-118">Exibe uma pessoa ou contato por sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="2741d-118">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="2741d-119">Pessoas</span><span class="sxs-lookup"><span data-stu-id="2741d-119">People</span></span>](./components/people.md)|<span data-ttu-id="2741d-120">Exibe um grupo de pessoas ou contatos por suas fotos ou iniciais.</span><span class="sxs-lookup"><span data-stu-id="2741d-120">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="2741d-121">Agenda</span><span class="sxs-lookup"><span data-stu-id="2741d-121">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="2741d-122">Exibe eventos no calendário de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="2741d-122">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="2741d-123">Tarefas</span><span class="sxs-lookup"><span data-stu-id="2741d-123">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="2741d-124">Exibe e habilita adição, remoção, conclusão ou edição de tarefas do Microsoft Planner ou do Microsoft para o.</span><span class="sxs-lookup"><span data-stu-id="2741d-124">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To Do.</span></span>|
|[<span data-ttu-id="2741d-125">Seletor de pessoas</span><span class="sxs-lookup"><span data-stu-id="2741d-125">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="2741d-126">Fornece a capacidade de Pesquisar pessoas e renderizar a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="2741d-126">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="2741d-127">Cartão de pessoa</span><span class="sxs-lookup"><span data-stu-id="2741d-127">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="2741d-128">Um submenu usado no componente Person para exibir mais informações de perfil sobre um usuário.</span><span class="sxs-lookup"><span data-stu-id="2741d-128">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="2741d-129">Get</span><span class="sxs-lookup"><span data-stu-id="2741d-129">Get</span></span>](./components/get.md)|<span data-ttu-id="2741d-130">Faça uma consulta GET para qualquer API do Microsoft Graph diretamente no HTML.</span><span class="sxs-lookup"><span data-stu-id="2741d-130">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="2741d-131">Seletor de canal</span><span class="sxs-lookup"><span data-stu-id="2741d-131">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="2741d-132">Fornece a capacidade de Pesquisar os canais do Microsoft Teams para selecionar um canal de uma lista de resultados renderizada.</span><span class="sxs-lookup"><span data-stu-id="2741d-132">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|
|[<span data-ttu-id="2741d-133">Tarefas Pendentes</span><span class="sxs-lookup"><span data-stu-id="2741d-133">To Do</span></span>](./components/todo.md)|<span data-ttu-id="2741d-134">Exibe e permite adicionar, remover, concluir ou editar tarefas da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2741d-134">Displays and enables adding, removing, completing, or editing of tasks from Microsoft To Do.</span></span>|

### <a name="providers"></a><span data-ttu-id="2741d-135">Provedores</span><span class="sxs-lookup"><span data-stu-id="2741d-135">Providers</span></span>

<span data-ttu-id="2741d-136">Os [provedores](/providers/providers.md) habilitam a autenticação e fornecem a implementação para adquirir tokens de acesso em várias plataformas e expor um cliente do Microsoft Graph para chamar as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2741d-136">[Providers](/providers/providers.md) enable authentication and provide the implementation for acquiring access tokens on various platforms and expose a Microsoft Graph client for calling the Microsoft Graph APIs.</span></span> <span data-ttu-id="2741d-137">Os componentes funcionam melhor quando usados com um provedor, mas os provedores podem ser usados sozinhos.</span><span class="sxs-lookup"><span data-stu-id="2741d-137">The components work best when used with a provider, but the providers can be used on their own.</span></span>

|<span data-ttu-id="2741d-138">Provedores</span><span class="sxs-lookup"><span data-stu-id="2741d-138">Providers</span></span>|<span data-ttu-id="2741d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="2741d-139">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="2741d-140">MSAL</span><span class="sxs-lookup"><span data-stu-id="2741d-140">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="2741d-141">Usa MSAL.js para entrar em usuários e adquirir tokens para uso com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2741d-141">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="2741d-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="2741d-142">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="2741d-143">Autentica e fornece acesso do Microsoft Graph aos componentes dentro de Web Parts do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2741d-143">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="2741d-144">Teams</span><span class="sxs-lookup"><span data-stu-id="2741d-144">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="2741d-145">Autentica e fornece acesso do Microsoft Graph aos componentes dentro das guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2741d-145">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="2741d-146">Acionista</span><span class="sxs-lookup"><span data-stu-id="2741d-146">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="2741d-147">Permite o uso da autenticação de backend ao rotear todas as chamadas para o Microsoft Graph por meio do seu back-end.</span><span class="sxs-lookup"><span data-stu-id="2741d-147">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="2741d-148">Personalizados</span><span class="sxs-lookup"><span data-stu-id="2741d-148">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="2741d-149">Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2741d-149">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="2741d-150">Por que usar o kit de ferramentas do Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="2741d-150">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="2741d-151">O kit de ferramentas do Microsoft Graph disponibiliza a integração de experiências comuns que o Microsoft Graph em seu próprio aplicativo rápido e fácil.</span><span class="sxs-lookup"><span data-stu-id="2741d-151">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="2741d-152">**Tempo de desenvolvimento reduzido**</span><span class="sxs-lookup"><span data-stu-id="2741d-152">**Cut Development Time**</span></span>

    <span data-ttu-id="2741d-153">O trabalho para se conectar às APIs do Microsoft Graph e renderizar os dados em uma interface do usuário que parece uma experiência de Microsoft365 é feita para você, sem a necessidade de personalização.</span><span class="sxs-lookup"><span data-stu-id="2741d-153">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="2741d-154">**Funciona em qualquer lugar**</span><span class="sxs-lookup"><span data-stu-id="2741d-154">**Works Everywhere**</span></span>

    <span data-ttu-id="2741d-155">Todos os componentes são baseados nos padrões da Web e funcionam de forma perfeita com qualquer navegador e Web Framework modernos (reagir, angulares, Vue, etc.).</span><span class="sxs-lookup"><span data-stu-id="2741d-155">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="2741d-156">**Linda, mas flexível**</span><span class="sxs-lookup"><span data-stu-id="2741d-156">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="2741d-157">Os componentes foram projetados para serem parecidos com as experiências do Microsoft365, mas também podem ser personalizáveis usando [as propriedades personalizadas](./customize-components/style.md) e [Templating](./customize-components/templates.md)de CSS.</span><span class="sxs-lookup"><span data-stu-id="2741d-157">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./customize-components/style.md) and [templating](./customize-components/templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="2741d-158">Quem deve usá-lo?</span><span class="sxs-lookup"><span data-stu-id="2741d-158">Who should use it?</span></span>

<span data-ttu-id="2741d-159">O Microsoft Graph Toolkit é excelente para desenvolvedores de todos os níveis de experiência que procuram desenvolver um aplicativo Web, guia do Microsoft Teams ou Web Part do SharePoint que se conecta e acessa os dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2741d-159">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop a web application, Microsoft Teams tab, or SharePoint web part that connects to and accesses data from Microsoft Graph.</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="2741d-160">Onde posso usá-lo?</span><span class="sxs-lookup"><span data-stu-id="2741d-160">Where can I use it?</span></span>

<span data-ttu-id="2741d-161">O kit de ferramentas do Microsoft Graph é suportado nos seguintes navegadores.</span><span class="sxs-lookup"><span data-stu-id="2741d-161">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Borda](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="2741d-168">**Borda**</span><span class="sxs-lookup"><span data-stu-id="2741d-168">**Edge**</span></span>|<span data-ttu-id="2741d-169">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="2741d-169">**Firefox**</span></span>|<span data-ttu-id="2741d-170">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="2741d-170">**Chrome**</span></span>|<span data-ttu-id="2741d-171">**Safari**</span><span class="sxs-lookup"><span data-stu-id="2741d-171">**Safari**</span></span>|<span data-ttu-id="2741d-172">**Opera**</span><span class="sxs-lookup"><span data-stu-id="2741d-172">**Opera**</span></span>|<span data-ttu-id="2741d-173">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="2741d-173">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="2741d-174">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2741d-174">Next steps</span></span>

- <span data-ttu-id="2741d-175">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="2741d-175">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="2741d-176">[Introdução](./get-started/overview.md) ao Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="2741d-176">[Get started](./get-started/overview.md) with the Microsoft Graph Toolkit.</span></span>
- <span data-ttu-id="2741d-177">Confira o Microsoft Graph Toolkit no [GitHub](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="2741d-177">Check out the Microsoft Graph Toolkit on [GitHub](https://aka.ms/mgt).</span></span>
