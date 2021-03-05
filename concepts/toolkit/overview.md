---
title: 'Microsoft Graph Toolkit: Componentes da interface do usuário e provedores de autenticação para o Microsoft Graph'
description: O microsoft graph Toolkit é uma coleção de provedores de autenticação e componentes web reutilizáveis e agnósticos da estrutura para acessar e trabalhar com o Microsoft Graph.
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 01f406c288ebca1dde5c6b1577fd2acdc7631d5b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470533"
---
# <a name="microsoft-graph-toolkit-ui-components-and-authentication-providers-for-microsoft-graph"></a><span data-ttu-id="a68b4-103">Microsoft Graph Toolkit: Componentes da interface do usuário e provedores de autenticação para o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a68b4-103">Microsoft Graph Toolkit: UI Components and Authentication Providers for Microsoft Graph</span></span> 

<span data-ttu-id="a68b4-104">O microsoft graph Toolkit é uma coleção de componentes reutilizáveis, componentes de estrutura e provedores de autenticação para acessar e trabalhar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a68b4-104">The Microsoft Graph Toolkit is a collection of reusable, framework-agnostic components and authentication providers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="a68b4-105">Os componentes são totalmente funcionais imediatamente, com provedores internos que se autenticam com e buscam dados do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a68b4-105">The components are fully functional right of out of the box, with built in providers that authenticate with and fetch data from Microsoft Graph.</span></span>

<span data-ttu-id="a68b4-106">A Toolkit do Microsoft Graph facilita o uso do Microsoft Graph em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a68b4-106">The Microsoft Graph Toolkit makes it easy to use Microsoft Graph in your application.</span></span> <span data-ttu-id="a68b4-107">No exemplo a seguir, um usuário e seus eventos de calendário são exibidos com apenas duas linhas de código usando os componentes [Login](./components/login.md) e [Agenda.](./components/agenda.md)</span><span class="sxs-lookup"><span data-stu-id="a68b4-107">In the following example, a signed in user and their calendar events are displayed with just two lines of code by using the [Login](./components/login.md) and [Agenda](./components/agenda.md) components.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=samples-general--login-to-show-agenda&source=docs&source=docs" height="400"></iframe>

[<span data-ttu-id="a68b4-108">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="a68b4-108">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/samples-general--login-to-show-agenda&source=docs)

## <a name="whats-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="a68b4-109">O que há no microsoft graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="a68b4-109">What's in the Microsoft Graph Toolkit?</span></span>

### <a name="components"></a><span data-ttu-id="a68b4-110">Componentes</span><span class="sxs-lookup"><span data-stu-id="a68b4-110">Components</span></span>

<span data-ttu-id="a68b4-111">O microsoft graph Toolkit inclui uma coleção de componentes da Web para as experiências mais comumente criadas com as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a68b4-111">The Microsoft Graph Toolkit includes a collection of web components for the most commonly built experiences powered by Microsoft Graph APIs.</span></span> 

<span data-ttu-id="a68b4-112">Os componentes também estão disponíveis como [componentes do React.](./get-started/mgt-react.md)</span><span class="sxs-lookup"><span data-stu-id="a68b4-112">The components are also available as [React components](./get-started/mgt-react.md).</span></span>

|<span data-ttu-id="a68b4-113">Componente</span><span class="sxs-lookup"><span data-stu-id="a68b4-113">Component</span></span>|<span data-ttu-id="a68b4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a68b4-114">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="a68b4-115">Logon</span><span class="sxs-lookup"><span data-stu-id="a68b4-115">Login</span></span>](./components/login.md)|<span data-ttu-id="a68b4-116">Um botão e um controle de sobrevoo para autenticar um usuário com a plataforma Microsoft Identity e exibir as informações de perfil do usuário ao entrar.</span><span class="sxs-lookup"><span data-stu-id="a68b4-116">A button and a flyout control to authenticate a user with the Microsoft Identity platform and display the user's profile information on sign in.</span></span>|
|[<span data-ttu-id="a68b4-117">Pessoa</span><span class="sxs-lookup"><span data-stu-id="a68b4-117">Person</span></span>](./components/person.md)|<span data-ttu-id="a68b4-118">Exibe uma pessoa ou contato por sua foto, nome e/ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="a68b4-118">Displays a person or contact by their photo, name, and/or email address.</span></span>|
|[<span data-ttu-id="a68b4-119">Pessoas</span><span class="sxs-lookup"><span data-stu-id="a68b4-119">People</span></span>](./components/people.md)|<span data-ttu-id="a68b4-120">Exibe um grupo de pessoas ou contatos por suas fotos ou iniciais.</span><span class="sxs-lookup"><span data-stu-id="a68b4-120">Displays a group of people or contacts by their photos or initials.</span></span>|
|[<span data-ttu-id="a68b4-121">Agenda</span><span class="sxs-lookup"><span data-stu-id="a68b4-121">Agenda</span></span>](./components/agenda.md)|<span data-ttu-id="a68b4-122">Exibe eventos no calendário de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="a68b4-122">Displays events in a user or group's calendar.</span></span>|
|[<span data-ttu-id="a68b4-123">Tarefas</span><span class="sxs-lookup"><span data-stu-id="a68b4-123">Tasks</span></span>](./components/tasks.md)|<span data-ttu-id="a68b4-124">Exibe e habilita a adição, remoção, conclusão ou edição de tarefas do Microsoft Planner ou Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="a68b4-124">Displays and enables adding, removing, completing, or editing of tasks from Microsoft Planner or Microsoft To Do.</span></span>|
|[<span data-ttu-id="a68b4-125">Seletor de pessoas</span><span class="sxs-lookup"><span data-stu-id="a68b4-125">People picker</span></span>](./components/people-picker.md)|<span data-ttu-id="a68b4-126">Fornece a capacidade de pesquisar por pessoas e renderiza a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="a68b4-126">Provides the ability to search for people and renders the list of results.</span></span>|
|[<span data-ttu-id="a68b4-127">Cartão pessoal</span><span class="sxs-lookup"><span data-stu-id="a68b4-127">Person card</span></span>](./components/person-card.md)|<span data-ttu-id="a68b4-128">Um flyout usado no componente da pessoa para exibir mais informações de perfil sobre um usuário.</span><span class="sxs-lookup"><span data-stu-id="a68b4-128">A flyout used on the person component to display more profile information about a user.</span></span>|
|[<span data-ttu-id="a68b4-129">Get</span><span class="sxs-lookup"><span data-stu-id="a68b4-129">Get</span></span>](./components/get.md)|<span data-ttu-id="a68b4-130">Faça uma consulta GET para qualquer API do Microsoft Graph diretamente em seu HTML.</span><span class="sxs-lookup"><span data-stu-id="a68b4-130">Make a GET query to any Microsoft Graph API directly in your HTML.</span></span>|
|[<span data-ttu-id="a68b4-131">Se picker de canal</span><span class="sxs-lookup"><span data-stu-id="a68b4-131">Channel picker</span></span>](./components/teams-channel-picker.md)|<span data-ttu-id="a68b4-132">Fornece a capacidade de pesquisar canais do Microsoft Teams para selecionar um canal em uma lista renderizada de resultados.</span><span class="sxs-lookup"><span data-stu-id="a68b4-132">Provides the ability to search for Microsoft Teams channels to select a channel from a rendered list of results.</span></span>|
|[<span data-ttu-id="a68b4-133">To Do</span><span class="sxs-lookup"><span data-stu-id="a68b4-133">To Do</span></span>](./components/todo.md)|<span data-ttu-id="a68b4-134">Exibe e habilita a adição, remoção, conclusão ou edição de tarefas do Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="a68b4-134">Displays and enables adding, removing, completing, or editing of tasks from Microsoft To Do.</span></span>|

### <a name="providers"></a><span data-ttu-id="a68b4-135">Provedores</span><span class="sxs-lookup"><span data-stu-id="a68b4-135">Providers</span></span>

<span data-ttu-id="a68b4-136">[Os provedores](/providers/providers.md) habilitam a autenticação e fornecem a implementação para adquirir tokens de acesso em várias plataformas e expõem um cliente do Microsoft Graph para chamar as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a68b4-136">[Providers](/providers/providers.md) enable authentication and provide the implementation for acquiring access tokens on various platforms and expose a Microsoft Graph client for calling the Microsoft Graph APIs.</span></span> <span data-ttu-id="a68b4-137">Os componentes funcionam melhor quando usados com um provedor, mas os provedores podem ser usados por conta própria.</span><span class="sxs-lookup"><span data-stu-id="a68b4-137">The components work best when used with a provider, but the providers can be used on their own.</span></span>

|<span data-ttu-id="a68b4-138">Provedores</span><span class="sxs-lookup"><span data-stu-id="a68b4-138">Providers</span></span>|<span data-ttu-id="a68b4-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="a68b4-139">Description</span></span>|
|---------|-----------|
|[<span data-ttu-id="a68b4-140">Msal</span><span class="sxs-lookup"><span data-stu-id="a68b4-140">Msal</span></span>](./providers/msal.md)|<span data-ttu-id="a68b4-141">Usa MSAL.js para entrar em usuários e adquirir tokens para usar com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a68b4-141">Uses MSAL.js to sign in users and acquire tokens to use with Microsoft Graph.</span></span>|
|[<span data-ttu-id="a68b4-142">Tron</span><span class="sxs-lookup"><span data-stu-id="a68b4-142">Electron</span></span>](./providers/electron.md)|<span data-ttu-id="a68b4-143">Autentica e fornece acesso do Microsoft Graph a componentes dentro de aplicativos Detron</span><span class="sxs-lookup"><span data-stu-id="a68b4-143">Authenticates and provides Microsoft Graph access to components inside of Electron apps</span></span>|
|[<span data-ttu-id="a68b4-144">SharePoint</span><span class="sxs-lookup"><span data-stu-id="a68b4-144">SharePoint</span></span>](./providers/sharepoint.md)|<span data-ttu-id="a68b4-145">Autentica e fornece acesso do Microsoft Graph a componentes dentro das Web Parts do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a68b4-145">Authenticates and provides Microsoft Graph access to components inside of SharePoint web parts.</span></span>|
|[<span data-ttu-id="a68b4-146">Teams</span><span class="sxs-lookup"><span data-stu-id="a68b4-146">Teams</span></span>](./providers/teams.md)|<span data-ttu-id="a68b4-147">Autentica e fornece acesso do Microsoft Graph a componentes dentro das guias do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a68b4-147">Authenticates and provides Microsoft Graph access to components inside of Microsoft Teams tabs.</span></span>|
|[<span data-ttu-id="a68b4-148">Proxy</span><span class="sxs-lookup"><span data-stu-id="a68b4-148">Proxy</span></span>](./providers/proxy.md)|<span data-ttu-id="a68b4-149">Permite o uso da autenticação de back-end roteamento de todas as chamadas para o Microsoft Graph por meio do back-end.</span><span class="sxs-lookup"><span data-stu-id="a68b4-149">Allows the use of backend authentication by routing all calls to Microsoft Graph through your backend.</span></span>|
|[<span data-ttu-id="a68b4-150">Personalizados</span><span class="sxs-lookup"><span data-stu-id="a68b4-150">Custom</span></span>](./providers/custom.md)|<span data-ttu-id="a68b4-151">Crie um provedor personalizado para habilitar a autenticação e o acesso ao Microsoft Graph com o código de autenticação existente do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a68b4-151">Create a custom provider to enable authentication and access to Microsoft Graph with your application's existing authentication code.</span></span>|

## <a name="why-use-the-microsoft-graph-toolkit"></a><span data-ttu-id="a68b4-152">Por que usar o microsoft graph Toolkit?</span><span class="sxs-lookup"><span data-stu-id="a68b4-152">Why use the Microsoft Graph Toolkit?</span></span>

<span data-ttu-id="a68b4-153">A Toolkit do Microsoft Graph torna a integração de experiências comuns fornecidas pelo Microsoft Graph em seu próprio aplicativo de forma rápida e fácil.</span><span class="sxs-lookup"><span data-stu-id="a68b4-153">The Microsoft Graph Toolkit makes integrating common experiences powered by Microsoft Graph into your own application quick and easy.</span></span>

:::row:::
   :::column span="":::
    <span data-ttu-id="a68b4-154">**Reduzir o tempo de desenvolvimento**</span><span class="sxs-lookup"><span data-stu-id="a68b4-154">**Cut Development Time**</span></span>

    <span data-ttu-id="a68b4-155">O trabalho para se conectar às APIs do Microsoft Graph e renderizar os dados em uma interface do usuário que parece e parece uma experiência do Microsoft365 é feito para você, sem nenhuma personalização necessária.</span><span class="sxs-lookup"><span data-stu-id="a68b4-155">The work to connect to Microsoft Graph APIs and render the data in a UI that looks and feels like a Microsoft365 experience is done for you, with no customization required.</span></span>
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="a68b4-156">**Funciona em todos os lugares**</span><span class="sxs-lookup"><span data-stu-id="a68b4-156">**Works Everywhere**</span></span>

    <span data-ttu-id="a68b4-157">Todos os componentes são baseados em padrões da Web e funcionam perfeitamente com qualquer navegador moderno e estrutura da Web (React, Angular, Vue etc.).</span><span class="sxs-lookup"><span data-stu-id="a68b4-157">All components are based on web standards and work seamlessly with any modern browser and web framework (React, Angular, Vue, etc.).</span></span> 
  :::column-end:::
  :::column span="":::
    <span data-ttu-id="a68b4-158">**Belo, mas flexível**</span><span class="sxs-lookup"><span data-stu-id="a68b4-158">**Beautiful but Flexible**</span></span>

    <span data-ttu-id="a68b4-159">Os componentes são projetados para parecer experiências do Microsoft365, mas também são personalizáveis usando [propriedades personalizadas CSS](./customize-components/style.md) e [templating](./customize-components/templates.md).</span><span class="sxs-lookup"><span data-stu-id="a68b4-159">The components are designed to look and feel like Microsoft365 experiences, but are also customizable using [CSS custom properties](./customize-components/style.md) and [templating](./customize-components/templates.md).</span></span>
  :::column-end:::
:::row-end:::

## <a name="who-should-use-it"></a><span data-ttu-id="a68b4-160">Quem deve usá-lo?</span><span class="sxs-lookup"><span data-stu-id="a68b4-160">Who should use it?</span></span>

<span data-ttu-id="a68b4-161">O microsoft graph Toolkit é ótimo para desenvolvedores de todos os níveis de experiência que procuram desenvolver um aplicativo que se conecta e acessa dados do Microsoft Graph, como:</span><span class="sxs-lookup"><span data-stu-id="a68b4-161">The Microsoft Graph Toolkit is great for developers of all experience levels looking to develop an app that connects to and accesses data from Microsoft Graph, such as a:</span></span>
- <span data-ttu-id="a68b4-162">Aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="a68b4-162">Web app</span></span>
- <span data-ttu-id="a68b4-163">Guia Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a68b4-163">Microsoft Teams tab</span></span>
- <span data-ttu-id="a68b4-164">Aplicativo Web Progressivo (PWA)</span><span class="sxs-lookup"><span data-stu-id="a68b4-164">Progressive Web App (PWA)</span></span>
- <span data-ttu-id="a68b4-165">Aplicativo Detron</span><span class="sxs-lookup"><span data-stu-id="a68b4-165">Electron app</span></span>
- <span data-ttu-id="a68b4-166">Web Part do SharePoint</span><span class="sxs-lookup"><span data-stu-id="a68b4-166">SharePoint web part</span></span>

## <a name="where-can-i-use-it"></a><span data-ttu-id="a68b4-167">Onde posso usá-lo?</span><span class="sxs-lookup"><span data-stu-id="a68b4-167">Where can I use it?</span></span>

<span data-ttu-id="a68b4-168">O microsoft graph Toolkit é suportado nos seguintes navegadores.</span><span class="sxs-lookup"><span data-stu-id="a68b4-168">The Microsoft Graph Toolkit is supported in the following browsers.</span></span>

|![Borda](images/edgeIcon.png)|![Firefox](images/firefoxIcon.png)|![Chrome](images/chromeIcon.png)|![Safari](images/safariIcon.png)|![Opera](images/operaIcon.png)|![Samsung Internet](images/samsungInternetIcon.png)|
|----|----|----|----|----|----|----|
|<span data-ttu-id="a68b4-175">**Borda**</span><span class="sxs-lookup"><span data-stu-id="a68b4-175">**Edge**</span></span>|<span data-ttu-id="a68b4-176">**Firefox**</span><span class="sxs-lookup"><span data-stu-id="a68b4-176">**Firefox**</span></span>|<span data-ttu-id="a68b4-177">**Chrome**</span><span class="sxs-lookup"><span data-stu-id="a68b4-177">**Chrome**</span></span>|<span data-ttu-id="a68b4-178">**Safari**</span><span class="sxs-lookup"><span data-stu-id="a68b4-178">**Safari**</span></span>|<span data-ttu-id="a68b4-179">**Opera**</span><span class="sxs-lookup"><span data-stu-id="a68b4-179">**Opera**</span></span>|<span data-ttu-id="a68b4-180">**Samsung**</span><span class="sxs-lookup"><span data-stu-id="a68b4-180">**Samsung**</span></span>|

## <a name="next-steps"></a><span data-ttu-id="a68b4-181">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a68b4-181">Next steps</span></span>

- <span data-ttu-id="a68b4-182">Experimente os componentes no [playground](https://mgt.dev).</span><span class="sxs-lookup"><span data-stu-id="a68b4-182">Try out the components in the [playground](https://mgt.dev).</span></span>
- <span data-ttu-id="a68b4-183">[Começar a](./get-started/overview.md) trabalhar com o Microsoft Graph Toolkit.</span><span class="sxs-lookup"><span data-stu-id="a68b4-183">[Get started](./get-started/overview.md) with the Microsoft Graph Toolkit.</span></span>
- <span data-ttu-id="a68b4-184">Confira o microsoft graph Toolkit [github](https://aka.ms/mgt).</span><span class="sxs-lookup"><span data-stu-id="a68b4-184">Check out the Microsoft Graph Toolkit on [GitHub](https://aka.ms/mgt).</span></span>
