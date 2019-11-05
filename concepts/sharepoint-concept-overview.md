---
title: Visão geral da API de conteúdo e sites do SharePoint
description: O SharePoint é sua Intranet móvel e inteligente. Com o SharePoint, os usuários podem compartilhar e gerenciar conteúdo, conhecimentos e aplicativos para capacitar o trabalho em equipe, encontrar informações e colaborar em uma organização. Você pode usar a API REST do SharePoint no Microsoft Graph para integrar suas soluções a conteúdo e sites do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.custom: scenarios:getting-started
ms.openlocfilehash: 5b0424aa2bca03b4feecdd565ab77825d6a68ee3
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969358"
---
# <a name="sharepoint-sites-and-content-api-overview"></a><span data-ttu-id="6195e-105">Visão geral da API de conteúdo e sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="6195e-105">SharePoint sites and content API overview</span></span>

<span data-ttu-id="6195e-106">O SharePoint é sua Intranet móvel e inteligente.</span><span class="sxs-lookup"><span data-stu-id="6195e-106">SharePoint is your mobile, intelligent intranet.</span></span> <span data-ttu-id="6195e-107">Com o SharePoint, os usuários podem compartilhar e gerenciar conteúdo, conhecimentos e aplicativos para capacitar o trabalho em equipe, encontrar informações e colaborar em uma organização.</span><span class="sxs-lookup"><span data-stu-id="6195e-107">With SharePoint, users can share and manage content, knowledge, and applications to empower teamwork, find information, and collaborate across an organization.</span></span> <span data-ttu-id="6195e-108">Você pode usar a API REST do SharePoint no Microsoft Graph para integrar suas soluções a conteúdo e sites do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6195e-108">You can use the SharePoint REST API in Microsoft Graph to integrate your solutions with SharePoint sites and content.</span></span>

## <a name="why-integrate-with-sharepoint-sites-and-content"></a><span data-ttu-id="6195e-109">Por que integrar com conteúdo e sites do SharePoint?</span><span class="sxs-lookup"><span data-stu-id="6195e-109">Why integrate with SharePoint sites and content?</span></span>

<span data-ttu-id="6195e-110">Sites do SharePoint possibilitam a comunicação e a colaboração em equipe.</span><span class="sxs-lookup"><span data-stu-id="6195e-110">SharePoint sites power team collaboration and communication.</span></span> <span data-ttu-id="6195e-111">Os Grupos do Office 365, o Microsoft Teams e os portais são baseados no SharePoint, portanto, você pode usar o Microsoft Graph para acessar dados onde quer que eles sejam mantidos.</span><span class="sxs-lookup"><span data-stu-id="6195e-111">Office 365 groups, Microsoft Teams, and portals are all based on SharePoint, so you can use Microsoft Graph to access data no matter where it's kept.</span></span> <span data-ttu-id="6195e-112">Use a API do SharePoint no Microsoft Graph para acessar:</span><span class="sxs-lookup"><span data-stu-id="6195e-112">Use the SharePoint API in Microsoft Graph to access:</span></span>

- <span data-ttu-id="6195e-113">Sites de equipe que armazenam o conteúdo no qual os usuários colaboraram com seus colegas de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6195e-113">Team sites that store the content that users collaborate on with their coworkers.</span></span>
- <span data-ttu-id="6195e-114">Sites e portais de comunicação em que os usuários publicam páginas de conteúdo avançado para compartilhar em toda a organização.</span><span class="sxs-lookup"><span data-stu-id="6195e-114">Communication sites and portals where users publish rich content pages to share across the organization.</span></span>

### <a name="unleash-your-data-with-sharepoint-lists"></a><span data-ttu-id="6195e-115">Potencialize seus dados com listas do SharePoint</span><span class="sxs-lookup"><span data-stu-id="6195e-115">Unleash your data with SharePoint lists</span></span>

<span data-ttu-id="6195e-116">As [Listas][lista] são a base do armazenamento de dados no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6195e-116">[Lists][list] are the foundation for data storage in SharePoint.</span></span>
<span data-ttu-id="6195e-117">[Crie listas][criar] para armazenar uma variedade de dados corporativos, desde uma simples lista de contatos de clientes até um aplicativo corporativo personalizado com o PowerApps.</span><span class="sxs-lookup"><span data-stu-id="6195e-117">[Create lists][create] to store a variety of business data, from a simple customer contact list to a custom business application, fronted with PowerApps.</span></span>
<span data-ttu-id="6195e-118">Quando você usa [colunas][] para definir o esquema, o SharePoint pode proteger a integridade de seus dados e habilitar recursos avançados de indexação, consulta e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6195e-118">When you use [columns][] to define your schema, SharePoint can protect the integrity of your data as well as enable  rich indexing, querying, and search capabilities.</span></span>

### <a name="bring-the-power-of-lists-to-your-teams-files"></a><span data-ttu-id="6195e-119">Leve o poder de listas para os arquivos da sua equipe</span><span class="sxs-lookup"><span data-stu-id="6195e-119">Bring the power of lists to your team's files</span></span>

<span data-ttu-id="6195e-120">O SharePoint armazena arquivos em um [tipo de lista][] especial chamado biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="6195e-120">SharePoint stores files in a special [list type][] called a document library.</span></span>
<span data-ttu-id="6195e-121">Você pode usar a [API do OneDrive][] para trabalhar com uma biblioteca como uma [unidade][], ou a API do SharePoint para trabalhar com ela como uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="6195e-121">You can use the [OneDrive API][] to work with a library as a [drive][], or the SharePoint API to work with it as a [list][].</span></span>
<span data-ttu-id="6195e-122">Assim como com uma lista normal, você pode ampliar o esquema de uma Biblioteca de documentos para atender às suas necessidades de negócios com colunas personalizadas.</span><span class="sxs-lookup"><span data-stu-id="6195e-122">Just like a regular list, you can extend the schema of a Document Library to support your business needs with custom columns.</span></span>

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a><span data-ttu-id="6195e-123">Aprimore seu aplicativo com os dados da Intranet do SharePoint de seus usuários</span><span class="sxs-lookup"><span data-stu-id="6195e-123">Light up your app with your users' SharePoint intranet data</span></span>

<span data-ttu-id="6195e-124">Com o Microsoft Graph, você pode exibir os dados mais importantes dos seus usuários no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6195e-124">With Microsoft Graph, you can surface your users' most important data within your app.</span></span>
<span data-ttu-id="6195e-125">Mantenha os dados atualizados ao [consultar][] a lista que armazena os dados dos seus usuários.</span><span class="sxs-lookup"><span data-stu-id="6195e-125">Keep things fresh by [querying][] the list that stores your users' data.</span></span>
<span data-ttu-id="6195e-126">[Crie][] suas próprias listas para os usuários do seu aplicativo e permita que eles acessem seus dados em outras experiências do SharePoint ou mantenha os dados ocultos.</span><span class="sxs-lookup"><span data-stu-id="6195e-126">[Create][] your own lists for your app and let users access your data in other SharePoint experiences, or keep things hidden.</span></span>

### <a name="use-microsoft-graph-to-extend-sharepoint"></a><span data-ttu-id="6195e-127">Use o Microsoft Graph para aprimorar o SharePoint</span><span class="sxs-lookup"><span data-stu-id="6195e-127">Use Microsoft Graph to extend SharePoint</span></span>

<span data-ttu-id="6195e-128">Como uma plataforma, o SharePoint oferece vários modelos de extensão e integração:</span><span class="sxs-lookup"><span data-stu-id="6195e-128">As a platform, SharePoint provides several models for extension and integration:</span></span>

- <span data-ttu-id="6195e-129">A [Estrutura do SharePoint][] fornece uma maneira de compilar Web Parts usando tecnologias do lado do cliente e ferramentas de código aberto que podem ser hospedadas em páginas do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6195e-129">The [SharePoint Framework][] provides a way to build web parts using client-side technologies and open source tooling that can be hosted on SharePoint pages.</span></span>
- <span data-ttu-id="6195e-130">[Suplementos do SharePoint][] são extensões autônomas que podem ser adicionadas a um site do SharePoint sem a necessidade de um código personalizado em execução no servidor.</span><span class="sxs-lookup"><span data-stu-id="6195e-130">[SharePoint Add-ins][] are self-contained extensions that can be added to a SharePoint site without the need for custom code to run on the server.</span></span>

<span data-ttu-id="6195e-131">Quando seu aplicativo é executado em uma página do SharePoint, você pode usar o Microsoft Graph facilmente para acessar dados no Office 365.</span><span class="sxs-lookup"><span data-stu-id="6195e-131">When your app runs within a SharePoint page, you can easily use Microsoft Graph to access data across Office 365.</span></span>

<span data-ttu-id="6195e-132">Para saber mais sobre esses modelos, acesse o [Centro de Desenvolvedores do SharePoint][] ou os [Documentos para Desenvolvedores do SharePoint][].</span><span class="sxs-lookup"><span data-stu-id="6195e-132">To learn about these models in more detail, visit the [SharePoint Dev Center][] or the [SharePoint Developer Docs][].</span></span>

## <a name="api-reference"></a><span data-ttu-id="6195e-133">Referência da API</span><span class="sxs-lookup"><span data-stu-id="6195e-133">API reference</span></span>
<span data-ttu-id="6195e-134">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="6195e-134">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="6195e-135">API do SharePoint no Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="6195e-135">SharePoint API in Microsoft Graph v1.0</span></span>](/graph/api/resources/sharepoint?view=graph-rest-1.0)
- [<span data-ttu-id="6195e-136">API do SharePoint no Microsoft Graph beta</span><span class="sxs-lookup"><span data-stu-id="6195e-136">SharePoint API in Microsoft Graph beta</span></span>](/graph/api/resources/sharepoint?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="6195e-137">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6195e-137">Next steps</span></span>

<span data-ttu-id="6195e-138">Comece a usar o SharePoint no Microsoft Graph aprendendo mais sobre como [trabalhar com sites](/graph/api/resources/sharepoint?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="6195e-138">Get started with SharePoint in Microsoft Graph by learning more about [working with sites](/graph/api/resources/sharepoint?view=graph-rest-1.0).</span></span>

[list]: /graph/api/resources/list?view=graph-rest-1.0
[colunas]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[columns]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[tipo de lista]: /graph/api/resources/listinfo?view=graph-rest-1.0
[list type]: /graph/api/resources/listinfo?view=graph-rest-1.0
[criar]: /graph/api/list-create?view=graph-rest-1.0
[create]: /graph/api/list-create?view=graph-rest-1.0
[consultar]: /graph/api/listitem-get?view=graph-rest-1.0
[querying]: /graph/api/listitem-get?view=graph-rest-1.0
[unidade]: /graph/api/resources/drive?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[API do OneDrive]: /graph/api/resources/onedrive?view=graph-rest-1.0
[OneDrive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[Estrutura do SharePoint]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[SharePoint Framework]: https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview
[Suplementos do SharePoint]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint Add-ins]: https://docs.microsoft.com/sharepoint/dev/sp-add-ins/sharepoint-add-ins
[Centro de Desenvolvedores do SharePoint]: https://developer.microsoft.com/sharepoint
[SharePoint Dev Center]: https://developer.microsoft.com/sharepoint
[Documentos para Desenvolvedores do SharePoint]: https://aka.ms/spdev-docs
[SharePoint Developer Docs]: https://aka.ms/spdev-docs
[SharePoint]: /graph/api/resources/sharepoint?view=graph-rest-1.0
