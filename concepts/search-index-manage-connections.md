---
title: Criar, atualizar e excluir conexões com o serviço da Pesquisa da Microsoft
description: Aprenda a usar o Microsoft Graph para gerenciar conexões com o serviço da Pesquisa da Microsoft
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 99f0ab4591caa6c311f2771f1c6a0772a8f16087
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892797"
---
# <a name="create-update-and-delete-connections-to-the-microsoft-search-service"></a><span data-ttu-id="e2ab9-103">Criar, atualizar e excluir conexões com o serviço da Pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e2ab9-103">Create, update, and delete connections to the Microsoft Search service</span></span>

<span data-ttu-id="e2ab9-104">As conexões de serviços externos com o serviço da Pesquisa da Microsoft são representadas pelo recurso [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e2ab9-104">Connections from external services to the Microsoft Search service are represented by the [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) resource in Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="e2ab9-105">Uma conexão permite que seu aplicativo [defina um esquema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) para os itens que serão indexados e forneça um ponto de extremidade para o seu serviço [adicionar, atualizar ou excluir itens do índice](search-index-manage-items.md).</span><span class="sxs-lookup"><span data-stu-id="e2ab9-105">A connection allows your application to [define a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) for items that will be indexed, and provides an endpoint for your service to [add, update, or delete items from the index](search-index-manage-items.md).</span></span> <span data-ttu-id="e2ab9-106">Criar uma conexão é a primeira etapa para um aplicativo para adicionar itens ao índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e2ab9-106">Creating a connection is the first step for an application to add items to the search index.</span></span>

## <a name="create-a-connection"></a><span data-ttu-id="e2ab9-107">Criar uma conexão</span><span class="sxs-lookup"><span data-stu-id="e2ab9-107">Create a connection</span></span>

<span data-ttu-id="e2ab9-108">Antes que um aplicativo possa adicionar itens ao índice de pesquisa, ele deve criar e configurar uma conexão usando as etapas a seguir.</span><span class="sxs-lookup"><span data-stu-id="e2ab9-108">Before an application can add items to the search index, it must create and configure a connection using the following steps.</span></span>

- <span data-ttu-id="e2ab9-109">[Criar uma conexão](/graph/api/external-post-connections?view=graph-rest-beta) com ID exclusiva, nome de exibição e descrição.</span><span class="sxs-lookup"><span data-stu-id="e2ab9-109">[Create a connection](/graph/api/external-post-connections?view=graph-rest-beta) with a unique ID, display name, and description.</span></span>
- <span data-ttu-id="e2ab9-110">[Registre um esquema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) para definir os campos que serão incluídos no índice.</span><span class="sxs-lookup"><span data-stu-id="e2ab9-110">[Register a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) to define the fields that will be included in the index.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e2ab9-111">Depois que um esquema é registrado, ele não pode ser alterado para uma conexão existente.</span><span class="sxs-lookup"><span data-stu-id="e2ab9-111">Once a schema has been registered, it cannot be changed for an existing connection.</span></span>

## <a name="update-a-connection"></a><span data-ttu-id="e2ab9-112">Atualizar uma conexão</span><span class="sxs-lookup"><span data-stu-id="e2ab9-112">Update a connection</span></span>

<span data-ttu-id="e2ab9-113">Você pode alterar o nome de exibição ou a descrição de uma conexão existente [atualizando a conexão](/graph/api/externalconnection-update?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="e2ab9-113">You can change the display name or description of an existing connection by [updating the connection](/graph/api/externalconnection-update?view=graph-rest-beta).</span></span>

## <a name="delete-a-connection"></a><span data-ttu-id="e2ab9-114">Excluir uma conexão</span><span class="sxs-lookup"><span data-stu-id="e2ab9-114">Delete a connection</span></span>

<span data-ttu-id="e2ab9-115">Você pode [excluir uma conexão](/graph/api/externalconnection-delete?view=graph-rest-beta) e remover todos os itens que foram indexados por meio da conexão.</span><span class="sxs-lookup"><span data-stu-id="e2ab9-115">You can [delete a connection](/graph/api/externalconnection-delete?view=graph-rest-beta), and remove all items that were indexed via that connection.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e2ab9-116">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e2ab9-116">Next steps</span></span>

- [<span data-ttu-id="e2ab9-117">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="e2ab9-117">Why use the Microsoft Search API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="e2ab9-118">Examine a referência da API de indexação</span><span class="sxs-lookup"><span data-stu-id="e2ab9-118">Review the Indexing API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="e2ab9-119">Visão geral dos conectores do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e2ab9-119">Overview for Microsoft Graph Connectors</span></span>](/microsoftsearch/connectors-overview)
- <span data-ttu-id="e2ab9-120">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub</span><span class="sxs-lookup"><span data-stu-id="e2ab9-120">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
