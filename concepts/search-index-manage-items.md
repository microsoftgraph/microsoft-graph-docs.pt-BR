---
title: Criar, atualizar e excluir itens adicionados por seu aplicativo na conexão do Microsoft Graph
description: Aprenda a usar o Microsoft Graph para gerenciar itens adicionados pelo seu aplicativo ao serviço da Pesquisa da Microsoft
localization_priority: Priority
author: rsamai
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 4ac64724a676c2da2d39a68d842039bd14138161
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883176"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-graph-connection"></a><span data-ttu-id="20e56-103">Criar, atualizar e excluir itens adicionados por seu aplicativo na conexão do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="20e56-103">Create, update, and delete items added by your application in the Microsoft Graph connection</span></span>

<span data-ttu-id="20e56-104">Os itens adicionados por seu aplicativo ao serviço de Pesquisa da Microsoft são representados pelo recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20e56-104">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) resource in Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="20e56-105">Depois de criar uma conexão, você pode adicionar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="20e56-105">Once you have created a connection, you can add your content.</span></span> <span data-ttu-id="20e56-106">Cada item da fonte de dados deve ser representado como um [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) no Microsoft Graph com uma ID de item exclusiva. Essa ID é usada para criar, atualizar ou excluir o item do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20e56-106">Each item from your data source must be represented as an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) in Microsoft Graph with a unique item id. This id is used to create, update or delete the item from Microsoft Graph.</span></span> <span data-ttu-id="20e56-107">Você pode usar a chave primária da fonte de dados como itemId ou derivá-la de um ou mais campos.</span><span class="sxs-lookup"><span data-stu-id="20e56-107">You can use the primary key from your data source as the itemId or derive it from one or more fields.</span></span> <span data-ttu-id="20e56-108">Um [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) possui três componentes principais: lista de controle de acesso, propriedades e conteúdo.</span><span class="sxs-lookup"><span data-stu-id="20e56-108">An [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) has three key components: access control list, properties, and content.</span></span>

## <a name="access-control-list"></a><span data-ttu-id="20e56-109">Lista de controle de acesso</span><span class="sxs-lookup"><span data-stu-id="20e56-109">Access control list</span></span>

<span data-ttu-id="20e56-110">A lista de controle de acesso é usada para especificar se as funções determinadas têm acesso concedido ou negado para exibir itens nas experiências da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20e56-110">The access control list is used to specify whether the given roles are granted or denied access to view items in Microsoft experiences.</span></span> <span data-ttu-id="20e56-111">É uma matriz de entradas de controle de acesso, cada uma representando um usuário ou grupo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="20e56-111">It is an array of access control entries, each representing an Azure Active Directory user or group.</span></span> <span data-ttu-id="20e56-112">Há um terceiro tipo de entrada de controle de acesso `Everyone` que representa todos os usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="20e56-112">There is a third access control entry type `Everyone` that represents all the users in the tenant.</span></span>

![Exemplo de lista de controle de acesso](./images/search-index-manage-items-acl.png)

<span data-ttu-id="20e56-114">O valor accessType `deny` tem precedência sobre `grant`.</span><span class="sxs-lookup"><span data-stu-id="20e56-114">The accessType value `deny` takes precedence over `grant`.</span></span> <span data-ttu-id="20e56-115">Por exemplo, no item mostrado acima, enquanto `Everyone` recebe o acesso e a um usuário específico é negado o acesso, a permissão efetiva desse usuário é `deny`.</span><span class="sxs-lookup"><span data-stu-id="20e56-115">For example, in the item shown above, while `Everyone` is granted access and a specific user is denied access, the effective permission for this user is `deny`.</span></span>

<span data-ttu-id="20e56-116">Se sua fonte de dados tiver grupos não pertencentes ao Azure Active Directory como equipes no sistema de assistência técnica, usado para definir permissões para o item, você poderá criar grupos externos no Microsoft Graph usando as APIs de sincronização do grupo para duplicar as permissões de `allow` ou `deny`.</span><span class="sxs-lookup"><span data-stu-id="20e56-116">If your data source has non Azure Active Directory groups, such as teams within your helpdesk system, used to set permissions for the item, you can create external groups in Microsoft Graph using the group sync APIs to replicate the `allow` or `deny` permissions.</span></span> <span data-ttu-id="20e56-117">Evite expandir a afiliação dos seus grupos externos diretamente nas listas de controle de acesso de itens individuais, uma vez que cada atualização de afiliação ao grupo pode levar a um tumulto de atualizações de itens.</span><span class="sxs-lookup"><span data-stu-id="20e56-117">Avoid expanding the membership of your external groups directly into the access control lists of individual items since each group membership update could lead to a storm of item updates.</span></span>

<span data-ttu-id="20e56-118">Os grupos externos podem consistir em outro grupo externo, usuários do Azure Active Directory e grupos do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="20e56-118">External groups can consist of another external group, Azure Active Directory users, and Azure Active Directory groups.</span></span> <span data-ttu-id="20e56-119">Se você tiver usuários que não são do Azure Active Directory, deve traduzi-los para os usuários do Azure Active Directory na lista de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="20e56-119">If you have non-Azure Active Directory users, you must translate them to Azure Active Directory users in your access control list.</span></span>

## <a name="properties"></a><span data-ttu-id="20e56-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20e56-120">Properties</span></span>

<span data-ttu-id="20e56-121">O componente propriedades é usado para adicionar metadados de itens que são úteis nas experiências do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20e56-121">The properties component is used to add item metadata that is useful in Microsoft Graph experiences.</span></span> <span data-ttu-id="20e56-122">Você deve [registrar o esquema](./search-index-manage-schema.md) para a conexão antes de adicionar itens a ele e converter os tipos de dados em [tipos de dados com suporte](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="20e56-122">You must [register the schema](./search-index-manage-schema.md) for the connection before adding items into it and convert datatypes into [supported datatypes](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true).</span></span>

![Exemplo de um componente de propriedade](./images/search-index-manage-items-1.png)

## <a name="content"></a><span data-ttu-id="20e56-124">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="20e56-124">Content</span></span>

<span data-ttu-id="20e56-125">O componente de conteúdo é usado para adicionar a maior parte do item que deve ser indexado em texto completo.</span><span class="sxs-lookup"><span data-stu-id="20e56-125">The content component is used to add the bulk of the item that needs to be full text indexed.</span></span> <span data-ttu-id="20e56-126">Alguns exemplos incluem a descrição do tíquete, texto analisado de um corpo de arquivo ou um corpo de página wiki.</span><span class="sxs-lookup"><span data-stu-id="20e56-126">Examples include ticket description, parsed text from a file body, or a wiki page body.</span></span>

<span data-ttu-id="20e56-127">O conteúdo é um dos principais campos que influenciam na [relevância](./search-index-manage-schema.md#relevance) nas experiências da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20e56-127">Content is one of the key fields influencing [relevance](./search-index-manage-schema.md#relevance) across Microsoft experiences.</span></span> <span data-ttu-id="20e56-128">Oferecemos suporte para o tipo de conteúdo `text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="20e56-128">We support content of the type `text` and `HTML`.</span></span> <span data-ttu-id="20e56-129">Se sua fonte de dados tiver arquivos binários, você poderá analisá-los como texto antes de adicioná-los ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="20e56-129">If your data source has binary files, you can parse them to text before adding them to Microsoft Graph.</span></span>

![Um exemplo de componente de conteúdo](./images/search-index-manage-items-2.png)

<span data-ttu-id="20e56-131">O conteúdo não pode ser adicionado diretamente a um modelo de resultado de pesquisa, mas você pode usar um trecho de resultado gerado, que é uma prévia gerada dinamicamente das seções relevantes dentro do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="20e56-131">Content cannot be directly added into a search result template, but you can use a generated result snippet which is a dynamically generated preview of the relevant sections within content.</span></span>

![Uma captura de tela de um modelo de resultado de pesquisa](./images/search-index-manage-items-3.svg)

<span data-ttu-id="20e56-133">Quando o conteúdo da fonte de dados é alterado, você deve sincronizá-lo com seus itens de conexão.</span><span class="sxs-lookup"><span data-stu-id="20e56-133">When content in your data source changes, you must sync it with your connection items.</span></span> <span data-ttu-id="20e56-134">Você pode atualizar o item inteiro ou atualizar um ou mais dos seus componentes.</span><span class="sxs-lookup"><span data-stu-id="20e56-134">You can either update the entire item or update one or more of its components.</span></span> <span data-ttu-id="20e56-135">Depois que o conteúdo tiver sido adicionado ao Microsoft Graph, você poderá pesquisá-lo por meio da experiência de Pesquisa da Microsoft após configurar [verticais e tipos de resultado](/MicrosoftSearch/customize-search-page) ou usar a [API da Pesquisa da Microsoft Graph](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="20e56-135">Once your content has been added to Microsoft Graph, you can search for it through the Microsoft Search experience after setting up [verticals and result types](/MicrosoftSearch/customize-search-page) or using the [Microsoft Graph Search API](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="add-an-item"></a><span data-ttu-id="20e56-136">Adicionar um item</span><span class="sxs-lookup"><span data-stu-id="20e56-136">Add an item</span></span>

<span data-ttu-id="20e56-137">Você pode adicionar um item ao índice [criando um externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="20e56-137">You can add an item to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="20e56-138">Ao criar um item, você atribui um identificador exclusivo na URL.</span><span class="sxs-lookup"><span data-stu-id="20e56-138">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="20e56-139">Por exemplo, seu aplicativo pode indexar tíquetes de assistência técnica usando o número do tíquete.</span><span class="sxs-lookup"><span data-stu-id="20e56-139">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="20e56-140">Se um tíquete tiver o número do tíquete `SR00145`, a solicitação poderá ser semelhante à seguinte.</span><span class="sxs-lookup"><span data-stu-id="20e56-140">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> <span data-ttu-id="20e56-141">![OBSERVAÇÃO] Antes que os itens indexados possam ser encontrados na IU da Pesquisa da Microsoft, um administrador deve [personalizar a página de resultados de pesquisa](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) para a conexão correspondente.</span><span class="sxs-lookup"><span data-stu-id="20e56-141">![NOTE] Before indexed items can be found in the Microsoft Search UI, an administrator must [customize the search results page](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) for the corresponding connection.</span></span>

## <a name="update-an-item"></a><span data-ttu-id="20e56-142">Atualizar um item</span><span class="sxs-lookup"><span data-stu-id="20e56-142">Update an item</span></span>

<span data-ttu-id="20e56-143">Quando um item é atualizado no serviço externo (o tíquete de assistência técnica é reatribuído ou uma descrição de produto é atualizada), você pode atualizar a respectiva entrada no índice [atualizando o externalItem](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true), usando o identificador exclusivo atribuído ao item quando ele foi criado.</span><span class="sxs-lookup"><span data-stu-id="20e56-143">When an item is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a><span data-ttu-id="20e56-144">Excluir um item</span><span class="sxs-lookup"><span data-stu-id="20e56-144">Delete an item</span></span>

<span data-ttu-id="20e56-145">Você pode remover os itens do índice [excluindo o externalItem](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true), usando o identificador exclusivo atribuído ao item quando ele foi criado.</span><span class="sxs-lookup"><span data-stu-id="20e56-145">You can remove items from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a><span data-ttu-id="20e56-146">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="20e56-146">Next steps</span></span>

- [<span data-ttu-id="20e56-147">Consulta usando a API de Pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="20e56-147">Query using the Microsoft Search API</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="20e56-148">Examine a referência da API de indexação</span><span class="sxs-lookup"><span data-stu-id="20e56-148">Review the Indexing API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="20e56-149">Personalizar a página de resultados da pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="20e56-149">Customize Microsoft Search results page</span></span>](/MicrosoftSearch/customize-search-page)
- [<span data-ttu-id="20e56-150">Pesquisar tipos personalizados (externalItem)</span><span class="sxs-lookup"><span data-stu-id="20e56-150">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- <span data-ttu-id="20e56-151">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub</span><span class="sxs-lookup"><span data-stu-id="20e56-151">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>