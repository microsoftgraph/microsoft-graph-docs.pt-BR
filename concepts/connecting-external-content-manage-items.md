---
title: Criar, atualizar e excluir itens adicionados por seu aplicativo na conexão do Microsoft Graph
description: Aprenda a usar o Microsoft Graph para gerenciar itens adicionados pelo seu aplicativo ao serviço Pesquisa da Microsoft
localization_priority: Priority
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 141228dcefa35e8195e3095996e2c3157e9771f0
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645651"
---
<!---<author of this doc: rsamai>--->

# <a name="create-update-and-delete-items-added-by-your-application-via-microsoft-graph-connectors"></a><span data-ttu-id="faa53-103">Criar, atualizar e excluir itens adicionados por seu aplicativo via conectores do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="faa53-103">Create, update, and delete items added by your application via Microsoft Graph connectors</span></span>

<span data-ttu-id="faa53-104">A plataforma de conectores do Microsoft Graph oferece uma maneira simples de adicionar seus dados externos ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="faa53-104">Microsoft Graph connectors offer a simple way to bring external data into Microsoft Graph.</span></span> <span data-ttu-id="faa53-105">Os itens adicionados por seu aplicativo ao serviço Pesquisa da Microsoft são representados pelo recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="faa53-105">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) resource in Microsoft Graph.</span></span>

<span data-ttu-id="faa53-106">Depois de [criar uma conexão](/graph/api/external-post-connections?view=graph-rest-beta&preserve-view=true) e, você pode adicionar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="faa53-106">After you have [created a connection](/graph/api/external-post-connections?view=graph-rest-beta&preserve-view=true), you can add your content.</span></span> <span data-ttu-id="faa53-107">Cada item da fonte de dados deve ser representado como um [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) no Microsoft Graph com uma ID de item exclusiva.</span><span class="sxs-lookup"><span data-stu-id="faa53-107">Each item from your data source must be represented as an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) in Microsoft Graph with a unique item ID.</span></span> <span data-ttu-id="faa53-108">Essa ID é usada para criar, atualizar ou excluir o item do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="faa53-108">This ID is used to create, update, or delete the item from Microsoft Graph.</span></span> <span data-ttu-id="faa53-109">Você pode usar a chave primária da fonte de dados como itemId ou derivá-la de um ou mais campos.</span><span class="sxs-lookup"><span data-stu-id="faa53-109">You can use the primary key from your data source as the itemId or derive it from one or more fields.</span></span> <span data-ttu-id="faa53-110">Um **externalItem** possui três componentes principais: lista de controle de acesso, propriedades e conteúdo.</span><span class="sxs-lookup"><span data-stu-id="faa53-110">An **externalItem** has three key components: access control list, properties, and content.</span></span>

## <a name="access-control-list"></a><span data-ttu-id="faa53-111">Lista de controle de acesso</span><span class="sxs-lookup"><span data-stu-id="faa53-111">Access control list</span></span>

<span data-ttu-id="faa53-112">A lista de controle de acesso é usada para especificar se as funções determinadas têm acesso concedido ou negado para exibir itens nas experiências da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="faa53-112">The access control list is used to specify whether the given roles are granted or denied access to view items in Microsoft experiences.</span></span> <span data-ttu-id="faa53-113">É uma matriz de entradas de controle de acesso, cada uma representando um usuário ou grupo do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="faa53-113">It is an array of access control entries, each representing an Azure Active Directory user or group.</span></span> <span data-ttu-id="faa53-114">Um terceiro tipo de entrada de controle de acesso `Everyone` que representa todos os usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="faa53-114">A third access control entry type `Everyone` that represents all the users in the tenant.</span></span>

![Um exemplo de lista de controle de acesso](./images/connectors-images/connecting-external-content-manage-items-acl.png)

<span data-ttu-id="faa53-116">O valor **accessType** `deny` tem precedência sobre `grant`.</span><span class="sxs-lookup"><span data-stu-id="faa53-116">The **accessType** value `deny` takes precedence over `grant`.</span></span> <span data-ttu-id="faa53-117">Por exemplo, no item mostrado acima, enquanto `Everyone` recebe o acesso e um usuário específico tem negado o acesso, a permissão efetiva desse usuário é `deny`.</span><span class="sxs-lookup"><span data-stu-id="faa53-117">For example, in the item shown earlier, while `Everyone` is granted access and a specific user is denied access, the effective permission for this user is `deny`.</span></span>

<span data-ttu-id="faa53-118">Se sua fonte de dados tiver grupos não pertencentes ao Azure Active Directory como equipes no sistema de assistência técnica, usado para definir permissões para o item, você poderá criar grupos externos no Microsoft Graph usando as APIs de sincronização do grupo para duplicar as permissões de `allow` ou `deny`.</span><span class="sxs-lookup"><span data-stu-id="faa53-118">If your data source has non-Azure Active Directory groups, such as teams within your helpdesk system, used to set permissions for the item, you can create external groups in Microsoft Graph using the group sync APIs to replicate the `allow` or `deny` permissions.</span></span> <span data-ttu-id="faa53-119">Evite expandir a afiliação dos seus grupos externos diretamente nas listas de controle de acesso de itens individuais, uma vez que cada afiliação ao grupo pode levar a um tumulto de atualizações de itens.</span><span class="sxs-lookup"><span data-stu-id="faa53-119">Avoid expanding the membership of your external groups directly into the access control lists of individual items, because each group membership can lead to a high volume of item updates.</span></span>

<span data-ttu-id="faa53-120">Os grupos externos podem consistir em outro grupo externo, usuários do Azure Active Directory e grupos do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="faa53-120">External groups can consist of another external group, Azure Active Directory users, and Azure Active Directory groups.</span></span> <span data-ttu-id="faa53-121">Se você tiver usuários que não são do Azure Active Directory, deve traduzi-los para os usuários do Azure Active Directory na lista de controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="faa53-121">If you have non-Azure Active Directory users, you must translate them to Azure Active Directory users in your access control list.</span></span>

## <a name="properties"></a><span data-ttu-id="faa53-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faa53-122">Properties</span></span>

<span data-ttu-id="faa53-123">O componente propriedades é usado para adicionar metadados de itens que são úteis nas experiências do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="faa53-123">The properties component is used to add item metadata that is useful in Microsoft Graph experiences.</span></span> <span data-ttu-id="faa53-124">Você deve [registrar o esquema](./connecting-external-content-manage-schema.md) para a conexão antes de adicionar itens a ele e converter os **tipos de dados** em [tipos de dados com suporte](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="faa53-124">You must [register the schema](./connecting-external-content-manage-schema.md) for the connection before adding items into it and convert **datatypes** into [supported datatypes](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true).</span></span>

![Exemplo de um componente de propriedade](./images/connectors-images/connecting-external-content-manage-items-1.png)

## <a name="content"></a><span data-ttu-id="faa53-126">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="faa53-126">Content</span></span>

<span data-ttu-id="faa53-127">O componente de conteúdo é usado para adicionar a maior parte do item que deve ser indexado em texto completo.</span><span class="sxs-lookup"><span data-stu-id="faa53-127">The content component is used to add the bulk of the item that needs to be full text indexed.</span></span> <span data-ttu-id="faa53-128">Alguns exemplos incluem a descrição do tíquete, texto analisado de um corpo de arquivo ou um corpo de página wiki.</span><span class="sxs-lookup"><span data-stu-id="faa53-128">Examples include ticket description, parsed text from a file body, or a wiki page body.</span></span>

<span data-ttu-id="faa53-129">O conteúdo é um dos principais campos que influenciam na [relevância](./connecting-external-content-manage-schema.md#relevance) nas experiências da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="faa53-129">Content is one of the key fields influencing [relevance](./connecting-external-content-manage-schema.md#relevance) across Microsoft experiences.</span></span> <span data-ttu-id="faa53-130">Os tipos de conteúdo `text` e `HTML` são suportados.</span><span class="sxs-lookup"><span data-stu-id="faa53-130">The content types `text` and `HTML` are supported.</span></span> <span data-ttu-id="faa53-131">Se sua fonte de dados tiver arquivos binários, você poderá analisá-los como texto antes de adicioná-los ao Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="faa53-131">If your data source has binary files, you can parse them to text before adding them to Microsoft Graph.</span></span>

![Um exemplo de componente de conteúdo](./images/connectors-images/connecting-external-content-manage-items-2.png)

<span data-ttu-id="faa53-133">O conteúdo não pode ser adicionado diretamente a um modelo de resultado de pesquisa, mas você pode usar um trecho de resultado gerado, que é uma prévia gerada dinamicamente das seções relevantes dentro do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="faa53-133">Content cannot be directly added into a search result template, but you can use a generated result snippet, which is a dynamically generated preview of the relevant sections within content.</span></span>

![Uma captura de tela de um modelo de resultado de pesquisa](./images/connectors-images/connecting-external-content-manage-items-3.svg)

<span data-ttu-id="faa53-135">Quando o conteúdo da fonte de dados é alterado, você deve sincronizá-lo com seus itens de conexão.</span><span class="sxs-lookup"><span data-stu-id="faa53-135">When content in your data source changes, you must sync it with your connection items.</span></span> <span data-ttu-id="faa53-136">Você pode atualizar o item inteiro ou atualizar um ou mais dos seus componentes.</span><span class="sxs-lookup"><span data-stu-id="faa53-136">You can either update the entire item or update one or more of its components.</span></span> <span data-ttu-id="faa53-137">Depois que o conteúdo tiver sido adicionado ao Microsoft Graph, você poderá pesquisá-lo por meio da experiência de Pesquisa da Microsoft após configurar [verticais e tipos de resultado](/MicrosoftSearch/customize-search-page) ou usar a [API da Pesquisa da Microsoft Graph](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="faa53-137">Once your content has been added to Microsoft Graph, you can search for it through the Microsoft Search experience after setting up [verticals and result types](/MicrosoftSearch/customize-search-page) or using the [Microsoft Graph Search API](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="add-an-item"></a><span data-ttu-id="faa53-138">Adicionar um item</span><span class="sxs-lookup"><span data-stu-id="faa53-138">Add an item</span></span>

<span data-ttu-id="faa53-139">Você pode adicionar um item ao índice [criando um externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="faa53-139">You can add an item to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="faa53-140">Ao criar um item, você atribui um identificador exclusivo na URL.</span><span class="sxs-lookup"><span data-stu-id="faa53-140">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="faa53-141">Por exemplo, seu aplicativo pode indexar tíquetes de assistência técnica usando o número do tíquete.</span><span class="sxs-lookup"><span data-stu-id="faa53-141">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="faa53-142">Se um tíquete tiver o número do tíquete `SR00145`, a solicitação poderá ser semelhante à seguinte.</span><span class="sxs-lookup"><span data-stu-id="faa53-142">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> <span data-ttu-id="faa53-143">![OBSERVAÇÃO] Antes que os itens indexados possam ser encontrados na IU da Pesquisa da Microsoft, um administrador deve [personalizar a página de resultados de pesquisa](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) para a conexão correspondente.</span><span class="sxs-lookup"><span data-stu-id="faa53-143">![NOTE] Before indexed items can be found in the Microsoft Search UI, an administrator must [customize the search results page](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) for the corresponding connection.</span></span>

## <a name="update-an-item"></a><span data-ttu-id="faa53-144">Atualizar um item</span><span class="sxs-lookup"><span data-stu-id="faa53-144">Update an item</span></span>

<span data-ttu-id="faa53-145">Quando um item é atualizado no serviço externo (o tíquete de assistência técnica é reatribuído ou uma descrição de produto é atualizada), você pode atualizar a respectiva entrada no índice [atualizando o externalItem](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true), usando o identificador exclusivo atribuído ao item quando ele foi criado.</span><span class="sxs-lookup"><span data-stu-id="faa53-145">When an item is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a><span data-ttu-id="faa53-146">Excluir um item</span><span class="sxs-lookup"><span data-stu-id="faa53-146">Delete an item</span></span>

<span data-ttu-id="faa53-147">Você pode remover os itens do índice [excluindo o externalItem](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true), usando o identificador exclusivo atribuído ao item quando ele foi criado.</span><span class="sxs-lookup"><span data-stu-id="faa53-147">You can remove items from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="see-also"></a><span data-ttu-id="faa53-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="faa53-148">See also</span></span>

- [<span data-ttu-id="faa53-149">Consulta usando a API de Pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="faa53-149">Query using the Microsoft Search API</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="faa53-150">Examine a referência da API de indexação</span><span class="sxs-lookup"><span data-stu-id="faa53-150">Review the Indexing API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="faa53-151">Personalizar a página de resultados da pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="faa53-151">Customize Microsoft Search results page</span></span>](/MicrosoftSearch/customize-search-page)
- [<span data-ttu-id="faa53-152">Pesquisar tipos personalizados (externalItem)</span><span class="sxs-lookup"><span data-stu-id="faa53-152">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- <span data-ttu-id="faa53-153">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub</span><span class="sxs-lookup"><span data-stu-id="faa53-153">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>