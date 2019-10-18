---
title: Visão geral da API do OneNote
description: O OneNote é um bloco de anotações digital que permite que os clientes acompanhem ideias e anotações para uso doméstico, escolar ou profissional digitando, desenhando ou falando na Web, no telefone, no tablet ou no computador. Eles podem organizar anotações, alternar entre dispositivos e retomar de onde pararam, além de colaborar em anotações com outras pessoas em tempo real.
author: Jewan-microsoft
localization_priority: Priority
ms.prod: onenote
scenarios: getting-started
ms.openlocfilehash: 69aa0d83d9625559c7731391f6ad504bd86403f0
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792608"
---
# <a name="onenote-api-overview"></a><span data-ttu-id="e0672-104">Visão geral da API do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-104">OneNote API overview</span></span>

<span data-ttu-id="e0672-105">O OneNote é um bloco de anotações digital que permite que os clientes acompanhem ideias e anotações para uso doméstico, escolar ou profissional digitando, desenhando ou falando na Web, no telefone, no tablet ou no computador.</span><span class="sxs-lookup"><span data-stu-id="e0672-105">OneNote is a digital notebook that lets customers track ideas and notes for home, school, or work, by typing, sketching, or voice, on the web, phone, tablet, or desktop.</span></span> <span data-ttu-id="e0672-106">Eles podem organizar anotações, alternar entre dispositivos e retomar de onde pararam, além de colaborar em anotações com outras pessoas em tempo real.</span><span class="sxs-lookup"><span data-stu-id="e0672-106">They can freely organize notes, switch devices and pick up where they left off, and collaborate on notes with others in real time.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/VXd4OeQU1ek]

## <a name="why-integrate-with-onenote"></a><span data-ttu-id="e0672-107">Por que integrar com o OneNote?</span><span class="sxs-lookup"><span data-stu-id="e0672-107">Why integrate with OneNote?</span></span>

<span data-ttu-id="e0672-108">Integrando os aplicativos ao OneNote, você pode criar experiências para capacitação em várias plataformas que alcançam milhões de usuários em todo o mundo.</span><span class="sxs-lookup"><span data-stu-id="e0672-108">By integrating your apps with OneNote, you can create empowering experiences across multiple platforms that reach millions of users worldwide.</span></span> <span data-ttu-id="e0672-109">Você pode usar o Microsoft Graph para acessar blocos de anotações, seções e páginas no OneNote para criar soluções que ajudam os usuários a planejar e organizar informações e ideias.</span><span class="sxs-lookup"><span data-stu-id="e0672-109">You can use Microsoft Graph to access notebooks, sections, and pages in OneNote to create solutions that help your users plan and organize ideas and information.</span></span>

### <a name="collect-and-organize-notes-and-ideas"></a><span data-ttu-id="e0672-110">Coletar e organizar anotações e ideias</span><span class="sxs-lookup"><span data-stu-id="e0672-110">Collect and organize notes and ideas</span></span>  

<span data-ttu-id="e0672-111">Use o OneNote com uma tela em que os usuários podem adicionar e organizar conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e0672-111">Use OneNote as a canvas where users can add and arrange their content.</span></span> <span data-ttu-id="e0672-112">O Microsoft Graph facilita a criação de aplicativos que ajudam os alunos a fazer anotações e pesquisas, as famílias a compartilhar planos e ideias ou os compradores a compartilhar imagens.</span><span class="sxs-lookup"><span data-stu-id="e0672-112">Microsoft Graph makes it easy to write apps that enable students to take notes and do research, families to share plans and ideas, or shoppers to share pictures.</span></span> <span data-ttu-id="e0672-113">O aplicativo pode obter as informações que as pessoas desejam, enviá-las ao OneNote e ajudar a organizá-las.</span><span class="sxs-lookup"><span data-stu-id="e0672-113">Your app can grab the information people want, send it to OneNote, and then help them organize it.</span></span>

### <a name="capture-information-in-many-formats"></a><span data-ttu-id="e0672-114">Capturar informações em muitos formatos</span><span class="sxs-lookup"><span data-stu-id="e0672-114">Capture information in many formats</span></span>

<span data-ttu-id="e0672-115">Capture HTML, insira imagens (originadas localmente ou em uma URL pública), vídeo, áudio, mensagens de email e outros tipos de arquivos comuns.</span><span class="sxs-lookup"><span data-stu-id="e0672-115">Capture HTML, embed images (sourced locally or at a public URL), video, audio, email messages, and other common file types.</span></span> <span data-ttu-id="e0672-116">O OneNote pode até mesmo renderizar páginas da Web e arquivos PDF como instantâneos.</span><span class="sxs-lookup"><span data-stu-id="e0672-116">OneNote can even render webpages and PDF files as snapshots.</span></span> <span data-ttu-id="e0672-117">O Microsoft Graph dá suporte a um conjunto de HTML e CSS padrão para layout de página do OneNote. Portanto, você pode usar tabelas, imagens embutidas e formatação básica para obter a aparência desejada.</span><span class="sxs-lookup"><span data-stu-id="e0672-117">Microsoft Graph supports a set of standard HTML and CSS for OneNote page layout, so you can use tables, inline images, and basic formatting to get the look you want.</span></span> 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a><span data-ttu-id="e0672-118">Usar o ecossistema do OneNote para aprimorar seus cenários principais</span><span class="sxs-lookup"><span data-stu-id="e0672-118">Use the OneNote ecosystem to enhance your core scenarios</span></span>

<span data-ttu-id="e0672-119">Aproveite outros recursos poderosos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0672-119">Tap into other powerful OneNote features.</span></span> <span data-ttu-id="e0672-120">As APIs do OneNote no Microsoft Graph executam OCR em imagens, dão suporte à pesquisa de texto completo, sincronizam clientes automaticamente, processam imagens e extraem capturas de cartões de visita e listagens de receitas e produtos online.</span><span class="sxs-lookup"><span data-stu-id="e0672-120">The OneNote APIs in Microsoft Graph run OCR on images, support full-text search, auto-syncs clients, process images, and extract business card captures and online product and recipe listings.</span></span> <span data-ttu-id="e0672-121">Use o OneNote como seu repositório de memória digital na nuvem para anotações e mídia leve ou como um feed de dados para dados específicos de domínio.</span><span class="sxs-lookup"><span data-stu-id="e0672-121">Use OneNote as your digital memory store in the cloud for notes and lightweight media, or as a data feed for domain-specific data.</span></span> 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a><span data-ttu-id="e0672-122">Alcance milhares de usuários do OneNote em todas as principais plataformas</span><span class="sxs-lookup"><span data-stu-id="e0672-122">Reach millions of OneNote users on all major platforms</span></span>

<span data-ttu-id="e0672-123">Use o OneNote para aumentar o uso do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e0672-123">Use OneNote to increase your app usage.</span></span> <span data-ttu-id="e0672-124">O OneNote vem pré-instalado nos novos dispositivos Windows e está disponível para a maioria das plataformas, online e como parte do Office 365.
</span><span class="sxs-lookup"><span data-stu-id="e0672-124">OneNote is preinstalled on new Windows devices, and is available for most platforms, online, and as part of Office 365.</span></span> <span data-ttu-id="e0672-125">Ao publicar aplicativos que usam o ambiente do OneNote repleto de recursos, você tem acesso a um amplo potencial de mercado em várias plataformas.</span><span class="sxs-lookup"><span data-stu-id="e0672-125">When you publish apps that use the feature-rich OneNote environment, you have access to broad cross-platform market potential.</span></span>

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: featured_scenarios..md You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="e0672-126">O que posso fazer com as APIs do OneNote no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="e0672-126">What can I do with OneNote APIs in Microsoft Graph?</span></span>

<span data-ttu-id="e0672-127">A seguir, estão algumas das solicitações mais populares para trabalhar com os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0672-127">The following are some of the most popular requests for working with OneNote resources.</span></span>

|<span data-ttu-id="e0672-128">Operação</span><span class="sxs-lookup"><span data-stu-id="e0672-128">Operation</span></span>|<span data-ttu-id="e0672-129">URL</span><span class="sxs-lookup"><span data-stu-id="e0672-129">URL</span></span>|
|:--------|:--|
|<span data-ttu-id="e0672-130">Obter meus blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="e0672-130">GET my notebooks</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|<span data-ttu-id="e0672-131">Obter minhas seções</span><span class="sxs-lookup"><span data-stu-id="e0672-131">GET my sections</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|<span data-ttu-id="e0672-132">Obter minhas páginas</span><span class="sxs-lookup"><span data-stu-id="e0672-132">GET my pages</span></span>|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="learn-more-about-onenote-apis"></a><span data-ttu-id="e0672-133">Saiba mais sobre as APIs do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-133">Learn more about OneNote APIs</span></span>

<span data-ttu-id="e0672-134">Faça uma análise aprofundada das APIs do Microsoft Graph para saber mais sobre as funcionalidades de atualização de conteúdo do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0672-134">Take an in-depth look at Microsoft Graph APIs to learn about the OneNote content updating capabilities.</span></span> <span data-ttu-id="e0672-135">Os tópicos na lista a seguir mostram como criar novas páginas do OneNote e atualizar páginas existentes com novo conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e0672-135">The topics in the following list show you how to create new OneNote pages and update existing pages with new content.</span></span> <span data-ttu-id="e0672-136">Você também aprenderá sobre as práticas recomendadas usando o Microsoft Graph para atualizar os blocos de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0672-136">You'll also learn about best practices in using Microsoft Graph to update OneNote notebooks.</span></span> 


### <a name="work-with-onenote"></a><span data-ttu-id="e0672-137">Trabalhar com o OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-137">Work with OneNote</span></span>

* [<span data-ttu-id="e0672-138">Usar a API REST do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-138">Use the OneNote REST API</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
* [<span data-ttu-id="e0672-139">Práticas recomendadas</span><span class="sxs-lookup"><span data-stu-id="e0672-139">Best practices</span></span>](onenote-best-practices.md)
* [<span data-ttu-id="e0672-140">Diretrizes de identidade visual</span><span class="sxs-lookup"><span data-stu-id="e0672-140">Branding guidelines</span></span>](onenote-branding.md)
* [<span data-ttu-id="e0672-141">Abrir o cliente do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-141">Open the OneNote client</span></span>](open-onenote-client.md)
* [<span data-ttu-id="e0672-142">Usar marcas de anotação nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-142">Use note tags in OneNote pages</span></span>](onenote-note-tags.md)
* [<span data-ttu-id="e0672-143">Códigos de erro para APIs do OneNote no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e0672-143">Error codes for OneNote APIs in Microsoft Graph</span></span>](onenote-error-codes.md)

### <a name="work-with-onenote-pages"></a><span data-ttu-id="e0672-144">Trabalhar com páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-144">Work with OneNote pages</span></span>

* [<span data-ttu-id="e0672-145">HTML de entrada e saída nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-145">Input and output HTML in OneNote pages</span></span>](onenote-input-output-html.md)
* [<span data-ttu-id="e0672-146">Obter a estrutura e o conteúdo do OneNote com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e0672-146">Get OneNote content and structure with Microsoft Graph</span></span>](onenote-get-content.md)
* [<span data-ttu-id="e0672-147">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-147">Create OneNote pages</span></span>](onenote-create-page.md)
* [<span data-ttu-id="e0672-148">Atualizar o conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-148">Update OneNote page content</span></span>](onenote-update-page.md)

### <a name="work-with-onenote-page-content"></a><span data-ttu-id="e0672-149">Trabalhar com conteúdo da página do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-149">Work with OneNote page content</span></span>

* [<span data-ttu-id="e0672-150">Criar elementos posicionados absolutos nas páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-150">Create absolute positioned elements in OneNote pages</span></span>](onenote-abs-pos.md)
* [<span data-ttu-id="e0672-151">Adicionar imagens, vídeos e arquivos a páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-151">Add images, videos, and files to OneNote pages</span></span>](onenote-images-files.md)
* [<span data-ttu-id="e0672-152">Usar marcas DIV da API do OneNote para extrair dados de capturas</span><span class="sxs-lookup"><span data-stu-id="e0672-152">Use OneNote API div tags to extract data from captures</span></span>](onenote-extract-data.md)

## <a name="see-also"></a><span data-ttu-id="e0672-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="e0672-153">See also</span></span>
<span data-ttu-id="e0672-154">Saiba mais sobre alguns outros recursos do OneNote que estão expostos somente no ponto de extremidade REST específico do serviço do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0672-154">Find out about a few other OneNote features that are exposed only on the OneNote service-specific REST endpoint.</span></span>

- [<span data-ttu-id="e0672-155">Desenvolvimento do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-155">OneNote development</span></span>](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-landing)
- [<span data-ttu-id="e0672-156">Trabalhar com Blocos de Anotações de Classe</span><span class="sxs-lookup"><span data-stu-id="e0672-156">Work with class notebooks</span></span>](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-classnotebook)
- [<span data-ttu-id="e0672-157">Trabalhar com blocos de anotações de classe assíncronos</span><span class="sxs-lookup"><span data-stu-id="e0672-157">Work with asynchronous class notebooks</span></span>](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-classnotebook-asynchronous)
- [<span data-ttu-id="e0672-158">Trabalhar com Blocos de Anotações de Equipe</span><span class="sxs-lookup"><span data-stu-id="e0672-158">Work with staff notebooks</span></span>](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-staffnotebook)
- [<span data-ttu-id="e0672-159">Copiar blocos de anotações, seções e páginas</span><span class="sxs-lookup"><span data-stu-id="e0672-159">Copy notebooks, sections, and pages</span></span>](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-copy)
- [<span data-ttu-id="e0672-160">Gerenciar permissões em entidades do OneNote</span><span class="sxs-lookup"><span data-stu-id="e0672-160">Manage permissions on OneNote entities</span></span>](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-manage-perms)
- [<span data-ttu-id="e0672-161">Usar a caixa de diálogo Salvar do OneNote em suas páginas da Web</span><span class="sxs-lookup"><span data-stu-id="e0672-161">Use the OneNote save dialog on your webpages</span></span>](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-save-dialog)
- [<span data-ttu-id="e0672-162">Assinar webhooks</span><span class="sxs-lookup"><span data-stu-id="e0672-162">Subscribe to webhooks</span></span>](https://docs.microsoft.com/pt-BR/previous-versions/office/office-365-api/how-to/onenote-sync)

## <a name="api-reference"></a><span data-ttu-id="e0672-163">Referência da API</span><span class="sxs-lookup"><span data-stu-id="e0672-163">API reference</span></span>
<span data-ttu-id="e0672-164">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="e0672-164">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="e0672-165">API do OneNote no Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="e0672-165">OneNote API in Microsoft Graph v1.0</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0)
- [<span data-ttu-id="e0672-166">API do OneNote no Microsoft Graph beta</span><span class="sxs-lookup"><span data-stu-id="e0672-166">OneNote API in Microsoft Graph beta</span></span>](/graph/api/resources/onenote-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="e0672-167">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e0672-167">Next steps</span></span>

<span data-ttu-id="e0672-168">Use o [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) para experimentar as APIs do OneNote com seus próprios blocos de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0672-168">Use the [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out the OneNote APIs with your own OneNote notebooks.</span></span>

<span data-ttu-id="e0672-169">Para fazer chamadas à API do OneNote por meio do Explorador do Graph, escolha **Mostrar mais exemplos** na coluna à esquerda.</span><span class="sxs-lookup"><span data-stu-id="e0672-169">To make OneNote API calls from the Graph Explorer, choose **Show more samples** in the column on the left.</span></span> <span data-ttu-id="e0672-170">Use o menu para **Ativar** o OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0672-170">Use the menu to toggle OneNote **On**.</span></span> <span data-ttu-id="e0672-171">Você também precisará habilitar as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="e0672-171">You will also need to enable the appropriate permissions.</span></span> <span data-ttu-id="e0672-172">No nome da conta no menu à esquerda, escolha **modificar permissões**.</span><span class="sxs-lookup"><span data-stu-id="e0672-172">Under your account name in the menu on the left, choose **modify permissions**.</span></span> <span data-ttu-id="e0672-173">Para saber mais sobre as permissões do OneNote, confira [Permissões de anotações](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="e0672-173">For more information about OneNote permissions, see [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

<span data-ttu-id="e0672-174">Para começar a usar as APIs do OneNote no Microsoft Graph, confira o [conteúdo de referência do OneNote](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="e0672-174">To get started with OneNote APIs in Microsoft Graph, see the [OneNote reference content](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0).</span></span>

